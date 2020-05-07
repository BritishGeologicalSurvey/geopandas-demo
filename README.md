# GeoPandas Demo

[![DOI](https://zenodo.org/badge/140001231.svg)](https://zenodo.org/badge/latestdoi/140001231)

This repository contains a Jupyter notebook that demonstrates some of the
GIS-like functionality of the GeoPandas Python library.  It uses data from the
British Geological Survey's [earthquake catalogue](http://earthquakes.bgs.ac.uk/earthquakes/dataSearch.html) and the public domain [Natural Earth](http://www.naturalearthdata.com) project to calculate the towns in the UK that feel the most earthquakes.

Follow the instructions below to install and run the demonstration on your own
machine.  Alternatively, you can [view the code and
results](GeoPandas_demo.ipynb) in your browser.  Click [here](https://nbviewer.jupyter.org/github/BritishGeologicalSurvey/geopandas-demo/blob/master/GeoPandas_demo.ipynb) for mobile-friendly version rendered by _Jupyter nbviewer_.


## Prerequisites

+ Python 3
+ A Python 3 package manager e.g. pip3, conda
+ `libspatialindex` (Required for spatial joins. `apt install
  libspatialindex-c4v5` on Debian/Ubuntu)


## Installing dependencies


The following packages should be installed via `pip3` or `conda`:

```
pip3 install -r requirements.txt
```

### For developers

To test that the notebook runs to completion, extra packages are required:

```bash
pip3 install -r requirements-dev.txt
```

Run the test with:

```bash
pytest --nbval-lax GeoPandas_demo.ipynb
```


## Starting the notebook

The demo runs in a Jupyter notebook.  Start the notebook with:

```
jupyter notebook
```

A browser window will open at [http://localhost:8888](http://localhost:8888)
with a list of available notebooks.
