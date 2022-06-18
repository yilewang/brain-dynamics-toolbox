### Introduction of Deep Learning

Here is my study note of the deep learning. All the equations are credited by Andrew Ng's deep learning course: Neural Net and Deep Learning


### Course1 Week2 L03

#### The Sigmoid function

The general Sigmoid function applied in Logistic Regression is:
$$ \hat{y} = \sigma(W^{T} x + b) $$

where:
$$ \sigma(z) = \frac{1}{1+e^{(-z)}}$$
Based on the formula above, we can try to calculate the binary probability of the classification. 


#### The loss function of the Logistic Regression

In Neural Net, the loss function cannot be expressed as simple function

$$L_\varepsilon\bigl(\hat{y},y\bigr) = \frac{1}{2}(\hat{y} - y)^2$$

Instead, it should be describe as the following equation

$$L_\varepsilon\bigl(\hat{y},y\bigr)= -(y\log{\hat{y}} + (1-y)\log{\bigl(1-\hat{y}\bigr)})$$

In the loss function above, if y=1, 
$$L_\varepsilon\bigl(\hat{y},y\bigr) = -\log{\hat{y}}$$

and if we want $\log{\hat{y}}$ larger, 
the $\hat{y}$ should be as large as possible.

If y=0,
$$L_\varepsilon\bigl(\hat{y},y\bigr) = -\log{\bigl(1-\hat{y}}\bigr)$$

we want $\log{\bigl(1-\hat{y}}\bigr)$ to be large, 
so the $\hat{y}$ should be as small as possible.

The final cost function would be:


$$J(w,b)= \frac{1}{m} \sum_{i=1}^{m} L_\varepsilon\bigl(\hat{y}^{i} , y^{i}\bigr)$$

and after subtitution:

$$-\frac{1}{m} \sum^{m}_{i=1}[(y\log{\hat{y}} + (1-y)\log{\bigl(1-\hat{y}\bigr)})]$$

The ultimate goal is to find out the ${W}$ 
and ${B}$ 
that give us the minimum cost function ${J}$
