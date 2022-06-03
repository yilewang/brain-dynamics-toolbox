
The first mission is to make a dynamical system. To make a dynamical system, we need to know the evolution equations. They describe changes. A set of dynamical variables change in accordance with the underlying properties of the system (they characterize).

An esay example of the dynamical system is the "second law of mechanics" from Newton, which describe the acceleration of an object. 

**v(t) is the velocity**
$$ {d \mathbf v(t) \over dt} = {\mathbf F \over m} $$ 

**x(t) is the position info**
$$ {d \mathbf x(t) \over dt} = {\mathbf v(t)} $$ 

left side is **the rate of change of a variable**, but the right side is **the changes to the properties of the system**.

The explicit solution of the $\mathbf x(t)$ is

We know that the first derivative of the $\mathbf x(t)$ is velocity ($\mathbf v(t)$), and the second derivative of the $\mathbf x(t)$ is acceleration ($\mathbf a$).
$${d^2 \mathbf x(t) \over d^2 t} = {\mathbf F \over m}$$

Based on the acceleration, if we want to know the velocity, we can take the first derivative

$${d \mathbf x(t) \over dt} = {\mathbf F \over m} t + constant $$

The function of the velocity will be
$$\mathbf v(t) = {\mathbf F \over m} t + \mathbf v(0)$$

Then we can calculate the $\mathbf x(t)$ based on the $\mathbf v(t)$

$$\mathbf x(t) = {\mathbf F \over 2m} t^2 + \mathbf v(0)t + \mathbf x(0) $$

