![Picture of art installation of networked cables](images/header_small.jpeg)
Lesson II: Cellpose workflow for napari
=======================

## Overview & Learning Objectives

In this lesson, you'll learn how to use the Cellpose plugin for napari, paired with FIJI, to perform segmentation on an image. Subjects covered include: 

1.  Adjusting and understanding parameters in Cellpose
2.  Segmenting and exporting your image's mask in FIJI 

- **Time to learn**: 20 minutes

## Prerequisites

| Napari segmentation course                                                                        | Importance | Notes |
| -------------------------------------------------------------------------------- | ---------- | ----- |
| Stage I, Lesson III: [Getting started with napari](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html) | Mandatory  | (You installed napari successfully) | |

| Technical requirements                                                                  | Importance | Notes |
| -------------------------------------------------------------------------------- | ---------- | ----- |
| [napari v 0.4.14](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html) | (In the napari viewer, verify your version by clicking on the **Help** menu, then **napari info**) | |
| [Cellpose v 0.1.4]([https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html](https://www.napari-hub.org/plugins/cellpose-napari)) | |
| Input images | - tiffs or PNGs or JPEGs
                 - Single plane images that can be read *nY x nX x* or *x nY x nX*
                 - Multiplane images that can be read *nZ x nY x nX* | 

---

## 
