# Segmentation of nuclei

To begin the workflow, start by **detecting cell nuclei** as individual objects. Cell nuclei in a fluorescence image are clearly brighter than the surrounding background so, many automated thresholding algorithms will successfully find the correct thresholding values. We will add several post-processing steps to make sure that the edges of the detected nuclei are smooth and that the small bright particles in the background are not mistakenly classified as nuclei.

<script src="https://fast.wistia.com/embed/medias/ogftgh3nwb.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_ogftgh3nwb seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/ogftgh3nwb/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>

### PartSeg: ROI Mask Extraction parameters
Here is a sample exercise that shows how setting the parameters allows you to find the nuclei. Assuming you have loaded the [2D test data](https://github.com/chanzuckerberg/napari-segmentation-workshop/raw/main/content/workflow/images/cells_gh2ax.tif) into napari. You should also have the partseg plugin installed. To use it go to **Plugins>Install/Uninstall Plugins>partseg** and choose the **ROI Mask Extraction** option. A panel will appear on the right side of napari as shown below.   
#### Pre-processing settings <- This heading does not appear on the screen but these parameters set up the pre-processing.  
- **Target layer name:** *nuclei* (or the name of your choice)  
- In the dropdown below the *Run* button, select *Threshold*  
- **Channel**: the name of the image layer you are thresholding  
- **Filter**: *Median*    
- **Median type**: *Layer* (for 3D data, choose *Stack*)  
- **Median radius**: *2*       

![roi-mask-extraction-partseg-pre-processing](.\images\roi-mask-extraction-partseg-pre-processing.png)  

#### Thresholding settings <- This heading does not appear on the screen but these parameters set up the thresholding.   
-**Threshold**: *Otsu*  
-**Apply mask**: should be checked    
-**Histogram bins**: *128*    

![roi-mask-extraction-partseg-thresholding](.\images\roi-mask-extraction-partseg-thresholding.png)  

#### Post-processing settings <- This heading does not appear on the screen but these parameters set up the post-processing.   
-**Fill holes**: should be checked  
-**Maximum holes size (px)**: *100*    
-**Smooth borders**: *Opening*    
-**Smooth borders radius**: *5*  
-**Side by side connections**: should be checked  
-**Minimum size**: *400*  
-**Use convex hull**: *1*  
  
![roi-mask-extraction-partseg-post-processing](.\images\roi-mask-extraction-partseg-post-processing.png)  

Once all the parameters are set you can choose to save them at the top of this panel. Then click run to see the effect of these settings. Of course, you can change them and re-run partseg to see how the parameters affect the segmentation. 
