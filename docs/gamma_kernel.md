### Gamma Kernel in TVB modeling

The formula is coming from _Linear Systems Analysis of Functional Magnetic Resonance Imaging in HUman V1_

The temporal impulse reponse with a gamma function:
$$
h(t) = \frac{(t/\tau)^{(n-1)}e^{-(t/\tau)}}{\tau (n-1)!}
$$

$t$ is time. Two free parameters: time constant, $\tau$, a phase delay determined by intege 
$n$.

Allowed for a pure delay, $\delta$ between stimulus onset and beginning of the fMRI response.


Contrast response functions:

$$
r(c) = \frac{ac^p}{c^p + \sigma}
$$

$c$ is contrast, 
$a$ is a scale factor, 
$p$ is exponent, and 
$\sigma$ is the contrast gain.

The stimulus-evoked fMRI response is the product of two functions, one that depends only on contrast and the other that depends only on time. 

#### An important conclusion
fMRI response is proportional to the average neural activity. If this model were correct, then three important consequences would follow. 
- First, stimulus contrast and stimulus time course would influence fMRI responses separably. 
- Second, the linear transform model would enable us to estimate the temporal fMRI impulse–response function. 
- Third, the linear transform model would enable us to infer the underlying (presumably neural) contrast–response functions from fMRI data.