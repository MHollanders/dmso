# DMSO analysis

This repo houses the data and code for the analysis of the responses from two bacteria, *Pseudomonas aeruginosa* and *Streptococcus pneumoniae*, to dimethyl-sulfoxide (DMSO) with and without antibiotics. We fitted hormetic dose-response models (Cedergreen et al. 2005) with reversible jump MCMC (Green 1995) on the hormesis parameter using NIMBLE 0.12.2 (de Valpine et al. 2017) in R 4.2.0 (R Core Team 2022). We fit the models with weakly informative priors except for the rate parameter $\alpha$, which was fixed at 0.5 (Cedergreen et al. 2005). We fit species-by-treatment specific curves, with random correlated trial effects on each of the model parameters. Plots were produced using the `ggplot`, `ggdist`, and `patchwork`.


1. Cedergreen, N., Ritz, C., & Streibig, J. C. (2005). Improved empirical models describing hormesis. Environmental Toxicology and Chemistry, 24(12), 3166–3172. https://doi.org/10.1897/05-014R.1

2. de Valpine, P., Turek, D., Paciorek, C. J., Anderson-Bergman, C., Lang, D. T., & Bodik, R. (2017). Programming with models: Writing statistical algorithms for general model structures with NIMBLE. Journal of Computational and Graphical Statistics, 26(2), 403–413. https://doi.org/10.1080/10618600.2016.1172487

3. Green, P. J. (1995). Reversible Jump Markov Chain Monte Carlo computation and Bayesian model determination. Biometrika, 82(4), 711–732. https://doi.org/10.2307/2337340

4. Kay, M. (2021). ggdist: Visualizations of distributions and uncertainty, R package version 2.2.0. https://doi.org/10.5281/zenodo.3879620

5. Pedersen, T. L. (2020). patchwork: The composer of plots [Manual]. https://CRAN.R-project.org/package=patchwork

6. R Core Team. (2022). R: A language and environment for statistical computing. https://www.R-project.org/
Wickham, H. (2016). ggplot2: Elegant graphics for data analysis. Springer-Verlag New York. https://ggplot2.tidyverse.org


