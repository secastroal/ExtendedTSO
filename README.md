# ME-TSO
## Description
This repository contains the code developed to do the empirical analyses of the paper "Mixed-Effects Trait-State-Occasion Model: Studying the Psychometric Properties and the Person-Situation Interactions of Psychological Dynamics". The mixed-effects trait-state-occasion model (ME-TSO) is an extension of the multilevel TSO model ([Castro-Alvarez et al., 2021](https://psyarxiv.com/gvhk6/); [Eid et al., 2017](https://doi.org/10.1027/1015-5759/a000435)) that allows studying the person-situation interaction effects as in the latent state-trait models for the combination of random and fixed situations ([Geiser et al., 2015](https://doi.org/10.1037/met0000026)). Furthermore, the ME-TSO model is encompassed within the dynamic structural equation modeling framework (DSEM; [Asparouhov et al. 2018](https://doi.org/10.1080/10705511.2017.1406803)).
## Folders and Files Description
- **Main.R**: Contains the code used to prepare the data, to extract the results from the Mplus output files, and to create the tables and figures included in the paper.
- **tso_cluster.R**: Contains the code to run the analyses in Mplus within R in parallel on a cluster computer.
- **METSO.sh**: Is a batch file used to run the analyses on a cluster computer.
- **Figures**: PDF Figures created in R.
- **Mplus**
    - *Syntaxes*: Mplus input files of the models fitted for the empirical example.
    - *ResultsFullSample*: Mplus output files of the analyses with the complete sample (644 individuals). These results were reported in the article.
    - *ResultsStationarySample*: Mplus output files of the analyses with the stationary sample (451 individuals). Tables with the unstandardized residuals of these analyses were reported in the supplementary material.
- **R**: Personalized functions created for these analyses.
    - *esmfunctions.R*: Set of four functions useful to manipulate intensive longitudinal data. These functions will be included in the `esmpack` in a future release.
    - *metso.var.coeff.R*: Function to compute the variance coefficients (both across fixed situations and wihtin fixed situations) of the ME-TSO when there are no additional time-invariant covariates in the model. 
- **Tables**: Text files with the tables in LaTeX format, which were created with the `xtable` package.

## Note
We are not authorized to share the data used for the empirical example. Nonetheless, data can be requested to the [Hoegekisnl team](https://www.hoegekis.nl/welkom).
