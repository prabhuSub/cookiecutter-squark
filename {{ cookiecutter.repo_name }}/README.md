{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs(optional)     <- A default doc for references
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries. 
    │                         Word2vec models
    │
    ├── notebooks          <- Jupyter notebooks. POC(proof of concepts). 
    │                         Naming conventions to be followed by every author                         
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    └── src                <- Source code for use in this project.
        ├── main           <- folder containing all main scripts
        │     ├── lib      <- containing all the libraries that needs to be imported into preprocessor 
        │     │               and automodeler. ex: H2O, DataIO, Wrangler, Analysis, etc.
        │     │
        │     ├── logs     <- logs genereated for every run 
        │     ├── preprocessor.py     <-  first script to run in production
        │     └── automodeler.py      <- second to follow the first script
        │
        │
        ├── configuration  <- configuration folder of the project
        │
        │   (optional)
        └── visualization  <- Scripts to create exploratory and results oriented visualizations
            └── visualize.py

--------
