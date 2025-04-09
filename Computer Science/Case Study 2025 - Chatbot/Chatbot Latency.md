The only valuable source from the [case study doc](https://docs.google.com/document/d/1DoSZb8THuHoYBR7W97kslzA4GOVKUN0lpPFHo4NlDJs/edit?tab=t.0) on latency is this: *[https://platform.openai.com/docs/guides/latency-optimization](https://platform.openai.com/docs/guides/latency-optimization)*

In general 4 main factors influence an LLMs latency, namely: [[#Inference Speed|Model Size/Inference Speed]], [[#Generated Token Quantity]], [[#Input Token Quantity]] and [[#Request Quantity]]. By addressing the aforementioned concerns and utilizing [[#Parallelization]] with [[#Other Techniques]], LLM latency can be improved

<br>


### Inference Speed

Inference speed refers the rate at which an LLM processes tokens, often measured in TMP (tokens per minute) or TPS (tokens per second)

*How to improve?*

The main factor that influences inference speed is **model size** – smaller models usually run faster (and cheaper)

### Generated Token Quantity

Generating tokens is almost always the highest latency step when using an LLM: as a general heuristic, **cutting 50% of your output tokens may cut ~50% your latency**. 
*How to improve?*

The way you reduce your output size will depend on output type:
- Models which generate *Natural Language* may perform faster when asked to be "brief", i.e. generate fewer tokens
- Models which generate *Structured Output* may perform faster when minimizing output syntax: shorten function names, omit named arguments, coalesce parameters, etc

### Input Token Quantity

In contrast to [[#Generated Token Quantity]], input token *quantity* is not usually a significant factor - **cutting 50% of your prompt may only result in a 1-5% latency improvement**. 

The only case where the quantity of input tokens appears significant is when utilizing massive contexts (documents, images). 

*How to improve?*

- **Fine-tuning the model**, to replace the need for lengthy instructions / examples.
- **Filtering context input**, like pruning [RAG](https://www.promptingguide.ai/research/rag) results, cleaning HTML, etc.
- **Maximize shared prompt prefix**, by putting dynamic portions (e.g. RAG results, history, etc) later in the prompt. This makes your request more [KV cache](https://medium.com/@joaolages/kv-caching-explained-276520203249)-friendly (which most LLM providers use) and means fewer input tokens are processed on each request. ([why?](https://lilianweng.github.io/posts/2023-01-10-inference-optimization/))

### Request Quantity

Each time you make a request you incur some round-trip latency – this can start to add up.
*How to improve?*
instead of firing off one request per step consider putting them in a single prompt and getting them all in a single response.

An approach to doing this is by collecting your steps in an enumerated list in the combined prompt, and then requesting the model to return the results in named fields in a JSON or some other data structure

### Parallelization

If an LLM can perform a sequence of steps in a non-sequential manner, splitting those steps into parallel calls will, obviously, improve latency.

If the steps are *strictly* sequential, it is still possible to leverage **speculative execution**. This is particularly effective for classification steps where one outcome is more likely than the others (e.g. moderation).

*How to improve?*

1. Start step 1 & step 2 simultaneously (e.g. input moderation & story generation)
2. Verify the result of step 1
3. If result was not the expected, cancel step 2 (and retry if necessary)

### Other Techniques

- **Streaming**: sending parts of data as soon as they're available instead of responding with the full output (`Promise() vs Promise.all()`)
- **Chunking**: closely related to *streaming*, chunking is the process of breaking down a large data set or input request into smaller pieces/chunks. This is useful when the output needs further processing before being shown to the user (moderation, translation)

