# Segmenting in napari, and exporting a mask to FIJI

## Workflow for 2D Segmentation

* Open your image in the napari viewer, with *cellpose-napari* enabled. 
* Select the appropriate cellpose parameters (uncheck **“Process stack as 3D”**).
* Run the segmentation.

## Workflow for 3D Segmentation

* Open your image in the napari viewer, with *cellpose-napari* enabled. 
* Select the appropriate cellpose parameters (check off **”Process stack as 3D”** OR use the **“stitch threshold slices”** option).
* Run the segmentation.

## Workflow for Time segmentation

* Open your image in the napari viewer, with *cellpose-napari* enabled. 
* Select the appropriate cellpose parameters (use the **“stitch threshold slices”** option with value >0).
* Run the segmentation.

## Export mask as TIF:

Convert the **“label layer”** into images by doing right click on it and select: **“Convert to image”**. Then, split it as individual images by right clicking and selecting **“Split Stack”** (3D and time Serie only). Then reconvert each image into a label by right clicking on it and selecting: **“Convert to label”**. Rename them (1 to X). Finally save each label as a tif.

![Converting your image to a tif in cellpose-napari](images/cellpose3.png)

<br>

![Split stack in cellpose-napari](images/cellpose4.png)

## Opening the mask in FIJI

Use the plugin BioFormat importer and select: **”group file with similar name”** (3D and time Serie only). In the pop-up window, select:”pattern”. Open normally for 2D mask. You will be able to display the raw image and the mask image side by side.

![Using the plugin BioFormat importer](images/cellpose5.png)

## Using the mask as a mask

Navigating to the main menu in FIJI, go to **process > binary > convert to mask > Yen**.

![Converting to a mask in FIJI](images/cellpose6.png)

Performing this Binarization step can also correct some segmentation issues. As we can see in the example above, cells were over segmented with cellpose in napari, but the binarization in FIJI corrects this. 

![Binarization in FIJI](images/cellpose7.png)

## Performing a 3D analysis

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/RCat0ylcSHw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center>

In FIJI, you may perform a 3D analysis of the your mask in one of two ways, as shown in the video above: 

* Analyze > 3D OC options > select measurements option
* Analyze > 3D object counter > fine tune if necessary 

![3D analysis in FIJI](images/cellpose8.png)
