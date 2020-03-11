{{ cookiecutter.project_name.lower().replace(' ', '_') }}
==============================

{{cookiecutter.description}}

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make repo` or `make data`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-rxb-whats-an-ocean`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── environment.yml    <- The requirements file for reproducing the analysis environment,
    │                         installed via `conda env update -f environment.yml`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── {{ cookiecutter.project_name.lower().replace(' ', '_') }}    <- Source code for use in this project.
    │   ├── __init__.py    <- Makes {{ cookiecutter.project_name.lower().replace(' ', '_') }} a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    |
    ├── .gitignore         <- Tells Github which files to ignore when adding to repository.
    |
    ├── .pre-commit-config.yaml <- Configuration file for `pre-commit`.
    |
    ├── .travis.yml           <- Configuration file for Travis Continuous Integration.
    |
    ├── create_repo.sh    <- Script to create Github repository for this folder.


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
