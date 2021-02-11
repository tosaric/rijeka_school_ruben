You *must* have a Github account to access this repo.
You *must* be a LST member to access this repo.

# What you need

To prepare for the lessons, please do the following steps:

1. Install general software (Before Day 1)
2. Install CTA-specific software (Before Day 2)
3. Access to the La Palma IT Cluster and LST Data (Before Day 3)

## 0. Pre-requirements
To have a look at this is not compulsory but very much recommended:

[Introduction to Python for Scientists](http://astrofrog.github.io/py4sci/)

## 1. Install software

Please come with your computer and software already installed. If you have problems, do not hesitate to write before the start of the lessons.
In any case, we will have a setup session the first day to solve problems with the installations.

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
* More information for IPython (how to start and execute notebooks) is available in Chapter 1 of the ["Python Data Science Handbook"](http://nbviewer.jupyter.org/github/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/Index.ipynb)

* Basic knowledge of python is necessary for the start of the course, here there are a good list of notebooks and the Python Data Science Handbook:
   * https://github.com/jakevdp/WhirlwindTourOfPython
   * https://github.com/jakevdp/PythonDataScienceHandbook

## 2. Install CTA-specific software
For the purposes of the lessons, we will need [ctapipe](https://github.com/cta-observatory/ctapipe), [cta-lstchain](https://github.com/cta-observatory/cta-lstchain), [gammapy](https://github.com/gammapy/gammapy) and all the auxiliary software coming with them.

You can create a conda environment and install all the needed LST-specific software and its dependencies by following the instrunctions of cta-lstchain [installation](https://github.com/cta-observatory/cta-lstchain#as-user)

## 3. Access to the La Palma IT Cluster and LST Data
There is an IT cluster in LP that allows to access data and run analysis on site, it is powerful and can be used for LST and CTA members. It is wise to have access to data there.
Obtain an LDAP account
Send a request to Daniela Hadasch (hadasch@icrr.u-tokyo.ac.jp) to be included in the "ctan-onsite-it" group and the `lst` group (to access LST data at PIC).
 
Afterwards you will receive an e-mail from Microsoft Online Services Team. Follow the instructions in the e-mail. Once you logged in with the temporary password, you have to set your own password. 
 
Your LDAP account looks like this:

user name: firstname.lastname

password: <the password you just set>
 
with an associated e-mail address firstname.lastname@cta-observatory.org. 

#### Log in to the IT center
Follow the 2-step authentication system:
 
0.) You need to have a registered secure IP in your institute. It is recommended that you have a central server at your institute that acts as a gate, but you can also access the IT center through PIC (username@mic.magic.pic.es)

1.) You login with the general user CtAlAPaLmA to a general login server. The system automatically redirects you to server login01 or login02:

`$ ssh -l CtAlAPaLmA 161.72.87.1`
 
The password for this account can be found here:
https://ctaoobservatory.sharepoint.com/sites/ctan-onsite-it/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2Fctan%2Donsite%2Dit%2FShared%20Documents%2FGeneral%2Finformation%2Ejpg&parent=%2Fsites%2Fctan%2Donsite%2Dit%2FShared%20Documents%2FGeneral
 
2.) From one of the login servers you can now login with your LDAP account either to cp01 or cp02. Special telescope accounts can login to the telescope servers tcs01-07. 

`$ ssh -l firstname.lastname cp01/cp02`
 
After you have logged in for the first time your home directory with a quota of 10GB will be automatically created:
/fefs/home/firstname.lastname


### 3.1 Setup of the IT cluster environment for the lessons
You will need a n up to date lstchain installation. You can either install anaconda and lstchain yourself, or add these lines to your .bashrc:

`export PATH="/home/ruben.lopez/anaconda3/bin:$PATH"`

then type:

`conda init`

and the configuration should be added to your bashrc. The conda environment is called `lst-dev`, therefore to activate it, every time you log in, you should type:

`conda activate lst-dev`

### 3.2 Download materials:
All attendees should be LST members to be able to access LST data. Data can be downloaded by accessing http://data.lstcam.pic.es/ using your personal credentials.

#### Troubleshooting
LST data at PIC is located in:
http://data.lstcam.pic.es/

it may be that when you got the aforementioned account, you still cannot access the link where data is stored at PIC. You need to be added to the `1584(lst)` group of the IT center. Please write Daniel Mazin (mazin@icrr.u-tokyo.ac.jp).
