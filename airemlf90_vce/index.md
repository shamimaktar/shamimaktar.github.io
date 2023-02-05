# Variance component estimation with AIREMLF90 for Single Trait Analysis


In the previous post, I tried to show how to solve MME to derive BLUP values with **assumed** variance components. We need to estimate actual variance components of the animals under study in practical application. Especially, if:


- we are interested in a new trait, from which no parameters are available
- variances and covariances might have changed over time
- considerable changes have occurred in a population e.g. due to recent
importations.


Here is a brief overview of the methods used in VCE. We use AI-REML method as default in BLUPF90. We can use EM-REML and Gibbs Sampling also, depending on individual use cases. A good explanation of which method to use, can be found here. https://doi.org/10.1111/j.1439-0388.2008.00774.x 



{{< figure src="/posts/airemlf90_vce/aireml.jpeg" title="Evolution of methods used for VCE" >}}



In this example, we use simulated data and corresponding pedigree file to estimate the variance components. The model contains animals as random effect, farm, sex, year as fixed effects, and a single trait (observation). The following video explains the process in detail.

{{< youtube YvXRJq6Tqq8 >}}


This exmpale has also been taken from Y. Masuda's awesome tutorial for BLUPF90 suite of programs. You can find the details here. https://masuday.github.io/blupf90_tutorial/vc_aireml.html 
