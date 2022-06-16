## Steps to install miniconda

- Visit the official [conda site](conda.io).
- Locate the link for miniconda. 

![Link to download miniconda](images/install-1.png)

- Select the appropriate Miniconda installation for your computer (in this case, it is highlighted as a Windows 64-bit installation).

:::{hint} 
Note the current version of Python that will be installed also. Below, this is listed as “Python 3.9.7”.  Typically, if one wants a previous version of Python installed, alternative links will be available further down on the page.
:::

![Downloading Miniconda for Windows](images/install-2.png)

:::{note} 
We will be installing napari into its own virtual environment. One could have more than one virtual environment with napari installed into each, in the case it had different versions, dependency requirements, etc (or for other programs, for example). The environment manager (in this case miniconda), manages these environments for you.
:::

- Once the download has finished, run it. Default installation options are typically sufficient.
- This can be found by clicking on the lower left windows icon (Windows 10) and either typing **“anaconda…”** (in which case it will find "**Anaconda Prompt (miniconda3)"**), or scrolling down to the anaconda folder and finding it.

![Finding the Anaconda prompt](images/install-3.png)

- This launches the command prompt into the **“base environment”** (as denoted by **“(base)”** at the start of the command line). This is not the virtual environment yet, as we haven’t created one, and as such, is not the environment we’ll be installing napari into.

:::{hint} 
If you plan on running napari on a regular basis, it may be handy at this point to create a shortcut to the Anaconda Prompt, or pin it to your taskbar, for easy access.
:::
