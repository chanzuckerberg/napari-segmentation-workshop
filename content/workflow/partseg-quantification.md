# Quantification of segmented regions

As we approach the final steps of our workflow, napari gives us several options for quantification of regions based on the segmentation masks. Importantly, you can perform this quantification regardless of how the segmentation mask was created or loaded into the napari viewer. 

- If interested in a simple quantification check, look at the **Simple Measurement** tool in the PartSeg napari viewer widget. 

- For full flexibility of quantifying different classes of objects, look at the **Measurement** tool in the PartSeg napari viewer widget. 

## Simple measurements in PartSeg  
In this video we load the PartSeg widgets plugin and choose *Simple Measurement*. When the panel opens, choose the image we have been working with, [2D test data](https://github.com/chanzuckerberg/napari-segmentation-workshop/raw/main/content/workflow/images/cells_gh2ax.tif). Choose a **Label** and **Data units**. For this example, we choose to examine **Diameter**, **Mean pixel brightness**, and **Sphericity**.  Click **Calculate** to see a table of the results.  

<script src="https://fast.wistia.com/embed/medias/59hl61l69o.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_59hl61l69o seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/59hl61l69o/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>

:::{hint}
Some of the simple quantification based on segmented regions include the analysis of the shape of the objects (ex. area or sphericity - the measurement of how close to a circle the object is) or the analysis of the signal intensity within the regions (ex. mean or standard deviation of pixel intensities within the objects).
:::

## Full measurements in PartSeg  

This video is designed to  explore full measurements by calculating the properties of nuclei and foci and the relationship between the two. We select the PartSeg widgets plugin and choose the **Measurement** option. 
- Click the **Measurement settings** tab and create a name for this set of measurements in the **Set name:** field.  
- Select the properties you want to measure and specify for each one if they are per component or not. Per component means per a single region of interest (ROI) whether it is (in this case) focus or nucleus.  
- Click the arrow between the two boxes to save the properties you want to measure.  
  Optional: You can save these with custom parameter designations, which means you can create your own label for each property. These are the column headings for the output table.  
- Click the **Measurements** tab.  
    - **Channel:** is the image layer. for this example the  - **ROI** is foci, for this example  
    - **Mask:** is nuclei.  
    - Choose the **Measurement set:** that you previously defined.   
- Click **Recalculate and replace measurement**.  
- Optional: Choose **Horizontal view** by placing a checkmark in that box. 

<script src="https://fast.wistia.com/embed/medias/k0w5y27wiy.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_k0w5y27wiy seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/k0w5y27wiy/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>

:::{hint}
Having segmented more than one class of objects (ex. the nuclei and foci within them) we can separately quantify not only the properties of each class of objects, but also the relationships between them. For example, we can count how many foci belong to a given nucleus or combine measurements of the nuclei and foci into a single table of results. 
:::
