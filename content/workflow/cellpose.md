![Samples of images segmented by Cellpose](images/Cellpose-banner.png)
Cellpose-napari + FIJI
=======================
**By [Frederic Bonnet](https://chanzuckerberg.github.io/napari-segmentation-workshop/preface/whomadethis.html#frederic-bonnet) 🔬**
## Learning Objectives

In this lesson, you'll learn how to use the Cellpose napari plugin in conjunction with FIJI to complete a segmentation workflow.

1.  [Loading an image correctly in *Cellpose-napari*](cellpose-parameters.md)
2.  [Understanding and adjusting parameters in Cellpose](cellpose-parameters.md)
3.  [Segmenting and exporting your image's mask in FIJI](cellpose-FIJI.md)

- **Time to learn**: 1 hour

## Prerequisites

| Napari version and plugins                                                                     | Importance | Notes |
| -------------------------------------------------------------------------------- | ---------- | ----- |
| [napari v 0.4.17](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html) | Mandatory  | In the napari viewer, verify your version of napari by clicking on the **Help** menu, then **napari info**. | |
| [cellpose v 0.1.4](https://www.napari-hub.org/plugins/cellpose-napari) | Mandatory  | Install this plugin from within the napari viewer, by going to the **Plugin** menu, then clicking on **Install/uninstall plugins**. Search for *Cellpose-napari* and click **install**. | |
| [FIJI](https://imagej.net/software/fiji/) | Mandatory  | | |
| [Bio Formats for Image J/FIJI](https://imagej.net/formats/bio-formats) | Mandatory  | Allows us to open our image's mask in FIJI.| |
| <center>**Image inputs**</center> |  |  |
| tiffs, JPEGs or PNGs | Mandatory  | Any of these three file types will be supported | |
| Single plane images | *Optional*  | Channels can be read as: (**nY x nX x**) or (**x nY x nX**)| |
| Multiplane images | *Optional*  | Required image shape: (**nZ x nY x nX**)  | |
| Multichannel images, like multi-Z tiffs | *Optional*  | The expected format: (**nZ x nC x nY x nX**) | |
| <center>**Sample data**</center> |  |  |
| [2D data used in lesson](https://github.com/chanzuckerberg/napari-segmentation-workshop/raw/main/content/workflow/images/napari-Cellpose.tif) | *Optional* | Because this is 2D data, only 2D segmentation may be applied to it. | |

## What does this plugin do?

*Cellpose-napari* utilizes a generalist algorithm for cell and nucleus segmentation. It allows you to perform segmentation workflows on **cell bodies**, **membranes** and **nuclei** in images. It also has deep-learning built-in, allowing it to segment many types of cells without requiring parameter adjustments, new training data, or further model retraining. Because of its versatility, it supports a wide variety of microscopy modalities and fluorescent markers.

## Demo of *Cellpose-napari*

<center>
<script src="https://fast.wistia.com/embed/medias/ezh7e1nqr1.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_ezh7e1nqr1 seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/ezh7e1nqr1/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>
</center>

<br>
  
The above video demonstrates how to open the *Cellpose-napari* plugin, segment your image, and adjust its parameters. If you would like a more detailed [explanation of each parameter](cellpose-parameters.md), proceed to the next part of this lesson. 
  
:::{note}
Because napari can't export an image's mask at this time, we must use FIJI for this. The final part of this lesson covers [segmenting your image](cellpose-FIJI.md) with *cellpose-napari*, then using FIJI to export and analyze your image's mask. 
:::

## Supporting materials

- [Cellpose documentation site](https://cellpose.readthedocs.io/en/latest/)

- [Image J profile for Trackmate-Cellpose](https://imagej.net/plugins/trackmate/trackmate-cellpose)

- [Github page for Cellpose](https://github.com/mouseland/cellpose)

- ["Cellpose: a generalist algorithm for cellular segmentation" from Nature](https://www.nature.com/articles/s41592-020-01018-x.epdf?)
