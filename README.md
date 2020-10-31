# pysal-narsc20

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sjsrey/pysal-narsc20/master?urlpath=lab)

PySAL Workshop at NARSC20

### Instructors

* Serge Rey - University of California Riverside, Center for Geospatial Sciences
* Elijah Knaap - University of California Riverside, Center for Geospatial Sciences

---

## Schedule

### AM Session
1. Introduction (20 min)
    - Welcome
    - PySAL Overview
3. Software and Tool (60 min)
    - Anaconda Python Distribution
    - IPython/Jupyter Notebooks
4. Python Primer (80 min)
    - Data structures
    - Control and Iteration
    - Functions and Modules
    - Files
    
### Break (1-hour)

### PM Session

3. PySAL for ESDA (80 min)
    - Spatial data processing with PySAL (40 min)
        - Processing spatial data with PySAL
        - Spatial weights in PySAL
    - ESDA with PySAL (40 min)
        - Global spatial autocorrelation analysis
        - Local spatial autocorrelation analysis
4. PySAL for Regional Analysis (80 min)
    - Regionalization (40 minutes)
        - clustering
        - spatially constrained clustering
    - Spatial Segregation Analysis (40 minutes)
        - spatial and aspatial indices
        - comparative inference
        - decomposition


## Obtaining Workshop Materials

**To get started immediately without installing or downloading anything, click the *"Launch Binder"* button at the top of this page**

---
If you are familiar with GitHub, you should clone or fork this GitHub repository to a specific directory. Cloning can be done by:

``` bash
git clone https://github.com/sjsrey/pysal-narsc20.git
```

If you are not using git, you can grab the workshop materials as a zip file by pointing your browser to (https://github.com/sjsrey/pysal-narsc20.git) and clicking on the green _Clone or download_ button in the upper right.

![download](figs/readmefigs/download.png)

Extract the downloaded zip file to a working directory.

## Installation

We will be using a number of Python packages for geospatial analysis.

An easy way to install all of these packages is to use a Python distribution such as [Anaconda](https://www.anaconda.com/download/#macos). In this workshop we will use anaconda to build an [environment](https://conda.io/docs/user-guide/tasks/manage-environments.html) for **Python 3.6**. It does not matter which version of anaconda is downloaded. We recommend installing Anaconda 3.7.

![anaconda](figs/readmefigs/anaconda.png)

On windows, all our work will begin from an anaconda prompt, which you can start as follows:

![anacondaprompt](figs/readmefigs/anacondastartwin.png)

Start a terminal and navigate to the directory of the downloaded/ cloned materials. For example, if the materials now live in the directory `/Users/sjsrey/Downloads/pysal-narsc20` , you need to navigate to that directory from the terminal (using command `cd` ):

![directory](figs/readmefigs/directory.png)

Once we have done that, run:

``` bash
conda-env create -f environment.yml
```

This will build a conda python 3.7environment that sandboxes the installation of the required packages for this workshop so we don't break anything in your computer's system Python (if it has one).

This may take 10-15 minutes to complete depending on the speed of your network connection.

Once this completes, you can activate the workshop environment with:

``` bash
conda activate pysal-narsc20
```

You're now all setup for the tutorial!

## Troubleshooting

If you encounter the following error when starting jupyterlab:

``` bash
FileNotFoundError: [WinError 2] The system cannot find the file specified
```

A solution is to issue the following command in the anaconda prompt:

``` bash
 python -m ipykernel install --user
```
