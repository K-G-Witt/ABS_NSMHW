# ABS_NSMHW
## Australian Bureau of Statistics (ABS) National Survey of Mental Health and Wellbeing (NSMHW) Project
[![DOI](https://zenodo.org/badge/1071838645.svg)](https://doi.org/10.5281/zenodo.17290805)

This repository is licensed under the [MIT License](LICENSE).

If you use or build on this code, please cite it as:
* Initial release: Witt, KG. (2025). [ABS_NSMHW]. Zenodo. https://doi.org/10.5281/zenodo.17290805.


### Background:
The Australian Bureau of Statistics National Survey of Mental Health and Wellbeing (ABS_NSMHW) Project uses publicly available data from the ABS to answer the following key research questions:

1. What is the self-reported age of onset for suicidal ideation, self-harm, and attempted suicide by generation and is the self-reported age of onset getting younger?
2. What is the relationship between self-reported chronic pain and suicidal ideation, self-harm, and attempted suicide?

Suicide is the leading cause of death for Australians aged 18-44 years (ABS, 2024), and rates are increasing. Self-harm is even more prevalent. For every suicide death, 9 Australians are admitted to a hospital following self-harm, while 127 more Australians engage in self-harming behaviors in the community (Christensen et al., 2022). Suicidal ideation is even more common. For every suicide death between 2020-22, for example, the Australian Institute of Health and Welfare (AIHW) estimates that 344 Australians have reported seriously thinking about suicide at least once in their lifetime (AIHW 2023).

Adolescence and early adulthood have been identified as high-risk periods for the emergence of both suicidal ideation (Zagdańska et al., 2013) and self-harm (Gillies et al., 2018). A younger age of onset for suicidal ideation and self-harm has been associated with numerous pooerer outcomes in adulthood, including increased risks of experiencing mental health problems, chronic suicidal ideation (Fergusson et al., 2005), more frequent self-harm, greater severity of self-harm (Ammerman et al., 2018), and greater risks of early death, including by suicide (Olfson et al., 2018). The onset of suicidal ideation and self-harm has also been associated with experiencing chronic pain. Chronic pain, in turn, has also been associated with the onset of suicidal ideation and/or self-harm (Koenig et al., 2015).



### Analyses:
#### Self-reported age of onset for suicidal ideation, self-harm, and attempted suicide by generation.
1. Data for the two periods of data collection for the ABS NSMHW (i.e., Cohort 1, surveyed between December 2020-July 2021 and Cohort 2, surveyed between December 2021-October 2022) were combined.
   
2. Respondents were grouped according to generation:
   * Generation Z, aged 16-25 years
   * Millennials, aged 26-41 years
   * Generation X, aged 42-57 years
   * Baby Boomers, aged 58-76 years

3. Survival models (Cox's proportaional hazards model) were used to determine whether age of onset for suicidal ideation, self-harm, and/or attempted suicide differed by generation.

4. Generation-stratified survivial models (Cox's proportaional hazards model) were used to determine whether there were any risk factors that were differentially associated with self-reported age of onset for suicidal ideation, self-harm, and/or attempted suicide by generation.

Full analysis code is provided in this repo: [Suicide_populationchar_addCI_v2.html](https://github.com/K-G-Witt/ABS_NSMHW/blob/main/Code/Suicide_populationchar_addCI_v2.html), [Suicide_kmcurves.html](https://github.com/K-G-Witt/ABS_NSMHW/blob/main/Code/Suicide_kmcurves.html), [Suicide_weighted.html](https://github.com/K-G-Witt/ABS_NSMHW/blob/main/Code/Suicide_weighted.html).



### Data Sources:
The Australian Bureau of Statistics National Survey of Mental Health and Wellbeing (ABS_NSMHW) Project uses data from two waves of the 2020-2022 National Survey of Mental Health and Wellbeing:
* Cohort 1: surveyed between December 2020-July 2021
* Cohort 2: surveyed between December 2021-October 2022

Data for the [ABS NSMHW](https://www.abs.gov.au/statistics/health/mental-health/national-study-mental-health-and-wellbeing/latest-release) is publicly available from the ABS on request.



### Packages:
Analyses were undertaken in R for Windows. In addition to base R, the following packages were used:

* [missRanger](https://www.rdocumentation.org/packages/missRanger/versions/2.6.1/topics/missRanger)
* [survival](https://www.rdocumentation.org/packages/survival/versions/3.5-7)
* [survminer](https://www.rdocumentation.org/packages/survminer/versions/0.4.9)



### Publications:
The following publications have arisen from the ABS_NSMHW Project:

* Witt K., et al. (2025). Generational effects in self-reported age of onset for youth suicidal ideation, self-harm, and attempted suicide using data from the Australian National Study of Mental Health and Wellbeing, 2020-22. _SSRN Preprints_. DOI: [10.2139/ssrn.5262921](http://dx.doi.org/10.2139/ssrn.5262921).




### Additional References:
Ammerman BA., et al. (2018). The relationship between nonsuicidal self-injury age of onset and severity of self-harm. _Suicide Life Threat Behav_, 48(1): 31-7. DOI: [10.1111/sltb.12330](https://onlinelibrary.wiley.com/doi/10.1111/sltb.12330).

Australian Bureau of Statistics. (2024). _Causes of Death, Australia_. Canberra, Australian Capital Territory: Author. [Link](https://www.abs.gov.au/statistics/health/causes-death/causes-death-australia/latest-release).

Australian Institute of Health and Welfare. (2023) _The National Suicide and Self-Harm Monitoring System_. [Link](https://www.aihw.gov.au/suicide-self-harm-monitoring)

Christensen H., et al. (2022). Self-harm iceberg reveals hidden depth. MJA Insight 40: 1. [Link](https://insightplus.mja.com.au/2022/40/self-harm-iceberg-reveals-hidden-depth/)

Fergusson DM., et al. (2005). Suicidal behaviour in adolescence and subsequent mental health outcomes in young adulthood. _Psychological Medicine_, 35(7): 983-93. DOI: [10.1017/s0033291704004167](https://www.cambridge.org/core/journals/psychological-medicine/article/abs/suicidal-behaviour-in-adolescence-and-subsequent-mental-health-outcomes-in-young-adulthood/3BFFAB5FA36E1E3F6BD330DDF8B3102B)

Gillies D., et al. (2018). Prevalence and characteristics of self-Harm in adolescents: Meta-analyses of community-based studies 1990–2015. _J Am Acad Child and Adolesc Psychiatry_, 57: 733-41. DOI: [10.1016/j.jaac.2018.06.018](https://www.jaacap.org/article/S0890-8567(18)31267-X/abstract).

Koenig, J., et al. (2015). The association of self-injurious behaviour and suicide attempts with recurrent idiopathic pain in adolescents: evidence from a population-based study. __Child Adolesc Psychiatry Ment Health_, 9: 32. DOI: [10.1186/s13034-015-0069-0](https://doi.org/10.1186/s13034-015-0069-0)

Olfson M., et al. (2018). Suicide after deliberate self-harm in adolescents and young adults. _Pediatrics_, 141: e20173517. DOI: [10.1542/peds.2017-3517](https://publications.aap.org/pediatrics/article-abstract/141/4/e20173517/37791/Suicide-After-Deliberate-Self-Harm-in-Adolescents?redirectedFrom=fulltext).

Zagdańska MJ., et al. A (2013). Prevalence and age-of-onset distributions of suicidal thoughts, plans and attempts among students of nine public universities in Wroclaw, Poland: WMH-CIDI findings. _Eur Psychiatry_, 28: 1. DOI:[10.1016/S0924-9338(13)76060-7](https://www.cambridge.org/core/journals/european-psychiatry/article/896-prevalence-and-ageofonset-distributions-of-suicidal-thoughts-plans-and-attempts-among-students-of-nine-public-universities-in-wroclaw-poland-wmhcidi-findings/BCE09437F879CB3689891C58A64443A6)
