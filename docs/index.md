---
binder_popup: "[binder-link]{:target='_blank'}"
binder_button: "[![Launch Binder](https://mybinder.org/badge_logo.svg)][binder-link]{:target='_blank'}"
colab_popup: "[colab-link]{:target='_blank'}"
colab_button: "[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)][colab-link]{:target='_blank'}"
notebook_button: "[![Download Notebook](../badges/jupyter.svg)][notebook-link]"
github_button: "[![View on Github](../badges/github.svg)][repo-link]"
zipball_button: "[![Download Zip](../badges/zip.svg)][zipball-link]"
tarball_button: "[![Download TarGz](../badges/tgz.svg)][tarball-link]"
---

{{ page.binder_button }}&nbsp;
{{ page.colab_button }}&nbsp;
{{ page.notebook_button }}&nbsp;
{{ page.github_button }}&nbsp;
{{ page.zipball_button }}&nbsp;
{{ page.tarball_button }}&nbsp;
![last updated][last-updated-badge]

**A Tufts University Data Lab Workshop**\
Written by {{ site.author }}

[![datalab.tufts.edu](../badges/datalab.svg)](https://sites.tufts.edu/datalab)&nbsp;
[![@TuftsDataLab](../badges/twitter.svg)](https://twitter.com/intent/follow?screen_name=tuftsdatalab)

Slides: [tufts.box.com/v/{{ site.slides }}](https://tufts.box.com/v/{{ site.slides }})\
Live offerings: [go.tufts.edu/workshops](https://go.tufts.edu/workshops)\
Contact: <datalab-support@elist.tufts.edu>

---
## Table of Contents {#toc}

- [Workshop Overview](#overview)
- [Running the Workshop Notebook using a Virtual JupyterLab Instance (Recommended)](#binder)
- [Running the Workshop Notebook using Google Colab](#colab)
- [Running the Workshop Notebook using a Local Anaconda Installation](#anaconda)
- [Running the Workshop Notebook using a Local Mambaforge Installation](#mambaforge)

---
## Workshop Overview {#overview}

This hands-on interactive workshop introduces you to scientific computing in Python and demonstrates how to work with matrices and multidimensional arrays using the popular NumPy library. The workshop is intended for those with some previous Python experience and draws comparisons between NumPy and alternatives like MATLAB, C/C++, and Fortran. The workshop notebook is suitable for self-guided study and covers the following:

- **Importing** Python **packages** and common **aliases**
- The NumPy **`numpy.ndarray`** a.k.a. **`np.array`** data structure
- Different ways of **creating**, **indexing**, and **slicing** NumPy arrays
- **Broadcasting** and using mathematical operators with `np.array`
- **Universal** functions and **aggregation** functions
- **Iterating** and **mapping** over elements in NumPy arrays
- ***Row-major*** vs ***column-major*** order and array **flattening**
- **Shape manipulation** and the difference between ***copies*** and ***views***
- Various options for **importing** and **exporting** NumPy arrays
- Tweaking the textual representation of numbers using **format strings**
- Reading files with Python using **`with`** and **`open()`**
- Quick overview of **creating** and **styling plots** with Matplotlib
- Creating a figure with multiple **subplots** in Matplotlib

The notebook is designed to be run in a pre-configured cloud-computing environment either via [Binder](#binder) or [Google Colab](#colab) and does not require the installation of any software. Use of [Binder](#binder) is recommended as it provides a JupyterLab interface and allows for an experience similar to using a local installation. It is also possible to run the workshop notebook using a local [Anaconda](#anaconda) or [Mambaforge](#mambaforge) installation. Instructions on how to install Anaconda or Mambaforge are available here: [go.tufts.edu/installingPython](https://go.tufts.edu/installingPython)

---
## Running the Workshop Notebook using a Virtual JupyterLab Instance (Recommended) {#binder}

{{ page.binder_button }}

1. Click on the [**Launch Binder**]{{ page.binder_popup }} button above.
2. A Binder instance will launch in a new tab with the message *Starting Repository*.
3. Wait patiently and do not close the Binder tab. After a few minutes, a **JupyterLab** instance will launch.
4. If the workshop notebook does not automatically open, *double-click* on `{{ site.file }}` in the file browser on the left.

---
## Running the Workshop Notebook using Google Colab {#colab}

{{ page.colab_button }}

1. Click on the [**Open in Colab**]{{ page.colab_popup }} button above. The Google Colab interface will open in a new tab.
2. If you are not already signed into your Google account, click on ***Sign In*** in the upper-right and sign in with your Google credentials. **You must be signed in with a Google account to be able to run notebooks in Google Colab.**
3. **Optional:** To retain any changes you make to this notebook, save a copy of the notebook to your Google Drive by clicking the ***Copy to Drive*** button or selecting ***File > Save a copy in Drive***. This will save the notebook to the `Colab Notebooks` directory in your Google Drive. Once the saved copy pops up, close the original notebook and use the copy going forward. Feel free to rename the copy if desired. Any changes made to your personal copy will be automatically saved.

*You might also see a message warning you that this notebook was not authored by Google and hence might contain malicious code. You can trust Data Lab notebooks, so click __Run Anyway__. But when running other third-party notebooks, you should review the code beforehand.*

---
## Running the Workshop Notebook using a Local Anaconda Installation {#anaconda}

{{ page.notebook_button }}

1. Click on the [**Download Notebook**][notebook-link] button above to download the workshop notebook.
2. Create a designated directory for this workshop and move the downloaded `{{ site.file }}` notebook there.
3. Launch **Anaconda Navigator** via the Start Menu (*Windows*) or from Applications (*macOS*).
    - **Windows**: *Start > Anaconda3 > Anaconda Navigator*
    - **macOS**: *Applications > Anaconda Navigator*
4. Launch **JupyterLab** using the corresponding ***Launch*** button.
5. JupyterLab will launch in a web browser. (A new tab will be generated if a browser is already open.)
6. Within the JupyterLab file explorer on the left, navigate to the directory containing the `{{ site.file }}` notebook.
7. Once you are in the correct directory, *double-click* on `{{ site.file }}` in the file browser to open the workshop notebook.

---
## Running the Workshop Notebook using a Local Mambaforge Installation {#mambaforge}

{{ page.zipball_button }}&nbsp;
{{ page.tarball_button }}

1. Launch **Terminal** (*macOS/Linux*) or **Mambaforge Prompt** (*Windows*).
    - **Windows**: *Start > Mambaforge > Mambaforge Prompt*
    - **macOS**: *Applications > Utilities > Terminal*
2. Run the following commands by typing or pasting the command into the console and then pressing <kbd>Enter</kbd> or <kbd>Return</kbd>.
    - Download and extract the workshop materials:\
      `curl -Lo - https://github.com/tuftsdatalab/{{ site.repo }}/archive/workshop.tar.gz | tar -xzf -`
    - Navigate into the extracted directory: `cd {{ site.repo }}-workshop`
    - Create a new environment for the workshop: `mamba env create -f environment.yml`
    - Activate the workshop environment: `conda activate {{ site.env }}`
    - Open the workshop notebook in JupyterLab: `jupyter lab {{ site.file }}`
3. JupyterLab will launch in a web browser. (A new tab will be generated if a browser is already open.)
4. If the workshop notebook does not automatically open, *double-click* on `{{ site.file }}` in the file browser on the left.
5. **Do not close the console!** Closing the console will also terminate JupyterLab. Leave the console running in the background.


[binder-link]: https://mybinder.org/v2/gh/tuftsdatalab/{{ site.repo }}/binder?urlpath=lab/tree/{{ site.file }}
[colab-link]: https://colab.research.google.com/github/tuftsdatalab/{{ site.repo }}/blob/workshop/{{ site.file }}
[notebook-link]: https://cdn.jsdelivr.net/gh/tuftsdatalab/{{ site.repo }}@workshop/{{ site.file }}
[repo-link]: https://github.com/tuftsdatalab/{{ site.repo }}
[zipball-link]: https://github.com/tuftsdatalab/{{ site.repo }}/archive/workshop.zip
[tarball-link]: https://github.com/tuftsdatalab/{{ site.repo }}/archive/workshop.tar.gz
[last-updated-badge]: https://img.shields.io/github/last-commit/tuftsdatalab/{{ site.repo }}?label=last%20updated
