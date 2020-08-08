# Cookiecutter Squark

### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.5
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

    cookiecutter https://github.com/prabhuSub/cookiecutter-squark.git


### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```
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
├── models             <- Trained and serialized models, model predictions, or model summaries. Word2vec models
│
├── notebooks          <- Jupyter notebooks. POC(proof of concepts). 
│                         Naming conventions to be followed by every contributer to recognize the author                         
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
└── src                <- Source code for use in this project.
    ├── main           <- folder containing all main scripts
    │     ├── lib      <- containing all the libraries that needs to be imported into preprocessor and automodeler. 
    │     │               ex: H2O, DataIO, Wrangler, Analysis, etc.
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
```

### Installing development requirements
------------

    pip install -r requirements.txt
    
------------
