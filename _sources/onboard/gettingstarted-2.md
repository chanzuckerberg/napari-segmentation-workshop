# Virtual environments, and installing napari

## Creating a virtual environment

- We’ll now create a virtual environment and install Python into it, in one step. The name of this environment is up to our choosing and does not necessarily need to be the same as below. For this example, we’ll be creating a virtual environment called **“napari-env”** to install napari into. However, *outside of the environment’s name, the exact syntax needs to be followed*. You can ensure this by hitting the enter key after typing. 

  - **conda create -y -n *napari-env* -c conda-forge python=3.9**

- After hitting the enter key, the virtual environment will be created and Python installed into it.

:::{note} 
For the purposes of this tutorial, it is not necessary to understand the nature of the syntax we’ll be using. However, it is critical, unless otherwise mentioned, that you copy the command syntax exactly as you see it here. 
:::

- While the virtual environment **“napari-env”** has been created, it has not been activated yet. You can tell this as **“(base)”** is still indicated at the command line:  

![Virtual environment syntax](images/install-4.png)

- To activate the virtual environment:

  - **conda activate *napari-env***

- **“(napari-env)”** should now be indicated at the command line:

![Virtual environment syntax modified](images/install-5.png)

## Installation of napari 

## Launching napari after installation session
