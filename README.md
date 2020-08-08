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

Copyright 2020 Squark

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
