# Quantification of segmented regions

As we approach the final steps of our workflow, napari gives us several options for quantification of regions based on the segmentation masks. Importantly, you can perform this quantification regardless of how the segmentation mask was created or loaded into the napari viewer. 

If interested in a simple quantification check, check the **Simple Measurement** tool in the PartSeg napari viewer widget. 

For full flexibility of quantifying different classes of objects, check the **Measurement** tool in the PartSeg napari viewer widget. 

## Simple measurements in PartSeg

<script src="https://fast.wistia.com/embed/medias/59hl61l69o.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_59hl61l69o seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/59hl61l69o/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>

:::{note}
Some of the simple quantification based on segmented regions include the analysis of the shape of the objects (ex. area or sphericity - the measurement of how close to a circle the object is) or the analysis of the signal intensity within the regions (ex. mean or standard deviation of pixel intensities within the objects).
:::
