airbnb_optimization
==============================

An attempt to find the best airbnb listing under price constraints. Project generated from [cookie-cutter-data-science](https://drivendata.github.io/cookiecutter-data-science/)

Project Organization
------------

    ├── LICENSE
    ├── README.md          <- Top-level README
    ├── data
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   ├── interim        <- Intermediate data that has been transformed/concatenated.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── models             <- Models for `Best` Airbnb Listing under price constraints
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
                              generated with `pip freeze > requirements.txt`
--------

## Personal Checklist :rocket:
- [ ] Data cleaning (extract relevant columns, deal with NAs & Outliers)
- [ ] Data Exploration and Visualization (Play around with Plotly a bit)
- [ ] Implement most basic model to mind -> Lagrangian Optimization with multiple constraints
- [ ] Research optimization methods

## Issues :anger:
1. Currently no way to measure `performance` of model (since there isn't user feedback of the model) so choosing a model that's highly interpretable is preferable (reason for `Lagrangian`). However, I could use my trip to Cancún in March as a benchmark and compare my experience to model score output. Also, there is opportunity to use model for finding the `optimal` listing for trip to Toronto in August. 
2. Not Automated. Prob look to connect `flask app takes input -> crawler -> s3 bucket -> data processing -> model ranking listings -> flask app output` in the future.
3. Web scraping spider is not going to be reliable or ideal as Airbnb changes their site often (also has potential to harm the site). At this moment (June 30, 2019), Airbnb is not accepting new access requests for their API. *I really do hope* that access will be available for the future. 


