[![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tuftsdatalab/intro-numpy/main?urlpath=lab/tree/intro-numpy.ipynb){:target="_blank"}&nbsp;
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tuftsdatalab/intro-numpy/blob/main/intro-numpy.ipynb){:target="_blank"}&nbsp;
[![Download Notebook](https://tuftsdatalab.github.io/badges/jupyter.svg)](https://cdn.jsdelivr.net/gh/tuftsdatalab/intro-numpy@main/intro-numpy.ipynb)&nbsp;
[![View on Github](https://tuftsdatalab.github.io/badges/github.svg)](https://github.com/tuftsdatalab/intro-numpy){:target="_blank"}&nbsp;
![last updated](https://img.shields.io/github/last-commit/tuftsdatalab/intro-numpy?label=last%20updated)

**A Tufts University Data Lab Workshop**\
Written by Uku-Kaspar Uustalu

[![datalab.tufts.edu](https://tuftsdatalab.github.io/badges/datalab.svg)](https://sites.tufts.edu/datalab){:target="_blank"}&nbsp;
[![@TuftsDataLab](https://tuftsdatalab.github.io/badges/twitter.svg)](https://twitter.com/intent/follow?screen_name=tuftsdatalab){:target="_blank"}

Python resources: [go.tufts.edu/python](https://sites.tufts.edu/datalab/python/){:target="_blank"}\
Questions: <datalab-support@elist.tufts.edu>\
Feedback: <uku-kaspar.uustalu@tufts.edu>

Workshop slides: [tufts.box.com/v/numpy-slides](https://tufts.box.com/v/numpy-slides){:target="_blank"}\
Live offerings: [go.tufts.edu/workshops](https://sites.tufts.edu/datalab/workshops/){:target="_blank"}

---
This interactive workshop serves as an introduction to scientific computing in Python and demonstrates how to work with matrices and multidimensional arrays using the popular [NumPy](https://numpy.org/){:target="_blank"} library. It also introduces plotting with [Matplotlib](https://matplotlib.org/){:target="_blank"} and outlines some key differences between NumPy, MATLAB, C/C++. and Fortran. The workshop is best suited for those with some previous experience in Python programming and scientific computing.

Although intended for use in a live instructor-guided session, the interactive workshop notebook is well-commented and fully suitable for self-guided study. Please check the [Data Lab workshop schedule](https://sites.tufts.edu/datalab/workshops/){:target="_blank"} for upcoming live offerings of this workshop.

---
## Running the Workshop Notebook

The workshop notebook can be run in a cloud-computing environment or using a local [Anaconda](https://www.anaconda.com/products/individual){:target="_blank"} installation. Please select the most suitable option for you.

- Use a cloud-computing environment *(does not require the installation of additional software)*
    - [Virtual JupyterLab interface via **Binder**](#binder) *(reccomneded)*
    - [Google Colab](#colab)
- [Run the notebook locally on your computer](#local) *(requires an Anaconda installation)*

---
## Using Binder (virtual JupyterLab) to Run the Notebook {#binder}
[![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tuftsdatalab/intro-numpy/main?urlpath=lab/tree/intro-numpy.ipynb){:target="_blank"}

Follow the instructions below to launch the notebook in an online version of the [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/){:target="_blank"} interface pre-configured for this workshop.

1. Click on the [**Launch Binder**](https://mybinder.org/v2/gh/tuftsdatalab/intro-numpy/main?urlpath=lab/tree/intro-numpy.ipynb){:target="_blank"} button above.
2. A Binder instance will launch in a new tab with the message *Starting Repository*.
3. Wait patiently and do not close the Binder tab.
4. After a few minutes, the notebook will launch in a JupyterLab instance.

---
## Using Google Colab to Run the Notebook {#colab}
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tuftsdatalab/intro-numpy/blob/main/intro-numpy.ipynb){:target="_blank"}

Follow the instructions below to launch the workshop notebook in the [Google Colab](https://colab.research.google.com/){:target="_blank"} interactive Python notebook environment. *Note that a Google account is required to run notebooks in Google Colab.*

1. Click on the [**Open in Colab**](https://colab.research.google.com/github/tuftsdatalab/intro-numpy/blob/main/intro-numpy.ipynb){:target="_blank"} button above. The Google Colab interface will open in a new tab.
2. If you are not already signed into your Google account, click on *Sign In* in the upper-right corner and sign in with your Google credentials. **You must be signed in with a Google account to be able to run notebooks in Google Colab.**
3. *Optional:* If you want to keep track of your progress and retain any changes you make to this notebook, you should save a copy of the notebook to your Google Drive. This can be done by clicking the *Copy to Drive* button or selecting *File > Save a copy in Drive*. The notebook will be saved to the *Colab Notebooks* folder in your Google Drive. Once the saved copy pops up, close the original file and use the copy for the rest of the workshop. Feel free to rename the copy if desired. Any changes you make to your personal copy will automatically be saved.

*You might also see a message warning you that this notebook was not authored by Google and hence might contain malicious code. You can trust Data Lab notebooks, so click __Run Anyway__. But when running other third-party notebooks, you should review the code beforehand.*

---
## Running the Notebook Locally on your Computer {#local}
[![Download Notebook](https://tuftsdatalab.github.io/badges/jupyter.svg)](https://cdn.jsdelivr.net/gh/tuftsdatalab/intro-numpy@main/intro-numpy.ipynb)

The following assumes that you have [Anaconda](https://www.anaconda.com/products/individual){:target="_blank"} installed on your computer along with [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/){:target="_blank"}, [NumPy](https://numpy.org/){:target="_blank"}, and [Matplotlib](https://matplotlib.org/){:target="_blank"}. These packages are all included in Anaconda by default, so there is no need to individually install them if you have an unmodified Anaconda installation.

If you have not done so already, [install Anaconda]((https://docs.anaconda.com/anaconda/install/){:target="_blank"}) on your computer. Then follow the instructions below to run the workshop notebook in a locally hosted JupyterLab environment.

1. Click on the [**Download Notebook**](https://cdn.jsdelivr.net/gh/tuftsdatalab/intro-python@master/intro-python.ipynb) button above to download the workshop notebook. It is recommended you create a designated folder for this workshop and move the notebook there.
2. Launch JupyterLab either from the **command line** or via **Anaconda Navigator**.
    - From the **command line**:
        1. Launch **Terminal** (*macOS/Linux*) or the **Anaconda PowerShell Prompt** (*Windows*).
            - **Windows**: *Start > Anaconda3 > Anaconda PowerShell Prompt*
            - **macOS**: *Applications > Utilities > Terminal*
        2. Type `jupyter lab` and press **Enter/Return**.
    - Using **Anaconda Navigator**:
        1. Launch Anaconda Navigator via the Start Menu (*Windows*) or from Applications (*macOS*).
            - **Windows**: *Start > Anaconda3 > Anaconda Navigator*
            - **macOS**: *Applications > Utilities > Terminal*
        2. Launch **JupyterLab** using the corresponding *Launch* button.
3. JupyterLab will open in a web browser. (A new tab will be generated if a browser is already open.)
4. Within the JupyterLab file explorer on the left, navigate to the location of the downloaded **intro-python.ipynb** notebook.
5. Once you are in the correct directory, *double-click* on **intro-python.ipynb** in the file browser to open the workshop notebook.