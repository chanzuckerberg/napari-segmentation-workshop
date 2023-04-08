![Samples of images segmented by Cellpose](images/partseg-banner.png)
Classical segmentation with PartSeg
=======================
**By [Kasia Kedziora](https://chanzuckerberg.github.io/napari-segmentation-workshop/preface/whomadethis.html#katarzyna-kasia-kedziora) 🔬**

### Learning Objectives

In this lesson, you'll learn how to use and configure the PartSeg plugin in napari to complete a classical segmentation workflow. 

1.  [An introduction to classical segmentation](https://chanzuckerberg.github.io/napari-segmentation-workshop/workflow/partseg.html#what-is-a-classical-segmentation-pipeline)
2.  [Detecting and segmenting nuclei as individual objects](partseg-nuclei.md)
3.  [Detecting and segmenting foci as individual objects](partseg-foci.md)
4.  [Quantifying segmentation regions based on your masks](partseg-quantification.md)

- **Time to learn**: 1 hour

### Prerequisites

| Napari version and plugins                                                                     | Importance | Notes |
| -------------------------------------------------------------------------------- | ---------- | ----- |
| [napari v 0.4.15](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html) | Mandatory  | Tested with this napari version. Verify your version by going to the **Help** menu and choosing **napari info**. <!-- What if they have a different version, like 0.4.17? -->
| [PartSeg v 0.14.2](https://www.napari-hub.org/plugins/PartSeg) | Mandatory  | Install this plugin from within the napari viewer, by going to the **Plugin** menu, then clicking on **Install/uninstall plugins**. Search for *PartSeg* and click **install**. | |<!-- What if they have a different version, like 0.14.6? -->
| [Napari-segment-blobs-and-things-with-membranes v 0.2.22](https://www.napari-hub.org/plugins/napari-segment-blobs-and-things-with-membranes) | Mandatory  | Install this plugin from within the napari viewer, by going to the **Plugin** menu, then clicking on **Install/uninstall plugins**. Search for *Napari-segment-blobs-and-things-with-membranes* and click **install**. | |
| <center>**Sample data**</center> |  |  |
| [2D data used in lesson](https://github.com/chanzuckerberg/napari-segmentation-workshop/raw/main/content/workflow/images/cells_gh2ax.tif) | *Optional* |  | |

### What is a classical segmentation pipeline?

A classical segmentation pipeline is built around a thresholding algorithm to detect objects with intensities that vary from their surrounding background. It can be divided into 3 main parts:

- **preprocessing**: preparation of images for thresholding (e.g. filtering to remove noise).
- **thresholding**: finding an intensity value that separates objects from the background.
- **postprocessing**: a set of operations designed to refine the shape of detected objects.

### Video introduction to classical segmentation

<center>
<script src="https://fast.wistia.com/embed/medias/oogdwlg80o.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_oogdwlg80o seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/oogdwlg80o/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>
</center>

<br>

### Supporting materials
- [Image Analysis Primer](https://chanzuckerberg.github.io/napari-segmentation-workshop/preface/imageanalysis.html)
- [PartSeg documentation](https://partseg.readthedocs.io/en/stable/)
- [Developer site for PartSeg](https://plewczynski-lab.org/PartSeg/)
