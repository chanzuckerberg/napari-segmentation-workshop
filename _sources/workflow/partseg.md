![Samples of images segmented by Cellpose](images/Cellpose-banner.png)
Classical segmentation with PartSeg
=======================

## Learning Objectives

In this lesson, you'll learn how to use and configure the PartSeg plugin in napari to complete a classical segmentation workflow. 

1.  [Understanding the steps behind a classical segmentation](partseg-primer.md)
2.  [Learning how to perform segmentation using napari and plugins](partseg-nuclei.md)
3.  [Using elements of PartSeg and Napari-segment-blobs-and-things-with-membranes](partseg-quantification.md)

- **Time to learn**: 1 hour

## Prerequisites

| Napari version and plugins                                                                     | Importance | Notes |
| -------------------------------------------------------------------------------- | ---------- | ----- |
| [napari v 0.4.15](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html) | Mandatory  | Tested with this napari version. Verify your version by going to the **Help** menu and choosing **napari info**.
| [PartSeg v 0.14.2](https://www.napari-hub.org/plugins/PartSeg) | Mandatory  | Install this plugin from within the napari viewer, by going to the **Plugin** menu, then clicking on **Install/uninstall plugins**. Search for *PartSeg* and click **install**. | |
| [Napari-segment-blobs-and-things-with-membranes v 0.2.22](https://www.napari-hub.org/plugins/napari-segment-blobs-and-things-with-membranes) | Mandatory  | Install this plugin from within the napari viewer, by going to the **Plugin** menu, then clicking on **Install/uninstall plugins**. Search for *Napari-segment-blobs-and-things-with-membranes* and click **install**. | |
| <center>**Sample data**</center> |  |  |
| [2D data used in lesson](https://github.com/chanzuckerberg/napari-segmentation-workshop/raw/main/content/workflow/images/cells_gh2ax.tif) | *Optional* |  | |

## What is a classical segmentation pipeline?

A classical segmentation pipeline is built around a thresholding algorithm to detect objects which intensity vary from the surrounding background. It can be divided into 3 main parts:

- **preprocessing**: preparation of images for thresholding (ex. filtering to remove noise).
- **thresholding**: finding an intensity value that separates objects from the background.
- **postprocessing**: a set of operations designed to refine the shape of detected objects.


## Short introductiion to classical segmentation

<center>
<script src="https://fast.wistia.com/embed/medias/ezh7e1nqr1.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_ezh7e1nqr1 seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/ezh7e1nqr1/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>
</center>

<br>
  
The above video demonstrates...
