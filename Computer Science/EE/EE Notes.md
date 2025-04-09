### Colour Normalization
$$
Y \leftarrow 0.299 \cdot R + 0.587 \cdot G + 0.114 \cdot B \tag{1}
$$

### Convolution

$$
f*h=\sum_{k}\sum_{l}f(k,l)h(-k,-l) \tag{1}
$$

### Gradient Computation


Central difference
$$
F_{y}[x_{m},y_{n}] = \frac{ \partial I[x_{m},y_{n}] }{ \partial x } \approx |\ I(x_{m}-1,y_{n})-I(x_{m}+1,y_{n})\ | \tag{2}
$$
$$
F_{x}[x_{m},y_{n}] = \frac{ \partial I[x_{m},y_{n}] }{ \partial x } \approx |\ I(x_{m},y_{n}+1)-I(x_{m},y_{n}-1)\ | \tag{3}
$$


$$
| G[x_{m},y_{n}] | = \sqrt{ F_{y}[x_{m},y_{n}]^2+F_{y}[x_{m},y_{n}]^2 }
$$
$$
\theta = \arctan \left( \frac{F_{y}[x_{m},y_{n}]}{F_{x}[x_{m},y_{n}]} \right) \tag{4}
$$

<br>

$$x_{m} \notin [0,X] \quad \text{and} \quad y_{m}\not\in [0,Y] \tag{5}$$


Forward Difference
$$
F_{x}[x_{m},0] =  | I(x_{m},1)-I(x_{m},0) | \tag{6}
$$
$$
F_{y}[0,y_{n}] =  | I(1,y_{n})-I(0,y_{n}) | \tag{7}
$$
Backward Difference
$$
F_{x}[x_{m},Y] =  | I(x_{m},Y)-I(x_{m},Y-1) | \tag{8}
$$
$$
F_{y}[X,y_{n}] =  | I(X,y_{n})-I(X-1,y_{n}) | \tag{9}
$$

<br>




$j$ is a bin's index value
$$
j = \left\lfloor  \left( \frac{\theta \omega}{180\degree} \right) - \frac{1}{2}  \right\rfloor \tag{10}
$$

### Local Spatial Group Vector
$$f_{b} = \{ b_{i} \ |\ i=1,2,\dots,\alpha \cdot\beta \}$$


### Final Feature Vector Size

Sliding Window - $\Lambda, \Phi$, Slide Step - $\lambda, \phi$
Cells per Block - $\alpha,\beta$, Block Stride - $\delta, \gamma$
Pixels per Cell - $\zeta,\eta$, Orientation Bin Amount - $\omega$

when $\alpha \ne \beta$
$$
L \in \mathbb{R}^{d}
$$

$$
\begin{align}
d &= \left\lfloor \frac{\frac{\Lambda}{\zeta}-2\cdot\frac{\alpha}{2}+1}{\delta} \right\rfloor\left\lfloor \frac{\frac{\Phi}{\eta}-2\cdot\frac{\beta}{2}+1}{\gamma} \right\rfloor\cdot\alpha\beta\omega \\ &= \left\lfloor  \frac{\Lambda-\alpha\zeta+\zeta}{\delta\zeta}  \right\rfloor \left\lfloor   \frac{\Phi -\beta\eta+\eta}{\gamma\eta} \right\rfloor \alpha\beta\omega
\end{align}
$$


$$
\left[ \frac{\alpha}{2}; \frac{\Lambda}{\zeta} - \frac{\alpha}{2}\right]
$$



Once a histogram of $n$ bins has been computed for each of the block of varying density a feature vector is and the values of each histogram are normalized (in the original paper, L2 Norm is used)

Let $P$ be the penalty term

Then the apply the penalty term to an OLS regularization

$$
\sum_{i=1}^{n} \left( Y_{i}-\sum_{j=1}^{p} X_{ij}\beta_{ij} \right)^{2} + P
$$

in L1

$$
P = \lambda \sum_{j=1}^{p} |\beta_{j}|
$$

in L2
$$
P = \lambda \sum_{j=1}^{p} \beta_{j}^{2}
$$

$$
\zeta
\eta

$$

### Overlap
$$
a_{0} = \frac{\mathrm{area}(BB_{dt} \cap BB_{gt})}{area(BB_{dt}\cup)BB_{gt}} > 0.5 \tag{12}
$$

$$
D=\{ (x_{1},y_{1}),\dots,(x_{n},y_{n}) \}
$$

### Images to large
![[Pasted image 20241013161038.png]]

### Training Samples
![[Pasted image 20241013170610.png]]

### Testing samples
![[Pasted image 20241013170704.png]]

Total model count: 864

models like logistic regression do not support high dimensionality data. in our case dimensions can exceed 6000, therefore SVM

advantages vs disadvantages

![[Pasted image 20241016141551.png]]
The number of features in an SVM can help find a hyperplane of n-1 feature dimensionality to better separate the data points
![[Pasted image 20241016143818.png]]
The smaller dimensional space is converted to the larger dimensional space using a kernel

Kernel function generally transforms the training set of data so that a non-linear decision surface can be transformed to a linear equation in a higher number dimensional space

a linear kernel is defined as follows
$$
K(x_{1},x_{2})=x_{1}^\intercal x_{2}
$$
### SVM example using 2 dimensional data

the weight, $w$ or parameter of the hyperplane which separates the data points in 2D data space directly correlates to the gradient and intercept of the hyperplane (in this case $mx+c$) such that $w=(m,c)$

in matrix multiplication, the column width of one matrix should equal the row width of the other matrix. notice that in a 2D space  $w^\intercal = \begin{bmatrix}m  \\c\end{bmatrix}$ and $\text{point}=\begin{bmatrix}x,y\end{bmatrix}$

if for example $w^\intercal = \begin{bmatrix}-1 \\ 0\end{bmatrix}$ and $\text{point}=\begin{bmatrix}-3& 0\end{bmatrix}$
then 
$w^\intercal\text{point} = 3$

![[Pasted image 20241016145121.png]]

For all points on one side of the hyperplane the $w^\intercal\text{point}$ will be positive, on for all points on the other side it will be negative (the output of the multiplication is the label which is assigned)

keep in mind that multiplying each point with the weight and adding the bias creates the "vector"

this is how an SVM performs binary classification 

A shift in a hyperplane that does not pass through the origin is called a bias
![[Pasted image 20241016145820.png]]

The problem of the SVM model is to identify which hyperplane maximizes the margin space between the support vectors of each binary class

![[Pasted image 20241016150929.png]]

in the image above, the margin space is identified with $x_{1}-x_{2}$

maximise $\frac{2}{\lvert w \rvert}$ such that ![[Pasted image 20241016151233.png]]

note that maximising the value of $\frac{2}{\lvert w \rvert}$ is the same as minimising the value of $\frac{\lvert w \rvert}{2}$ (minimising is easier than maximising in machine learning?)

because outliers exists, you risk overfitting when optimising the hyperplane??

![[Pasted image 20241016151830.png]]

### Loss
loss is a function which measures how far an estimated values is from its true value
$$
\text{square error loss} = \frac{1}{n}\sum_{i=1}^{n} (Y_{i}-\hat{Y_{i}})^{2}
$$

to maximise the margin distance, *hinge loss* is used?
![[Pasted image 20241016161211.png]]
(classification boundary is the hyperplane)

remember that 
$$
\hat{Y_{i}} = \begin{equation}
\begin{cases}
-1, \quad w^\intercal x_{i} + b \le -1\\
1, \quad w^\intercal x_{i} + b \ge 1
\end{cases}
\end{equation}
$$
$$
L = \max(0,1-Y_{i}(w^\intercal x_{i}+b))
$$
if $L=0$, the classification is correct, if not, it is incorrect
![[Pasted image 20241016165051.png]]

the more a prediction is incorrect, the higher the hinge loss. Notice however that even correct predictions are penalized if they do not satisfy the boundary

### Gradient Descent

![[Pasted image 20241016174423.png]]

the cost function is the average of all the loss function for all the data points which are present

since the loss function approaches 0, the more accurate the predictions are, the minimum of the cost function will give the optimal weight for which the majority of of outputs from the loss function are closest to 0
![[Pasted image 20241016174801.png]]
![[Pasted image 20241016175135.png]]

gradient descent is an optimization algorithm used for minimizing the cost function in various machine learning algorithms. it is used for updating the parameters of the learning model

$$
\begin{align}
w_{2}=w_{1}-L\cdot \frac{ \partial J }{ \partial w }   \\
b_{2}=b_{1}-L\frac{ \partial J }{ \partial b } 
\end{align}
$$
$L$ here is the learning rate. it is simply the amount of change u give to weight or bias

![[Pasted image 20241016180454.png]]

$\lambda$ is the regularisation paramater


### Now from MIT

https://www.youtube.com/watch?v=_PwhiWxHK8o

![[Pasted image 20241016181527.png]]

in the image above, $\bar{u}$ is an unknown sample

if youre a positive sample, then the decision function should give $\ge {1}$, if youre a negative sample $\le -1$

$y_{i}$ is $\ge 1$ for positive samples and $\le -1$ for negative samples

$$
\begin{equation}
\begin{cases} 
y_{i}(w^\top x_{i}+b)\ge 0 \quad \\
\min_{i}|w^\top x_{i}+b| = 1 \quad 
\end{cases}
\quad
\Leftrightarrow
\quad
y_{i}(w^\top x_{i}+b)\ge 1
\end{equation}
$$


### Random Examples
$$
	\left( \frac{b_{w}}{2}, \frac{b_{h}}{2} \right) = \left( \frac{4}{2}, \frac{4}{2} \right)
	$$
	
	$$
	\left( \left( \frac{W_{w}}{c_{w}}-\frac{b_{w}}{2} \right), \left( \frac{W_{h}}{c_{h}}-\frac{b_{h}}{2} \right) \right) = \left( \left( \frac{64}{8} -\frac{4}{2}\right), \left( \frac{128}{8}-\frac{4}{2} \right) \right) = (6,14)
	$$

$$
\begin{align}
N &= |(W_h, W_w)| \times |\{\omega\}| \times |(c_w, c_h)| \times \sum_{\substack{b_w \geq s_w \\ b_h \geq s_h}} |(b_w, b_h)| \times |(s_w, s_h)| \times 2 \\
&= 4 \times 3 \times 4 \times 9 \times 3 =864
\end{align}

$$



### Best with HDM vs Best with no hdm
mcnemar: 0.004549551708841035 
bw bwo ww wwo
[0.83314207 0.91651759 0.90849673 0.02802624 0.97029409 0.97203796]
[0.78278778 0.89102564 0.87883308 0.03428742 0.95456293 0.95259332]
[0.63971306 0.80575432 0.81935394 0.16487776 0.9352923  0.93493455]
[0.62185623 0.81217977 0.79540743 0.09149466 0.89573911 0.87901402]

128x96 vs 100x50: 0.01
128x96 vs 112x48: 0.004

total pixels_per_cell:
{(4, 4): np.float64(0.7367819785566146), (6, 6): np.float64(0.7482676284415525), (8, 8): np.float64(0.753592813613876), (10, 10): np.float64(0.7274793886785962)}

PnPLO pixels_per_cell:
{(4, 4): np.float64(0.5709806735179347), (6, 6): np.float64(0.6093343663523442), (8, 8): np.float64(0.6319509703166148), (10, 10): np.float64(0.6205867959049844)}

Model 1: 9 bins, Model 2: 13 bins
pvalue      0.6756280479843453
statistic   280.0 

Model 1: 9 bins, Model 2: 18 bins
pvalue      0.0064010777268400515
statistic   176.0 

Model 1: 13 bins, Model 2: 18 bins
pvalue      0.051952814015705374
statistic   234.0 


### BEST HDM VS BEST CDM
6.047127736480351e-09

MCC scores:
0.8490664401120699
0.8396347686487944


CALTECH BLOCK SIZE (2,2) vs BLOCK SIZE (4,4)
p=0.7757387167068798

dimensions:
3780
54288


----
4,4
0.0005342777626994592
2,2
0.29117943099914795

---

Introduction - 277
Background - 1783
Methodology - 981
Experimental Results - 203
Data Analysis - 394
Limitations - 102
Conclusions - 251