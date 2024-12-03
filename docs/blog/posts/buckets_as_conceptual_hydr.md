---
date:
  created: 2024-12-02
authors:
  - jmframe
---

# Buckets as a hydrologic conceptualization 

"Very clever, Sir Edmond, but it is buckets all the way down!"

## Sir Edmond Leakybucket

When I was first learning differential equations the professor told us a silly story about Sir Edmond LeakingBucket, some ol' timey English royal who had to drink his ale quickly because his ale bucket leaked. I went on to study hydrology, so I've had to think about Sir Edmond now for past fiteen years. I can't escape him. Sometimes he mixes two kinds of ales together, sometimes his ale bucket is more complicated or simpler, but he is always losing his ale. Poor guy. Sir Edmond and his bucket do two important things: 1) gives nice differential equation examples, but more importantly for hydrology 2) Leaking buckets are a primary conceptualization for hydrologic processes. 

## A walk through the watershed

Realizing that our computer models don't capture nearly anything that is really going on. Because of simplified equations, but also heterogeneity and complexity.

Going back again to undergraduate, I was building my first watershed model (Frame, 2010). I spend weeks staring at a computer screed, writing code, processing data, and thinking through discretization of Sir Edmond's ale bucket. I went out to do some field work for a different project in the Carmel River Watershed, a valley I've been to a dozen times. But after spending so much time thinking about this watershed digitally, a sense of dred came over me as I looked down from Carmel Valley Road (Figure x). I was realizing how much my precious computer model was missing. 

But in hydrology, we consider representing a delayed flow of water as a bucket a type of physical conceptualization. And as a matter of fact, this goes back a long way to Instantaneous Unit Hydrograph (IUH). In my MS level hydrology class, we learned that the IUH from linear reservoirs turns into a beta distribution (Nash 1960). This is a type of theoretical physical understanding of hydrology through buckets. This is similar to the use of harmonic oscillators in "real" physics. 

## Harmonic oscillators
The ultraviolate catastrophy is the result of using harmonic oscillators as conceptual representations of physical systems. Max Planck resolved the ultraviolet catastrophe in 1900 by fundamentally rethinking the energy distribution, quantizing the energy, allowing the thermodynamic limit to match experimental data, giving evidence that energy in the real world is quantum, rather than continuous. Let's take note of a few important pieces of this success story. In the classical case, the energy was poorly concieved. Physicists knew this because the theory, when taken to the thermodynamic limit, didn't match observation data. This led them to chance the conceptualization. 

Back now to hydrology. We've seen overwhelming evidence in the past few decades that neural networks are more accurate at predicting hydrologic responses than the conceptualization of hydrologic systems as buckets. Unless that conceptualization itself can be boosted by a neural network (Shen et al., 2024). What I've always pondered is what would happen if hydrologists acted a bit more like physicists, and rejected demonstratively predictive conceptualizations in favor of those that match observations. We still learn the Rayleigh–Jeans law in thermodynamics, but we then understand the limitations of the continuous energy conceptualization and turn to Planck's Law to grasp the quantum reality.

## Taking buckets to their limit

The actual physical representation of a mathematical structure of a system of buckets flowing into each other is the correct physical model of one type of system only, and that is, of course, a system of buckets flowing into each other. Applying this model to a watershed, for instance, is similar to using continuous energy waves in the form of harmonic oscillators to model black body radiation. Yes, it will do in some cases, but we know it is not how the real world behaves.

But let's take this idea of buckets flowing into each other a bit more seriously as a representation of hydrologic processes. When I am out on Carmel Valley Road overlooking the watershed, I see depressions, gullies, rills, blades of grass, everything else. All these individual processes do somewhat behave as oddly shaped buckets. A blad of grass, for instance, does collect moisture from the air, and that moisture does flow down the blade. A prarie pothole also fills up and overflows, bucket-like, yet some water flows down through the leaking bottom. Though these are not perfectly round reservoirs with known leaks with known coefficients, they do all sort of flow into each other. I used this idea to try to bring neural networks into hydrology from a more realistic conceptualization. With differentiable modeling, we can set up our neural network to behave like these systems of buckets, complete with valves on the spigots determining the flow coefficient (weights), and the water level dropping below the spigot shutting off flow completely (activation). What I think we are left with here is a pretty darn good digital interpretation of a messy, complex, heterogeneous system (Frame et al., 2024). Each individual bucket in our nash cascade neural network behaves like a mass concerving perceptron (Wang et al., 2024). In this scenario, we end up with a model that has the uncanney ability to match a downstream diagnostic variable very well, and we have utilized the hydrologists tool of choice.


## References
Acuña Espinoza, E., Loritz, R., Álvarez Chaves, M., Bäuerle, N., and Ehret, U.: To bucket or not to bucket? Analyzing the performance and interpretability of hybrid hydrological models with dynamic parameterization, Hydrol. Earth Syst. Sci., 28, 2705–2719, https://doi.org/10.5194/hess-28-2705-2024, 2024. 

Frame, J. M. (2010). An integrated surface water-groundwater interaction model for the Carmel River.

Frame J. M., L. Hernandez Rodriguez, and M. Bassiouni (2023). "DeepBucketLab - A Playground for Understanding Deep Learning for Hydrologic Process Representations," DOI: 10.5072/zenodo.7349

Frame J. M., Bindas T., Araki R., Rapp J. and Deardorff E. (2024) Synchronization in hydrologic  processes and modeling the response with concepts, physics and neural networks. ESS Open Archive. DOI: 10.22541/essoar.171320241.14125931/v1

Nash, J. E., & HRS. (1960). A unit hydrograph study, with particular reference to British catchments. Proceedings of the Institution of Civil Engineers, 17(3), 249-282.

Shen, C., Appling, A. P., Gentine, P., Bandai, T., Gupta, H., Tartakovsky, A., ... & Lawson, K. (2023). Differentiable modelling to unify machine learning and physical models for geosciences. Nature Reviews Earth & Environment, 4(8), 552-567.

Wang, Y. H., & Gupta, H. V. (2024). Towards interpretable physical‐conceptual catchment‐scale hydrological modeling using the mass‐conserving‐perceptron. Water Resources Research, 60(10), e2024WR037224.

<!-- more -->

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua.
