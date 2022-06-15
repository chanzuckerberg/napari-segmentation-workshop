![Samples of images segmented by Cellpose](images/allencell-1.png)

Allen Cell Segmenter
=======================

## Learning Objectives

In this lesson, you'll learn how to use and configure the Allen Cell Segmenter plugin for napari to complete a segmentation workflow.

1.  [A walkthrough of the segmentation protocol, with napari screenshots](allencell-protocol.md)
2.  
3.  

- **Time to learn**: 1 hour

## Prerequisites

| Napari version and plugins                                                                     | Importance | Notes |
| -------------------------------------------------------------------------------- | ---------- | ----- |
| [napari v 0.4.14](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html) | Mandatory  | In the napari viewer, verify your version of napari by clicking on the **Help** menu, then **napari info**. | |
| [napari-allencell-segmenter v 1.1.4](https://www.napari-hub.org/plugins/cellpose-napari) | Mandatory  | Install this plugin from within the napari viewer, by going to the **Plugin** menu, then clicking on **Install/uninstall plugins**. Search for *napari-allencell-segmenter* and click **install**. | |
| <center>**Image inputs**</center> |  |  |
| Image stack (3D data: 8, 12, and 16 bit) | Mandatory  | In some cases, the plugin may return error messages when the image scale is imported incorrectly. When this occurs, remove any pixel scaling before repeating this step. | |
| <center>**Sample data**</center> |  |  |
| [Sample data used in lesson](https://github.com/chanzuckerberg/napari-segmentation-workshop/raw/main/content/workflow/images/Allen-Cell-Segmenter-Sample-Data.tif) | *Optional* | Although napari may support the importing of other file types, this sample image is a tiff. | |

## What does this plugin do?

The Allen Cell Segmenter is a napari plugin that consists of pre designed classical image segmentation workflow for many cellular components for **3D data**. You can choose which images most resemble your data and adjust parameters within the workflow steps to optimize the segmentation quality on your data.

## Demo of *Allen Cell Segmenter*

<center><script src="https://fast.wistia.com/embed/medias/388imsy9td.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_388imsy9td seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/388imsy9td/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div></center>

<br>
  
The above video demonstrates how to complete the [Allen Cell segmentation workflow](allencell-protocol.md) within the napari viewer; and also showcases how the adjusting of parameters affects the resulting segmentation.

## Supporting materials

- [Original Python code](https://www.allencell.org/segmenter.html#lookup-table)

- [“The Allen Cell Structure Segmenter: a new open source toolkit for segmenting 3D intracellular structures in fluorescence microscopy images”](https://www.biorxiv.org/content/10.1101/491035v1.full#F2)

- [Github documentation for Allen Cell Segmenter](https://github.com/AllenCell/napari-allencell-segmenter)

- [A detailed explanation of Allen Cell parameters](https://github.com/AllenCell/aics-segmentation/blob/main/lookup_table_demo/playground_filament3d.ipynb)
