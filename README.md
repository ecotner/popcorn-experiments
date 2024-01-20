# Popcorn Experiments

Have you ever wondered how to make the perfect popcorn?
Should you use the microwave stuff?
Or pop it on the stove?
What factors of the cooking process make it turn out better/worse?
Which brands are the best?
If the kernels are past their expiration or sell-by date, are they still good?
What are the tradeoffs involved in calories consumed, energy used, time spent cooking, cost, quality, etc?

I aim to answer these questions and more, using rigorous experimentation and statistical inference techniques.

## Popcorn science background

From my literature search, I have found many different factors that could potentially influence popcorn quality.
I will divide some of these factors into kernel characteristics and cooking techniques.

Kernel characteristics:
* interior moisture: when heated, the moisture inside the kernel expands, and when the pressure becomes too great, it ruptures the shell and "pops". Apparently, the optimal moisture content for popping is 13-14% (by weight). Too much moisture and the pop occurs prematurely, and too little causes the kernel to pop too late or not all, both of which lead to disappointing kernel expansion.
* shell (aka _pericarp_) hardness/thickness: the shell needs to be durable enough to allow interior pressure to build up before popping, but not so durable that the expansion is suppressed when it does pop, or it pops too late or not at all. If the shell is too weak, not much pressure it built up and the pop does not 
* kernel dimensions (aka _grain caliber_): though not directly related to popping expansion, kernel length is correlated with shell thickness, which has an impact on popping expansion
* heat transfer properties: faster diffusion of heat throughout the kernel allows for more uniform buildup of pressure as moisture expands

Cooking techniques:
* Use of oil: coating the kernel in hot oil allows a more uniform distribution of heat around the outside of the kernel than heating the kernel from direct contact with a pot/pan, which tends to heat one side of the kernel more than the other.
* Temperature profile: A quick/slow ramp of external temperature can have a corresponding effect on the interior temperature of the kernel, which affects internal pressure as the moisture expands. The magnitude of the temperature plays a role too; higher temperatures will lead to higher pressures and faster cooking times.
* Agitation: can further reduce the asymmetry of heat transfer by repositioning the kernels over time.
* Hydration: you could potentially influence the internal moisture of the kernels beyond their natural state by baking them at a low temperature or soaking them in water.
* Steam retention (i.e. lid usage): cooking the kernels in an enclosed system can promote more uniform heating (as any steam produced can heat kernels from above), but also can result in less crispy popcorn, as the popped material can reabsorb the moisture and become soggy.
* Microwave: completely changes the cooking process! Kernels are heated from the inside out, and temperature profile likely depends on additional factors that would impact microwave absorption such as quantity of kernels being heated, their moisture content, placement geometry, microwave frequency/intensity, etc.

As a consumer, the kernel properties cannot be directly influenced except by choice of the brand of popcorn you purchase.
Many of the cooking techniques are under your direct control though; you choose whether to use a stove top, microwave, or air fryer, whether to use oil or not (and if so, what kind), temperature/power settings, etc.

Furthermore, there are also multiple different metrics of popcorn quality we can investigate:
* Popping expansion: the volume of finished product (popped kernels) divided by the mass/volume of the original kernels.
    * Literature seems to prefer ratio of popped volume to original mass, so the units are important.
* Unpopped fraction: the mass or volume ratio of inedible, unpopped kernels (after cooking) to original kernels. The inverse of this is known as the "percentage of explosion", and apparently 98% is the minimum acceptable level in industry.
    * A separate but related measure is the ratio of partially-popped kernels that have exploded but still have some hard bits that are unpleasant to bite down on.
* Burn severity: whether the popped kernels are noticibly burned or not, how severe those burns are, and the fraction of kernels that are effected.
* Crunchiness: is the popcorn soggy/chewy after popping, or is it nice and crunchy/crispy? This is probably a more qualitative factor, but I'll try and gauge it nonetheless.

References:
* [_Characteristics of a quality popcorn and how to store it correctly_](https://www.springhausagro.com/post/popcorn); mirianrivas; Springhaus; 2020-11-24
* [_Better popping potential for popcorn_](https://www.agronomy.org/news/science-news/better-popping-potential-popcorn/); Emily Matzke; American Society of Agronomy; 2021-05-31
* [_Influence of agronomic and kernel-related properties on popping expansion in popcorn_](https://acsess.onlinelibrary.wiley.com/doi/10.1002/agj2.20645); Saito et. al.; Agronomy Journal; DOI: 10.1002/agj2.20645; 2021-03-07

## Experiment 1: factorial analysis of stove-top cooking techniques
Investigating multiple independent factors of the cooking process so see which ones are the most impactful on popcorn quality.
Experiment is still in progress.
See [notebook](./experiments/exp001/untitled.ipynb) for details.

## Future experiment ideas:

* How does age of kernel impact moisture content and popcorn quality, and can it be influenced?
* Compare microwave brands?