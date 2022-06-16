![Samples of images segmented by Cellpose](images/allencell-1.png)

Allen Cell Segmenter
=======================
**By [Praju Anekal](https://chanzuckerberg.github.io/napari-segmentation-workshop/preface/whomadethis.html#praju-anekal) 🔬**
## Learning Objectives

In this lesson, you'll learn how to use and configure the Allen Cell Segmenter plugin for napari to complete a segmentation workflow.

1.  [A walkthrough of the segmentation protocol, with napari screenshots](allencell-protocol.md)
2.  [An explanation of parameters and effects, pertaining to *actin filaments*](allencell-parameters.md) 

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

The Allen Cell Segmenter consists of a *pre-designed* classical image segmentation workflow for many types of cellular components, and **3D data** sets. It allows you to choose your workflow from a library of images which most resemble your own data, and then adjust parameters within the workflow steps to optimize the segmentation quality of the data that results. 

The plugin workflow itself is broken into 3 discrete parts:
- **Preprocessing** >
- **Segmentation** > 
- **Post processing**

One of this plugin's core features is its ability to simplify a researcher's choice of workflows. When choosing your workflow, you will be presented with a library of similar-looking structures for you to compare and choose from. Clicking on one of these images will load the appropriate workflow. 

Once segmentation is completed, Allen Cell **outputs a segmented mask** which can be exported by napari, or analyzed by another napari plugin (e.g. [PartSeg](https://www.napari-hub.org/plugins/PartSeg)). 

:::{note}
Beyond these functions, Allen Cell Segmenter also has an **[iterative deep-learning](https://www.youtube.com/watch?v=W1DPfZk5iF8&t=8s)** component based on user-trained pixel classification (which is not within the scope of this lesson).
:::

## Demo of *Allen Cell Segmenter*

<center><script src="https://fast.wistia.com/embed/medias/388imsy9td.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_388imsy9td seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/388imsy9td/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div></center>

<br>
  
The above video demonstrates how to complete the [Allen Cell segmentation workflow](allencell-protocol.md) within napari, and also showcases how the adjusting of parameters affects the resulting segmentation.

## Supporting materials

- [Original Python code](https://www.allencell.org/segmenter.html#lookup-table)

- [“The Allen Cell Structure Segmenter: a new open source toolkit for segmenting 3D intracellular structures in fluorescence microscopy images”](https://www.biorxiv.org/content/10.1101/491035v1.full#F2)

- [Github documentation for Allen Cell Segmenter](https://github.com/AllenCell/napari-allencell-segmenter)

- [A detailed explanation of Allen Cell parameters](https://github.com/AllenCell/aics-segmentation/blob/main/lookup_table_demo/playground_filament3d.ipynb)

## Advanced materials 

- [Detailed video on the algorithms behind the Allen Cell Segmenter](https://www.youtube.com/watch?v=Ynl_Yt9N8p4)
