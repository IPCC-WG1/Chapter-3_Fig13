PRECIPITATION - MODEL BIAS
==========================
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6778032.svg)](https://doi.org/10.5281/zenodo.6778032)

Figure number: 3.13
From the IPCC Working Group I Contribution to the Sixth Assessment Report: Chapter 3

![Figure 3.13](ar6_wg1_chap3_figure3_13_precip_model_bias.png?raw=true)


Description:
------------
Annual-mean precipitation rate (mm day–1) for the period 1995–2014. (a) Multi-
model (ensemble) mean constructed with one realization of the CMIP6 historical 
experiments from each model. (b) Multi- model mean bias, defined as the 
difference between the CMIP6 multi-model mean and precipitation analyses from
the Global Precipitation Climatology Project (GPCP) version 2.3 (Adler et al., 
2003). (c) Multi-model mean of the root mean square error calculated over all 
months separately and averaged with respect to the precipitation analyses from 
GPCP v2.3. (d) Multi-model-mean bias, calculated as the difference between the 
CMIP6 multi-model mean and the precipitation analyses from GPCP v2.3. Also shown
is the multi-model mean bias as the difference between the multi-model mean of 
(e) high resolution and (f) low resolution simulations of four HighResMIP models 
and the precipitation analyses from GPCP v2.3. Uncertainty is represented using 
the advanced approach: No overlay indicates regions with robust signal, where 
≥66% of models show change greater than variability threshold and ≥80% of all 
models agree on sign of change; diagonal lines indicate regions with no change 
or no robust signal, where <66% of models show a change greater than the 
variability threshold; crossed lines indicate regions with conflicting signal, 
where ≥66% of models show change greater than variability threshold and <80% of
all models agree on sign of change. For more information on the advanced 
approach, please refer to the Cross-Chapter Box Atlas.1. Stippling in panel e) 
marks areas where the bias in high resolution versions of the HighResMIP models 
is lower in at least 3 out of 4 models than in the corresponding low resolution 
versions.


Author list:
------------
- Bock, L.: DLR, Germany; lisa.bock@dlr.de
- Barreiro, M.: Universidad de la República, Uruguay
- Eyring, V.: DLR., Germany


Publication sources:
--------------------
Bock, L., Lauer, A., Schlund, M., Barreiro, M., Bellouin, N., Jones, C., Predoi, V., Meehl, G., Roberts, M., and Eyring, V.: Quantifying progress across different CMIP phases with the ESMValTool, Journal of Geophysical Research: Atmospheres, 125, e2019JD032321. https://doi.org/10.1029/2019JD032321


ESMValTool Branch:
------------------
- ESMValTool-AR6-OriginalCode-FinalFigures: [ar6_chapter_3](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/tree/ar6_chapter_3)


ESMValCore Branch:
------------------
- ESMValCore-AR6-OriginalCode-FinalFigures: [fix_cmip6_models_newcore](https://github.com/ipcc-wgi/ESMValCore-AR6-OriginalCode-FinalFigures/tree/fix_cmip6_models_newcore)


Recipe & diagnostics:
---------------------
Recipes used: 
- [recipes/ipccwg1ar6ch3/recipe_ipccwg1ar6ch3_atmosphere.yml](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/ar6_chapter_3/esmvaltool/recipes/ipccwg1ar6ch3/recipe_ipccwg1ar6ch3_atmosphere.yml)
- [recipes/ipccwg1ar6ch3/recipe_ipccwg1ar6ch3_highres.yml
](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/ar6_chapter_3/esmvaltool/recipes/ipccwg1ar6ch3/recipe_ipccwg1ar6ch3_highres.yml)

Diagnostics used: 
- [diag_scripts/ipcc_ar5/ch12_calc_IAV_for_stippandhatch.ncl](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/ar6_chapter_3/esmvaltool/diag_scripts/ipcc_ar5/ch12_calc_IAV_for_stippandhatch.ncl) 
- [diag_scripts/ipcc_ar6/model_bias.ncl](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/ar6_chapter_3/esmvaltool/diag_scripts/ipcc_ar6/model_bias.ncl)
- [diag_scripts/ipcc_ar6/model_bias_diff.ncl](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/ar6_chapter_3/esmvaltool/diag_scripts/ipcc_ar6/model_bias_diff.ncl)


Expected image path:
--------------------
- recipe_ipccwg1ar6ch3_atmosphere_YYYYMMDD_HHMMSS/plots/fig_3_13_cmip5/fig_3_13/model_bias_pr_annualclim_CMIP5.eps  
- recipe_ipccwg1ar6ch3_atmosphere_YYYYMMDD_HHMMSS/plots/fig_3_13_cmip6/fig_3_13/model_bias_pr_annualclim_CMIP6.eps


Software description:
---------------------
- ESMValTool environment file: [IPCC_environments/ar6_newcore_lisa_conda_environment.yml](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/main/IPCC_environments/ar6_newcore_lisa_conda_environment.yml)
- pip file: [IPCC_environments/ar6_newcore_lisa_pip_environment.txt](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/main/IPCC_environments/ar6_newcore_lisa_pip_environment.txt)


Hardware description:
---------------------
Machine used: Mistral
