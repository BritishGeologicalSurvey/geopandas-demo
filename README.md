# GeoPandas Demo

This repository contains a Jupyter notebook that demonstrates some of the
GIS-like functionality of the GeoPandas Python library.  It uses data from the
British Geological Survey's [earthquake catalogue](http://earthquakes.bgs.ac.uk/earthquakes/dataSearch.html) and the public domain [Natural Earth](http://www.naturalearthdata.com) project to calculate the towns in the UK that feel the most earthquakes.

Follow the instructions below to install and run the demonstration on your own
machine.  Alternatively, you can view the code and results by browsing to the
[GeoPandas_demo.ipynb](GeoPandas_demo.ipynb) file.


## Prerequisites

+ Python 3
+ A Python 3 package manager e.g. pip3, conda
+ `libspatialindex` (Required for spatial joins. `apt install
  libspatialindex-c4v5` on Debian/Ubuntu)


## Installing dependencies

#### Via package manager

The following packages should be installed via `pip3` or `conda`:

```
pip3 install geopandas jupyter rtree
```

#### Via Pipenv

Alternatively, dependencies can be install via Pipenv.

[_Pipenv_](https://docs.pipenv.org) is a package and virtual environment
manager for Python.  Virtual environments allow you to install Python packages
without interfering with your system installation or other projects.

Pipenv reads the dependency information from the `Pipfile`.  A virtual
environment with the dependencies installed can be created and started as
follows:

```
pipenv create
pipenv install
pipenv shell
```

The shell session can be ended with `exit`.


## Starting the notebook

The demo runs in a Jupyter notebook.  Start the notebook with:

```
jupyter notebook
```

A browser window will open at [http://localhost:8888](http://localhost:8888)
with a list of available notebooks.
