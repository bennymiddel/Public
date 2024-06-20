
## E N E R G I E W E N D E 
=========================

### Executive Summary

European unity and the free movement of goods and people also affects the electricity market. Today, the entire European Union is part of a large interconnected grid. Unlike the physical connection, however, the price of electricity is determined in the individual electricity price zones. These zones roughly correspond to the individual member states. In the past, the electricity price followed the general and low inflation and did not show any major outliers. 

This changed with the coronavirus pandemic and the after-effects of massive government subsidy programmes, which have intensified, if not triggered, post-Covid inflation. 

During this period of transition from Covid-19, another event followed that influenced the price of electricity in Europe. The Ukraine war that began on 24 February 2022 triggered an energy crisis in Europe that drove electricity prices to unprecedented heights. 

During this time of crisis, the ruling coalition in Germany decided to take the remaining nuclear power plants off the grid, even though experts expected these existing plants to have a diminishing effect on the price of electricity.

The following work aims to analyse the impact of these two events on the electricity price in the Germany-Luxembourg price region. For this purpose, after a data analysis and adjustment phase, a model is first created based on the price data of the past before the war and the final nuclear phase-out, which predicts the price development without external effects. This model serves as the basis and benchmark for a further model that combines price data from the neighbouring zones, exports and imports to and from the Germany-Luxembourg zone, production in the zone, consumption in the zone and historical weather data.

#### Repository 

* `data` 
    - contains link to copy of the dataset (stored in a publicly accessible Google Drive folder)
    - saved copy of aggregated / processed data as long as those are not too large (> 10 MB)

* `model`
    - joblib dump of final model / model object

* `notebooks`
    - contains all final notebooks involved in the project
        - 01-data-loading-cleaning
        - 02-eda
        - 03-pre-processing
        - 04-modeling
        - 05-findings

* `docs`
    - contains final report which summarises the project

* `references`
    - contains papers / tutorials used in the project

* `src`
    - Contains the project source code (refactored from the notebooks)

* `.gitignore`
    - Part of Git, includes files and folders to be ignored by Git version control

* `conda.yml`
    - Conda environment specification

* `Makefile`
    - Automation script for the project

* `README.md`
    - Project landing page (this page)

* `LICENSE`
    - Project license


------------------------------------------------------------------------------