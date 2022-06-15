What is napari?
=======================
**By [Caron Jacobs](https://chanzuckerberg.github.io/napari-segmentation-workshop/preface/whomadethis.html#caron-jacobs) 🔬**
## Learning Objectives

In this lesson, you'll learn what [napari](https://www.napari.org) is, its relationship with the Python coding language, and some of the advantages of using open-source imaging tech. 

1.  [Processing multi-dimensional imaging data](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/whatisnapari.html#processing-multi-dimensional-imaging-data)
2.  [Accessibility of napari](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/whatisnapari.html#accessibility-of-napari)

![Picture of art installation of networked cables](images/napari-viewer.gif)

- **Time to learn**: 20 minutes

:::{note}
This is a brief introduction to a new image analysis platform called napari. Although parts of napari are still undergoing development and some kinks are still being ironed out here and there, it can be a very useful tool for your image analysis, especially if you have complex, large, or multi-dimensional datasets.
:::

---

## Processing multi-dimensional imaging data

Napari is an open-source **graphical user interface**[^mynote], developed specifically for viewing, annotating, and analysing large and multi-dimensional imaging datasets.

In 2022, the increasingly massive datasets that modern imaging technologies (such as time lapse imaging, confocal microscopy, super-resolution microscopy, or light sheet microscopy) generate can be challenging for legacy tech to handle and analyze. More and more, scientists are turning to sophisticated, modern analytical tools and pipelines developed with programming languages such as Python or MatLab. 

The open-source nature of Python means it has been widely adopted, and there is a large and rapidly growing number of libraries of scientific resources and tools available for use with Python. However, these scripting-based approaches can often be difficult to adopt, especially without a graphical user interface and a way to visualize the image analysis processes.

[^mynote]: Any program you can interact with in a separate window, equipped with clickable buttons, built-in tools, and other visual mechanisms. 

:::{hint}
Napari’s utility is certainly not limited to handling large datasets. The Python basis of napari means that many useful packages can be made available for a range of simple or complex data processing and analysis tasks.
:::

## The power of Python

Napari is built on the Python coding language, intending to bridge the gap between the inherently visual nature of image analysis and the computational power available through Python and its libraries. This includes, for example, being able to leverage the speed of GPU-based computing and machine learning for large and complex processes, such as content-aware denoising, handling of light-sheet microscope data, or even challenging segmentation cases! 

## Accessibility of napari

Napari aims to minimize (and eventually eliminate) the amount of coding knowledge needed for its use, making it friendly for life-science based fields, students and educators. However as napari is still being developed and evolving as a platform, the current version (as of June 2022) requires some user understanding of the basics of: **conda**, **python**, and **virtual environments**. Core developers are aiming for a “plug-and-play”, pre-built version that can be downloaded and installed like any desktop app or software you’re accustomed to using. 

:::{hint}
Although [this executable](https://napari.org/tutorials/fundamentals/quick_start.html#installation) exists, we recommend against using it if you intend to perform cell segmentations with napari, because it is still in-development and not entirely stable. 
:::

### Open-source adaptability

Napari is free-to-use, **open-source** and **community-developed**. This means that napari’s arsenal of tools will continue to develop in tandem with the needs of its users, and as new technologies and methodologies become available. These tools are made available as **plugins**[^mynote2] – analytical processes or pipelines packaged together as software components that you can download and “add-on” to your napari installation. These pipelines then become available in the napari viewer and they can be enabled and interacted with through its user-friendly GUI.

[^mynote2]: Installable add-ons for the napari viewer which enhance its image analysis capabilities. Discoverable in napari viewer or the [napari hub](https://www.napari-hub.org). 

## Interoperability of napari

Napari is also interoperable with other image analysis platforms, such as Fiji - common file formats such as .tiffs and hdf5 are compatible with almost all platforms. These different platforms have a lot of common functionality, but you may also find key differences in some functions availability (or capability). 

Different platforms may also have different ways of allowing you to interact with the data, that may suit different points in an analysis pipeline. Especially in light of the fact that napari is still in its alpha development stage, there are some functions that are not yet stable or available in napari.

## Supporting materials

### Official napari documentation

- [Napari.org 'Quick Start'](https://napari.org/tutorials/fundamentals/quick_start.html)

### Community pages for napari

- [CZI napari landing page](https://chanzuckerberg.com/napari-a-multi-dimensional-image-viewer-for-python/)
- [Image.SC forum for napari](https://forum.image.sc/tag/napari)

### Introduction from core dev

<br><center><iframe width="560" height="315" src="https://www.youtube.com/embed/VXdFOcBCto4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center> <br>


