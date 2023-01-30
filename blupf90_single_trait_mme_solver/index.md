# Single Trait Analysis with known/assumed variance components using BLUPF90+


Estimation of breeding values is at the core of Animal Breeding for genetic improvement of livestock. The BLUP methodology solving MME bt Henderson is standard in this regard. BLUPF90+ is a combination of programs with which we can solve MME for simultaneously getting BLUE and BLUP values of animals for trait/s. 

{{< figure src="/posts/blupf90_single_trait_mme_solver/blupf90+.png" title="BLUPF90+" >}}

In this example, we will try to solve the single trait (Pre weaning weight gain, WWG) with fixed effect (sex) and random effect (animal) from Chapter 3 data on animal model of Mrode(2014). Residual and genetic variances are assumed in this example. So, it is only concerned with solving MMEs with the BLUPF90 program. I will describe how to eastimate variance components in another video.

{{< figure src="/posts/blupf90_single_trait_mme_solver/Inkedblupf90.jpg" title="MME solver (BLUEs & BLUPs)" >}}

The following video contains the necessary instructions for estimating BLUEs for fixed effects and predicting BLUPs for animals.

{{< youtube IiIV4j2yD-I >}}


This exmpale has been taken from Y. Masuda's awesome tutorial for BLUPF90 suite of programs. You can find the details here. https://masuday.github.io/blupf90_tutorial/mrode_c03ex031_animal_model.html 
