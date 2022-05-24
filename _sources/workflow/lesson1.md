![Picture of art installation of networked cables](images/header_small.jpeg)
Lesson I: Introduction to cell segmentation
=======================

## Overview & Learning Objectives

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

1.  At volutpat diam ut venenatis tellus in metus
2.  Sed elementum tempus egestas sed sed risus pretium

- **Time to learn**: 20 minutes

## Prerequisites

| Napari segmentation course                                                                             | Importance | Notes |
| -------------------------------------------------------------------------------- | ---------- | ----- |
| Stage I, Lesson III: [Getting started with napari](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html) | Mandatory  | (You installed napari successfully) | |
| Stage I, Lesson IV: [Napari plugins](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson4.html) | Mandatory  | (You installed plugins successfully)      | |
| Stage II: [Digital images as "arrays of numbers"](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html) | Helpful  |  | |
| Stage II: [Dimensionality of digital images](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson4.html) | Helpful  |    | |
| Stage II: [Deep learning or A.I in image analysis](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson4.html) | Helpful  |   | |
| Stage II: [Bit depth](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson4.html) | Helpful  |     | |

After learning [what napari is](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson1.html) and what it can do for you, [how to install it on your machine](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/lesson3.html), and some of the [fundamentals of image analysis](https://chanzuckerberg.github.io/napari-segmentation-workshop/primer/lesson1.html), you're now ready to tackle the "segmentation problem" as we like to call it. 

---

## Defining the "segmentation problem" to solve

Pellentesque sit amet porttitor eget dolor. Sit amet nisl suscipit adipiscing bibendum est ultricies. Malesuada fames ac turpis egestas maecenas pharetra. Quam elementum pulvinar etiam non quam lacus suspendisse faucibus.

### Inputs and Outputs

Facilisi cras fermentum odio eu feugiat pretium nibh. Dictumst vestibulum rhoncus est pellentesque elit ullamcorper dignissim. Justo nec ultrices dui sapien eget. Ac ut consequat semper viverra nam libero justo. Laoreet id donec ultrices tincidunt. Consectetur adipiscing elit duis tristique sollicitudin nibh sit.

:::{tip}
Morbi tincidunt ornare massa eget. Sit amet mattis vulputate enim nulla aliquet porttitor. Et netus et malesuada fames ac. Pulvinar mattis nunc sed blandit libero volutpat sed cras ornare.
:::

### Section 1.2

(Sem nulla pharetra diam sit amet. Dolor sit amet consectetur adipiscing elit. Sit amet risus nullam eget felis. Phasellus egestas tellus rutrum tellus pellentesque eu tincidunt. Urna et pharetra pharetra massa massa ultricies mi quis hendrerit.)

Ultricies mi eget mauris pharetra et ultrices neque ornare:

```python
from skimage import data
import napari

viewer = napari.view_image(data.cells3d(), channel_axis=1, ndisplay=3)
```

![image](images/napari-viewer.png)

## Processing steps to segmentation

Ultricies mi eget mauris pharetra et. Lectus vestibulum mattis ullamcorper velit sed. Pellentesque habitant morbi tristique senectus et netus et malesuada.Vestibulum morbi blandit cursus risus at ultrices mi tempus imperdiet. Sit amet venenatis urna cursus eget. Sit amet purus gravida quis blandit turpis cursus in hac.

### Step 1

Vulputate enim nulla aliquet porttitor lacus. Elementum nibh tellus molestie nunc non blandit massa enim. Volutpat commodo sed egestas egestas fringilla phasellus faucibus. Amet consectetur adipiscing elit ut.

#### Basic explanation

Parturient montes nascetur ridiculus mus mauris vitae ultricies. Elementum curabitur vitae nunc sed velit dignissim. Odio ut sem nulla pharetra diam. Arcu cursus euismod quis viverra nibh cras pulvinar mattis nunc.

#### In-depth explanation

Nisl rhoncus mattis rhoncus urna neque viverra justo. Ultrices neque ornare aenean euismod elementum. Ac felis donec et odio pellentesque diam volutpat. Lobortis elementum nibh tellus molestie. Pellentesque elit ullamcorper dignissim cras tincidunt lobortis. Massa eget egestas purus viverra accumsan in. Phasellus vestibulum lorem sed risus. Cum sociis natoque penatibus et magnis dis parturient montes. Interdum consectetur libero id faucibus nisl tincidunt eget nullam.

### Step 2

Vulputate enim nulla aliquet porttitor lacus. Elementum nibh tellus molestie nunc non blandit massa enim. Volutpat commodo sed egestas egestas fringilla phasellus faucibus. Amet consectetur adipiscing elit ut.

#### Basic explanation

Consectetur adipiscing elit pellentesque habitant morbi tristique senectus. Praesent elementum facilisis leo vel. Integer quis auctor elit sed vulputate mi. At tellus at urna condimentum mattis. Eget dolor morbi non arcu risus. 

#### In-depth explanation

Neque laoreet suspendisse interdum consectetur libero id. Amet facilisis magna etiam tempor orci eu. Eu augue ut lectus arcu. Id eu nisl nunc mi ipsum. Commodo quis imperdiet massa tincidunt nunc pulvinar sapien. Bibendum ut tristique et egestas quis. Sapien pellentesque habitant morbi tristique. Arcu cursus euismod quis viverra nibh cras pulvinar mattis nunc. Sodales ut eu sem integer vitae justo. 

```{warning}
Maecenas sed enim ut sem viverra aliquet. Facilisis volutpat est velit egestas dui id. 
Erat nam at lectus urna. Lobortis scelerisque fermentum dui faucibus in ornare quam viverra orci.
```
### Step 3

Lobortis feugiat vivamus at augue eget arcu. Massa placerat duis ultricies lacus sed. Elit ullamcorper dignissim cras tincidunt lobortis feugiat vivamus at augue. Vel pretium lectus quam id leo in vitae. Sit amet dictum sit amet justo donec. 

#### Basic explanation

In nulla posuere sollicitudin aliquam ultrices sagittis. Adipiscing at in tellus integer feugiat scelerisque varius morbi. Magna fermentum iaculis eu non diam. Cras pulvinar mattis nunc sed blandit libero. Nunc id cursus metus aliquam. Etiam tempor orci eu lobortis elementum. Nulla facilisi etiam dignissim diam quis enim lobortis scelerisque. Magna eget est lorem ipsum dolor sit amet consectetur adipiscing. Augue mauris augue neque gravida.

#### In-depth explanation

Eros in cursus turpis massa tincidunt dui. Porttitor eget dolor morbi non arcu risus quis varius quam. Libero nunc consequat interdum varius sit amet mattis vulputate enim. Est ullamcorper eget nulla facilisi. Sociis natoque penatibus et magnis dis. Pellentesque nec nam aliquam sem.

<iframe width="560" height="315" src="https://www.youtube.com/embed/sFvZcUeShoo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Bonus: Writing loops in Python

Lobortis feugiat vivamus at augue eget arcu. Massa placerat duis ultricies lacus sed. Elit ullamcorper dignissim cras tincidunt lobortis feugiat vivamus at augue. Vel pretium lectus quam id leo in vitae. Sit amet dictum sit amet justo donec. 

````{tabbed} c++

```{code-block} c++

int main(const int argc, const char **argv) {
  return 0;
}
```
````

````{tabbed} python

```{code-block} python

def main():
    return
```
````

````{tabbed} java

```{code-block} java

class Main {
    public static void main(String[] args) {
    }
}
```
````

````{tabbed} julia

```{code-block} julia

function main()
end
```
````

````{tabbed} fortran

```{code-block} fortran

PROGRAM main
END PROGRAM main
```
````
## Lesson Glossary

```{glossary}
Threshold
  An indented explanation of term 1
  
Auto threshold
  An indented explanation of term2   

Pixel
  An indented explanation of term2
  
Pixel size
  An indented explanation of term2  
  
Voxel
  An indented explanation of term 1

Mask
  An indented explanation of term2
  
ROI
  An indented explanation of term 1
  
Bit depth
  An indented explanation of term 1

Processing filters
  An indented explanation of term2  
  
Binary filters
  An indented explanation of term2    
  
Machine learning and deep learning
  An indented explanation of term2   
  
Digital image
  An indented explanation of term2  
  ```
  
## Further Readings

### Basics of Bioimage Analysis

<br><center><iframe width="560" height="315" src="https://www.youtube.com/embed/1xo4vi6Ub4I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center>

### Introduction to Bioimage Analysis 

[Jupyter Book by Peter Bankhead](https://bioimagebook.github.io/README.html)

### Introduction to Image Segmentation

[ImageJ Community Wiki](https://imagej.net/imaging/segmentation)

## Next Steps 
