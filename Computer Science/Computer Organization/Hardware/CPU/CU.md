The CU is responsible for the operation of the [[CPU]], as in, the retrieval of instructions from [[Computer Hardware|primary memory]], the execution sequence

#todo more on that

The CU contains various **register**, smaller storage locations that can hold data. If a computer is *64 [[Bits|bit]]*, then CU contains *64 bit* **registers** 

> [!Info] The Basic Registers
> - The [[MAR]]
> - The [[MDR]]

> [!Tip] Reading from [[SRAM|cache]]
> When the CU needs to read from the [[DRAM|main memory]], it first checks if a copy of the data exists in the [[SRAM|cache]]
> 
> When the processor needs to write to the [[DRAM|main memory]], it does so through [[SRAM|cache memory]]
> ![[Pasted image 20240424193359.png]]

