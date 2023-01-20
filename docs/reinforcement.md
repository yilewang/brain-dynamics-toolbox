# Reinforcement Learning
  
`Date` 11/19/2023  
`Author` Yile Wang  

This markdown is a class note for basic concepts about the reinforcement learning. All the mathematical proofs could be found from Dr. Golden's book: **Statistical Machine Learning**.

First thing first, let's start from supervised machine learning:

## Supervised Machine Learning
let's assume $\vec{S}$ represents $P_e(\vec{S})$. $P_e$ is the statistical environment that generate $\vec{S}$. We called it the **Data Generation Process**. 

Then, let's say, $\bar{y}(\vec{S})$ is defined as function of $\vec{S}$.

Let's add some Gaussian noise to the function. $\eta(o, \sigma^2)$

$\tilde{y_i} = \bar{y_e}(\vec{S_i}) + n_i$

The training data $(\vec{S_i}, \vec{y_i})$ is the realization of the random variable
$(\underset{\sim}{\vec{S_i}}, \underset{\sim}{\vec{y_i}})$ 

The learning machine Model distribution is $P_m(\vec{S})$, thus, the probability of the $y_i$ could be written as

$$P(y_i | \vec{S_i}, \vec{\theta}) = \frac{e^{-(y_i-\ddot{y}(\vec{S_i}, \vec{\theta}))^2}2\sigma^2_m} {\sigma_m \sqrt{2}\pi }$$

Then, we can use maximum likelihood esitmation to do gradient descent.

$$P(\vec{S_i}, \vec{y_i}|\vec{\theta}) = P_m(\vec{S_i}) P(y_i | \vec{S_i}, \theta)$$

The loss function of it is: 

$$\mathcal{L}_n(\vec{\theta}) = - \frac{1}{n}log \underset{i=1}{\stackrel{n}{\Pi}}P(\vec{S_i}, \vec{y_i}|\vec{\theta})  $$

it could be written in this way:

$$\mathcal{L}_n(\vec{\theta}) = -\frac{1}{n} \underset{i=1}{\stackrel{n}{\sum}} log P(\vec{S_i}, \vec{y_i}|\vec{\theta})$$


## Policy Gradient Reinforcement Learning
