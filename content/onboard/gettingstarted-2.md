# Creating virtual environments and installing napari

## Creating a virtual environment

- We’ll now create a virtual environment and install napari into it. You can name your virtual environments anything you like. For this example, we’ll create a virtual environment called **“napari-env”**. However, *outside of the environment’s name, the exact syntax needs to be followed*. Just substitute your desired environment name for **napari-env** below and in subsequent steps. You can ensure this by hitting the enter key after typing. 

  ``` conda create -y -n *napari-env* -c conda-forge python=3.9 ```

- After hitting the enter key, the virtual environment is created with a specific Python version (3.9 in this case) installed into it.  If you need a different version of Python, specify that version instead of 3.9.

:::{note} 
For the purposes of this tutorial, it is not necessary to understand the nature of the syntax we’re using. However, it is critical, unless otherwise mentioned, that you copy the command syntax exactly as you see it here. 
:::

- While the virtual environment **“napari-env”** has been created, it has not been activated yet. You can tell this as **“(base)”** is still indicated on the command line:  

![Virtual environment syntax](images/install-4.png)

- To activate the virtual environment:

  - **conda activate *napari-env***

- **“(napari-env)”** should now be indicated on the command line:

![Virtual environment syntax modified](images/install-5.png)

## Installation of napari 

- To install napari into the activated environment, enter this command on the command line and hit enter:

  - **conda install -c conda-forge napari**

- This may take some time (a few minutes), and may reach a point where a user input is required to continue as dependencies are checked. If this is the case, the following will be displayed:

  - **Proceed ([y]/n)?**
  - You can type **y**, then enter, or simply hit enter.

- This may also take a few minutes to get all the requisite packages downloaded, extracted, and executed. 
- At this point, you will be returned to the prompt indicating the virtual environment you’ve just installed napari into. To launch napari, simply type the one word command below and hit enter:
  - **napari**

- In a few seconds, the napari viewer window should be displayed:

![Launching the napari viewer for the first time](images/install-6.png)

**Note:** The first time you launch napari may take longer than usual. 

- You have now successfully installed napari onto your machine!

## Launching napari after installation session

- Now that you have completed installation, the procedure for launching napari is:

:::{note} 
- Launch **“anaconda prompt (miniconda3)”** for Windows users or **terminal** for Mac users. 
- Activate the virtual environment you’ve created and installed napari into:
  - **conda activate *napari-env***
- Launch napari:
  - **napari**
:::
