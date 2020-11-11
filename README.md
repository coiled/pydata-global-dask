# Scaling your data work with Dask

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/coiled/pydata-global-dask/master?urlpath=lab)

This repository contains the materials for the "Scaling your data work with Dask" tutorial at PyData Global 2020.

## Running the tutorial

There are two ways in which you can set up and go through the tutorial materials. Both of which are outlined in the table below.

|     Method    | Setup | Description |
| :-----------: | :-----------: | ----------- |
| Binder        | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/coiled/pydata-global-dask/master?urlpath=lab)         | Run the tutorial notebooks on mybinder.org without installing anything locally. Note that due to resource limits, the tutorial notebooks will automatically use smaller datasets when running on Binder.       |
| Local install | [Instructions](#Local-installation-instructions)          | Download the tutorial notebooks and install the necessary packages (via `conda`) locally. Setting things up locally can take a few minutes, so we recommend going through the installation steps prior to the tutorial.    |


## Local installation instructions

### 1. Clone the repository

First clone this repository to your local machine via:

```
git clone https://github.com/coiled/pydata-global-dask
```

Alternatively, you can download a zip file of the repository at the top of the main page of the repository. If you prefer not to use git or don't have experience with it, this a good option.

### 2. Download conda (if you haven't already)

If you do not already have the conda package manager installed, please follow the instructions [here](https://docs.conda.io/en/latest/miniconda.html). 

### 3. Create a conda environment

Navigate to the `pydata-global-dask/` directory and create a new conda environment with the required
packages via:

```
cd pydata-global-dask
conda env create -f binder/environment.yml
```

This will create a new environment named "pydata-global-dask". Next, activate the environment:

```
conda activate pydata-global-dask
```

and install the JupyterLab extensions used in the tutorial with:

```
jupyter labextension install dask-labextension @jupyter-widgets/jupyterlab-manager
```

### 4. Launch JupyterLab

Finally, launch JupyterLab with:

```
jupyter lab
```
