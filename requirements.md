You *must* have a Github account to access this repo.

# If you have problems:


## What you need

To prepare for day 1, please do the following two steps:

1. Install general software
1.1 Install CTA-specific software
2. Download materials

### 1. Install software

Please come with your computer and software already installed. If you have problems, do not hesitate to write before the start of the lessons.
In any case, we will have a one-hour final setup the first day.

We recommend you install Anaconda from https://www.anaconda.com/ 

To check that your installation and setup is OK, try to exectue the following Python code:
* `print('hello world!')`
* `import numpy`
* `import scipy`
* `import matplotlib`
* `import astropy`

If you get an `ImportError` you don't have all the software we will use.

Try to execute `print('hello world')` from three places:
1. Python terminal (type `python` to start)
2. IPython terminal (type `ipython` to start)
3. IPython notebook (= Jupyter notebook) (type `jupyter-notebook` to start)

You can find instructions how to do the installation and how to start Python and IPython and execute your first Python code here:

* Section 1 ("Introduction", install section at the bottom) and 2 ("How to run Python code") from ["A Whirlwind Tour of Python"](http://nbviewer.jupyter.org/github/jakevdp/WhirlwindTourOfPython/blob/master/Index.ipynb)
* More information for IPython (how to start and execute notebooks) is available in Chapter 1 of the ["Python Data Science Handbook"](http://nbviewer.jupyter.org/github/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/Index.ipynb)~


### 1.1 Install CTA-specific software
For the purposes of the lessons, we will need [ctapipe](https://github.com/cta-observatory/ctapipe), [cta-lstchain](https://github.com/cta-observatory/cta-lstchain), [gammapy](https://github.com/gammapy/gammapy) and all the auxiliary software coming with them.

You can create a conda environment and install all the needed LST-specific software and its dependencies by following the instrunctions of cta-lstchain [installation](https://github.com/cta-observatory/cta-lstchain#as-user)


2. Download materials
All attendees should be LST members to be able to access LST data. Data can be downloaded by accessing http://data.lstcam.pic.es/ using your personal credentials.