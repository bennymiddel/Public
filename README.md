
## E N E R G I E W E N D E 
## Estimation of the effects of major events on the electricity prices in germany using using machine learning models
By back-induction based on a machine learning algorithm, outliers are
detected in an electricity price time series and assigned to specific events.

=========================

Benedikt Middelstaedt, 07/07/24 London

### Executive Summary

European unity and the free movement of goods and people also affects the electricity market. Today, the entire European Union is part of a large interconnected grid. Unlike the physical connection, however, the price of electricity is determined in the individual electricity price zones. These zones roughly correspond to the individual member states. In the past, the electricity price followed the general and low inflation and did not show any major outliers. 

This changed with the coronavirus pandemic and the after-effects of massive government subsidy programmes, which have intensified, if not triggered, post-Covid inflation. 

During this period of transition from Covid-19, another event followed that influenced the price of electricity in Europe. The Ukraine war that began on 24 February 2022 triggered an energy crisis in Europe that drove electricity prices to unprecedented heights. 

During this time of crisis, the gas distribution from russia was first reduced, than disrupted and showed a major impact on the electricity prices in europe.

The following work aims to analyse the impact of these two events on the electricity price in the Germany-Luxembourg price region. For this purpose, after a data analysis and adjustment phase, a model is first created based on the price data of the past before the war and the final nuclear phase-out, which predicts the price development without external effects. This model serves as the basis and benchmark for a further model that combines  exports and imports to and from the Germany-Luxembourg zone, production in the zone,and consumption in the zone.

The results are determined using a systematic approach of data loading, EDA, pre-processing and modelling, which is reflected in the project's notebooks.

- [01 - data-loading and cleaning](/notebooks/01-data-loading-cleaning.ipynb)
- [02 - eda ](/notebooks/02-eda.ipynb)
- [03 - splitting and and pre-processing](/notebooks/03-splitting-and-pre-processing.ipynb)
- [04 - modelling and findings](/notebooks/04-modelling-and-findings.ipynb)


The individual steps are explained and the interim results are categorised and presented graphically whenever appropriate. The trained models - SARIMAX and XGBoost - are also saved as .pkl files and can be accessed. 

The systematic approach is explained in markdown cells and the code is explained as a direct comment within the code blocks wherever useful and appropriate. 

==========================================
### The general findings:

The aim was to build a model based on the normal price ranges that could replicate the price development over the period as precisely as possible. The difference between this and the current price can be identified and quantified as an anomaly or outlier. 

![alt text](/images/image-7.png)

The model makes it possible to quantify the costs of the time series anomaly between May 2021 and the end of the period in May 2024 - in addition, individual outliers can be assigned to specific events. The additional costs can be quantified by multiplying them by the entire generation.  

![alt text](/images/image.png)


By multiplying by the generation, the anomaly can be specified at a cost of €13.6 billion, of which €5.8 billion is caused by the gas supply crisis and €3.43 billion by the war as a single event.  4.4 B€ cannot be allocated to either of the two events. In general, it can be said that the anomaly represents an additional cost of 40% compared to the expected increase. 


#### Repository 

* `data` 
    - contains link to copy of the dataset (stored in a publicly accessible Google Drive folder)
    - saved copy of aggregated / processed data as long as those are not too large (> 10 MB)

* `model`
    - joblib dump of all trained models

    - contains link to copy of the dataset (stored in a publicly accessible Google Drive folder)
    - saved copy of aggregated / processed data as long as those are not too large (> 10 MB)


* `notebooks`
    - contains all final notebooks involved in the project
        - 01-data-loading-cleaning
        - 02-eda
        - 03-splitting-and-pre-processing
        - 04-modeling-and-findings

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