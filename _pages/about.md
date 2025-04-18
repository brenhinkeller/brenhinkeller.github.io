---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

Despite the static appearance of Earth’s continental crust on human timescales, the composition and structure of the crust has changed markedly throughout Earth history. My group applies a wide range of integrated computational, field, and thermo/geochronological approaches to better understand the history of the solid Earth, particularly including the formation of the continental crust and its coevolution with the biosphere and the surface Earth system.

---
## Research group

| ------------------------- | ------------------------- | ------------------------- |
|<img width="256" src="images/profiles/jannitta_yao.jpg"><br>Jannitta Yao<br>Graduate Student|<img width="256" src="images/profiles/reina_harding.jpg"><br>Reina Harding<br>Graduate Student|<img width="256" src="images/profiles/alex_cox.jpg"><br>[Alexander Cox](https://earthsciences.dartmouth.edu/people/alexander-cox)<br>Graduate Student|
|<img width="256" src="images/profiles/ke_gao.jpg"><br>Ke Gao<br>Visiting Graduate Student|<img width="256" src="images/profiles/kalin_mcdannell.jpg"><br>[Kalin McDannell](https://www.kmcdannell.com/)<br>Postdoctoral Fellow|<img width="256" src="images/profiles/graham_edwards.jpg"><br>[Graham Edwards](https://grahamedwards.github.io/)<br>Postdoctoral Fellow|
{: style="font-size: 95%; text-align: center;"}

## Alumni

| ------------------------- | ------------------------- | ------------------------- |
|<img width="256" src="images/profiles/theo_green.jpg"><br>[Theodore Green](https://geosciences.princeton.edu/people/theodore-green)<br>Dartmouth Senior Fellow<br>Class of 2021|<img width="256" src="images/profiles/gailin_l_pease.jpg"><br>[Gailin Pease](https://earthsciences.dartmouth.edu/people/gailin-l-pease)<br>Master of Science<br>Class of 2021|<img width="256" src="images/profiles/akshay_mehra.jpg"><br>[Akshay Mehra](https://www.akshaymehra.com/)<br>Postdoctoral Fellow<br>2019-2022|
|<img width="256" src="images/profiles/blank.jpg">|<img width="256" src="images/profiles/blank.jpg">|<img width="256" src="images/profiles/blank.jpg">|
{: style="font-size: 95%; text-align: center;"}

---
## Resources

For mineral (especially zircon) eruption/deposition age estimation, there is a simple example in this [BayeZirChron demo notebook](https://mybinder.org/v2/gh/brenhinkeller/BayeZirChron.c/main?filepath=julia%2Fdemo.ipynb) based on [Keller, Schoene, & Samperton (2018)]( https://doi.org/10.7185/geochemlet.1826), or the [Chron.jl](https://github.com/brenhinkeller/Chron.jl) version of the same notebook:

* Standalone eruption/deposition age modelling
[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/brenhinkeller/Chron.jl/main?filepath=examples/EruptionDepositionAgeDemonstration.ipynb)

While originally developed for zircon eruption age estimation, an analagous approach is also applicable to plutonic settings (e.g., [Ratschbacher et al., 2018](https://doi.org/10.1093/petrology/egy079)), or to the problem of finding the distribution of the limits of a highly dispersed mineral crystallization (or closure) age spectrum more broadly.

Other [Chron.jl](https://github.com/brenhinkeller/Chron.jl) example notebooks demonstrate the integration of this eruption/deposition approach with age-depth modelling, or standalone age-depth models.

* Coupled eruption-age and age-depth modelling
[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/brenhinkeller/Chron.jl/main?filepath=examples/Chron1.0Coupled.ipynb)

* Age-depth modelling with simple Gaussian age constraints
[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/brenhinkeller/Chron.jl/main?filepath=examples/Chron1.0StratOnly.ipynb)

* Age-depth modelling with radiocarbon age constraints
[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/brenhinkeller/Chron.jl/main?filepath=examples/Chron1.0Radiocarbon.ipynb)


If you're interested in "statistical geochemistry", especially weighted bootstrap resampling of whole-rock geochemical data, try [StatGeochem.jl](https://github.com/brenhinkeller/StatGeochem.jl) (Julia), or else [StatisticalGeochemistry](https://github.com/brenhinkeller/StatisticalGeochemistry) (Matlab, no longer actively developed). A number of example usage notebooks are available in the StatGeochem.jl repo, including

* Weighted bootstrap resampling
[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/brenhinkeller/StatGeochem.jl/main?filepath=examples/BootstrapResamplingDemo.ipynb)

* Julia-alphaMELTS interface demo
[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/brenhinkeller/StatGeochem.jl/main?filepath=examples/MeltsExamples.ipynb)

* Julia-Perple_X interface demo
[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/brenhinkeller/StatGeochem.jl/main?filepath=examples/PerplexExamples.ipynb)

* Constant-silica reference crustal model (see [Keller & Harrison, 2020](https://www.pnas.org/content/117/35/21101))
[![Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/brenhinkeller/StatGeochem.jl/main?filepath=examples/ConstantSilicaReferenceModel.ipynb)

---

Over the past few years, I have transitioned most of my computational research from a C-and-Matlab two-language workflow (C for heavy lifting / parallel work, and Matlab everything else) to a pure [Julia](https://julialang.org/) workflow, using [MPI.jl](https://github.com/JuliaParallel/MPI.jl) for most parallel/HPC work, along with packages like [LoopVectoriztion.jl](https://github.com/chriselrod/LoopVectorization.jl) and [VectorizedRNG.jl](https://github.com/chriselrod/VectorizedRNG.jl) for SIMD performance. I have written up a few [notes](https://github.com/brenhinkeller/JuliaAdviceForMatlabProgrammers) of advice for anyone else who is interested in doing the same. The short version: efficient _multiple dispatch_ really does provide a solution to the "two-language problem", but the dispatch-centric programming paradigm can take quite a while to fully internalize; beware _type instability_.

---
<a rel="me" href="https://fosstodon.org/@brenhinkeller">Mastodon</a>
