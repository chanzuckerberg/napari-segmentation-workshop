# Segmentation of foci

In this second part of our workflow, we want to **detect foci within the nuclei** as individual objects. Foci are much smaller than nuclei and so their brightness is more heterogeneous in nature. Additionally, they belong to nuclei that can be brighter or darker, so this segmentation proves challenging--even more challenging than the segmentation of the nuclei themselves as they all share a relatively dark (i.e. low signal) background.

<script src="https://fast.wistia.com/embed/medias/2ky32y2rhd.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_2ky32y2rhd seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/2ky32y2rhd/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>

### Analysis pipeline steps

#### Napari-segment-blobs-and-things-with-membranes

- Gaussian Laplace filter

#### PartSeg: ROI analysis extraction parameters

- Mask (nuclei)
- Manual Threshold (-2)
- Size restriction (>3)
- Connect by side
