# Cookiecutter Climate Science

_A trimmped down version of cookiecutter data science for publishable climate science projects._


#### [Project homepage](http://drivendata.github.io/cookiecutter-data-science/)


### Requirements to use the cookiecutter template:
-----------
 - Python 3.8
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
------------

    cookiecutter https://github.com/bradyrx/cookiecutter-climate-science
    
Then move into the new folder and run `make repo`, which will automatically create the Github repo for your project. You'll have to enter your Github password.

Following this, run `make create_environment` to create a conda environment specifically for this project. Follow that with `make requirements` to install the default package requirements. You can update `environment.yml` to add/remove packages to this environment.

Finally, run `make pre-commit` to install the `pre-commit` rules. [pre-commit](https://pre-commit.com/) is an awesome service that runs a bunch of tests/formatting scripts prior to the user being able to commit their code. This will ensure that it looks good stylistically, passes `flake8` tests, etc.

For Travis to work, I believe you'll need to go to https://travis-ci.com/ and connect Travis to your repository. You can also ensure that Travis runs on your Pull Requests. I haven't tested this just yet.


### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```
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
    ├── project_name    <- Source code for use in this project.
    │   ├── __init__.py    <- Makes project_name a Python module
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
```
