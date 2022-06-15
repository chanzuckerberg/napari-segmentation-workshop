# Protocol for segmentation workflow

## Launch napari, and import your image

- Begin by importing an image to be analyzed. You may either drag and drop your image directly into the napari viewer, or locate it on your computer using the menu **File >> Open**. 

:::{hint}
Before proceeding, ensure that the Builitins reader plugin is being used, to minimize errors. You can verify this by going to menu **File >> Preference >> Plugins**, then checking that **"Builitins reader plugin"** is enabled. 
:::

- In this instance, I've opened an image of actin filaments (which you can acquire for yourself [here](https://github.com/chanzuckerberg/napari-segmentation-workshop/raw/main/content/workflow/images/Allen-Cell-Segmenter-Sample-Data.tif)). 

![Sample data of actin filaments](images/allencell-2.png)

## Allen Cell Segmenter Workflow editor

- With your image loaded, go to the menu **Plugins >> napari-allencell-segmenter >> Workflow editor**. 

![Workflow editor for Allen Cell Segmenter in napari viewer](images/allencell-3.png)

## Step 1: Select your image to segment

- In the "Workflow selection steps" window that appears, click on the 1st drop down menu (#1), then select the image you imported previously. 

![Workflow editor image selection](images/allencell-4.png)

## Step 2: Select the channel to segment

- Moving to the dropdown menu below (#2), select the channel of your image that you wish to segment. 

![Workflow editor channel selection](images/allencell-5.png)

## Step 3: Select a comparable reference 

- In the final dropdown menu (#3, choose an image from the reference library that most matches the image you've selected to segment and analyze.

![Reference library of images in Allen Cell Segmenter](images/allencell-6.png)

- Using our [sample data](https://github.com/chanzuckerberg/napari-segmentation-workshop/raw/main/content/workflow/images/Allen-Cell-Segmenter-Sample-Data.tif)), we'll choose the last image in this library since it most matches our own. 

![Choosing a comparable image from the Allen Cell Segmenter reference library of images](images/allencell-7.png)

