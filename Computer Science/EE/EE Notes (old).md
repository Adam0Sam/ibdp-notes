$$\mathrm{LBP}_{P,R}=\sum^{P-1}_{p=0}s(g_{p}-g_{c})2^p, \quad \text{where } \ s(x)= \begin{equation}\begin{cases}1, \ \ \text{if} \ x\ge 0 \\ 0,\ \ \text{otherwise} \end{cases} \end{equation}$$

$$\left( -R\sin\left( \frac{2\pi p}{P} \right), R\cos\left( \frac{2\pi p}{P} \right) \right)$$


$$\mathrm{LBP}^{riu 2}_{P,R}=\begin{equation}\begin{cases}\mathrm{LBP_{P,R}}\quad \text{if } \ U(\mathrm{LBP}_{P,R}) \le 2 \\ P+1\quad\quad\text{otherwise}\end{cases}\end{equation}$$
$$U(\mathrm{LBP}_{P,R}) = |s(g_{P-1}-g_{c}) - s(g_{0}-g_{c})| + \sum^{P-1}_{p=1}|s(g_{p}-g_{c})-s(g_{p-1}-g_{c})|$$

$$s'(x,g_{c}, t)=\begin{equation}
\begin{cases}
1, \quad\quad x  \ge g_{c} + t \\
0, \quad\quad  |x-g_{c}|<t \\
-1,\quad\ x\le g_{c}-t
\end{cases}
\end{equation}$$



---

*X. Tan and B. Triggs, "Enhanced Local Texture Feature Sets for Face Recognition Under Difficult Lighting Conditions," in IEEE Transactions on Image Processing, vol. 19, no. 6, pp. 1635-1650, June 2010*

*what to do with this?*
even though LBP features are completely invariant to monotonic global gray-level transformations, their performance degrades significantly under changes of lighting direction and shadowing

LBP features are known to be sensitive to noise in near-uniform image regions such as cheeks and foreheads. We introduce a generalization of LBP called local ternary patterns (LTPs) that is more discriminant and less sensitive to noise in uniform regions


**LBP extension**: The first defined LBPs for neighborhoods of different sizes, thus
making it feasible to deal with textures at different scales

**ULBP**: The second defined the so-called uniform patterns: an LBP is “uniform” if it contains at most one 0-1 and one 1-0 transition when viewed as a circular bit string. Uniformity is important because it characterizes the patches that contain primitive structural information such as edges and corners. 

Although only 58 of the 256 8-bit patterns are uniform, nearly 90% of all
observed image neighborhoods are uniform and many of the remaining ones contain essentially noise. Thus, when histogramming LBPs the number of bins can be reduced significantly by assigning all nonuniform patterns to a single bin, typically without losing too much information.

**LTP**: LBPs, because they threshold at exactly the value of the central pixel they tend to be sensitive to noise, particularly in near-uniform image regions, and to smooth weak illumination gradients