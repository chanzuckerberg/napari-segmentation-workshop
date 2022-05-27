![Samples of images segmented by Cellpose](images/Cellpose-banner.png)
Cellpose-napari + FIJI
=======================

## Learning Objectives

In this lesson, you'll learn how to use and configure the Cellpose plugin for napari, in conjunction with FIJI, to complete a segmentation workflow.

1.  [Loading an image correctly in *Cellpose-napari*](workflow/cellpose-parameters.md)
2.  [Understanding and adjusting parameters in Cellpose](workflow/cellpose-parameters.md)
3.  [Segmenting and exporting your image's mask in FIJI](workflow/cellpose-FIJI.md)

- **Time to learn**: 1 hour

## Prerequisites

| Napari version and plugins                                                                     | Importance | Notes |
| -------------------------------------------------------------------------------- | ---------- | ----- |
| [napari v 0.4.14](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html) | Mandatory  | In the napari viewer, verify your version of napari by clicking on the **Help** menu, then **napari info**. | |
| [cellpose v 0.1.4](https://www.napari-hub.org/plugins/cellpose-napari) | Mandatory  | Install this plugin from within the napari viewer, by going to the **Plugin** menu, then clicking on **Install/uninstall plugins**. Search for *Cellpose-napari* and click **install**. | |
| [FIJI](https://imagej.net/software/fiji/) | Mandatory  | | |
| [Bio Formats for Image J/FIJI](https://imagej.net/formats/bio-formats) | Mandatory  | Allows us to open our image's mask in FIJI.| |
| <center>**Image inputs**</center> |  |  |
| tiffs, JPEGs or PNGs | Mandatory  | Any of these three file types will be supported | |
| Single plane images | *Optional*  | Channels can be read as: (**nY x nX x**) or (**x nY x nX**)| |
| Multiplane images | *Optional*  | Required image shape: (**nZ x nY x nX**)  | |
| Multichannel images, like multi-Z tiffs | *Optional*  | The expected format: (**nZ x nC x nY x nX**) | |

## What does this plugin do?

*Cellpose-napari* utilizes a generalist algorithm for cell and nucleus segmentation. It allows you to perform segmentation workflows on **cell bodies**, **membranes** and **nuclei** from microscopy images. It also has deep-learning built-in, allowing it to segment many types of cells without requiring parameter adjustments, new training data or further model retraining. Because of its versatility, it supports a wide variety of microscopy modalities and fluorescent markers.

## Supporting materials

- [Cellpose documentation site](https://cellpose.readthedocs.io/en/latest/)

- [Image J profile for Trackmate-Cellpose](https://imagej.net/plugins/trackmate/trackmate-cellpose)

- [Github page for Cellpose](https://github.com/mouseland/cellpose)

- ["Cellpose: a generalist algorithm for cellular segmentation" from Nature](https://www.nature.com/articles/s41592-020-01018-x.epdf?)
