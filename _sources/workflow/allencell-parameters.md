# An explanation of parameters and their effects

:::{note}
The example below pertains to the segmentation of *actin filaments*. Options will vary depending on the [classical segmentation workflow](https://chanzuckerberg.github.io/napari-segmentation-workshop/workflow/allencell-protocol.html#step-3-select-a-comparable-reference) chosen within the Allen Cell napari plugin.
:::

## Pre-processing: Intensity normalization

Intended for scaling the intensity of the image between 0-1. The parameters themselves are **scaling_param 1** and **scaling_param 2**. These set the range from the **mean image intensity** to **normalised**. 

A mean image intensity is calculated for the image, then scaling_param 1 and 2 are substracted or added to the mean, setting the range that will be scaled from 0-1. 

![Mean intensity and scaling_parameters of Allen Cell Segmenter](images/allencell-10.png)

## Pre-processing: Edge preserving smoothing

## Core segmentation: Sigma

## Post-processing
