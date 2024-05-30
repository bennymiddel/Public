[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15133407&assignment_repo_type=AssignmentRepo)
# Usage



This is a template repository for quickly setting up a data science project
It includes a simple folder structure and a conda environment for isolated dependency management.

1. Start a new repo using this template
2. Update your `LICENSE` file.
3. Update your `README.md` file. 
4. Set up and activate conda environment
    1. Rename your conda environment in the `./conda.yml` file.
    2. Add/change any dependencies and their versions in the `./conda.yml` file.
    3. Set up your conda environment and activate it by running:
        ```bash
        conda env create -f conda.yml
        conda activate <your-env-name>
        ```
5. Add your own scripts in `./src/`
6. Add your own notebooks in `./notebooks/`
7. Add your own data in `./data/`
    gitignore will ignore the data folder when you push to github
    save a copy of your raw and process data, 
    pickled models in a Google Drive folder
    and add the link in the gdrive-links.md file
8. Add your project documents, reports, presentation pdfs in the `./docs`
9. Add your references (tutorials, papers, books etc.) in `./references` 

------------------------------------------------------------------------------

## Capstone - tbc
=========================

### Executive Summary

Analysing the energy market and the relationships between electricity production, demand and price. The following three problems are to be analysed and translated into a solution. 

Prediction of energy production and demand
Develop a model to predict future energy production and demand.
    Feature engineering (e.g. weather data, public holidays).
    Model training and evaluation.
Anomaly detection in energy production:
Create a system to detect anomalies in energy production and demand.
    Identification and labelling of normal operating states.
    Application of anomaly detection techniques to historical data.
Optimisation
Develop a model to optimise the energy market based on price and market conditions.
    Allow capacity expansion


Gain insights into the structure of the energy supply from the data set. In addition to the problems posed above, the following questions should be answered: 

1. Did the expansion of renewable energies lead to an increase in price?

2. Is an expansion of renewable energies to 100% achievable in a market economy?

3. Is there an optimal expansion point for renewable energies?

4. What influence does the nuclear phase-out have


The data is divided into:

-Generation and form of generation (329440, 15)
-demand for electricity (329440, 5)
-Export/import balance (329440, 25)
-Electricity price and electricity price in neighbouring countries Prices (329440, 17)


In the course of the project, weather data (historical), price data (CO2, variable costs and investment costs) will be added as required. However, these are not necessary for the entire duration of the data sets and will be loaded as required. 
### Demo

... Show your work:
...     Data visualisations
...     Interactive demo (e.g., stremlit app)
...     Short video of users trying out the solution


### Methodology

... High-level diagrams of entire process:
...     various data processing steps
...     various modelling directions
...     various prototyping directions


### Organization

#### Repository 

* `data` 
    - contains link to copy of the dataset (stored in a publicly accessible Google Drive folder)
    - saved copy of aggregated / processed data as long as those are not too large (> 10 MB)

* `model`
    - joblib dump of final model / model object

* `notebooks`
    - contains all final notebooks involved in the project

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

#### Dataset

... Google Drive links to datasets and pickeled models

### Credits & References

... Include any personal learning

------------------------------------------------------------------------------