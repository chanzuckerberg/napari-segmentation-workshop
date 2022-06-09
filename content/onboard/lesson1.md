![Picture of art installation of networked cables](images/header_small.jpeg)
What is napari?
=======================

## Learning Objectives

In this lesson, you'll learn what [napari](www.napari.org) is, how it works with Python, and some of the advantages of using open-source imaging tech. 

1.  At volutpat diam ut venenatis tellus in metus
2.  Sed elementum tempus egestas sed sed risus pretium

## Prerequisites

| Concepts                                                                         | Importance | Notes |
| -------------------------------------------------------------------------------- | ---------- | ----- |
| [Why Python?](https://foundations.projectpythia.org/foundations/why-python.html) | Helpful    |       |

- **Time to learn**: 20 minutes

:::{note}
This is a brief introduction to a new image analysis platform called napari. Although parts of napari are still undergoing development and some kinks are still being ironed out here and there, it can be a very useful tool for your image analysis, especially if you have complex, large, or multi-dimensional datasets.
:::

---

## Processing Multi-Dimensional Imaging Data

Napari is an open-source **graphical user interface**[^mynote], developed specifically for viewing, annotating, and analysing large and multi-dimensional imaging datasets.

In 2022, the increasingly massive datasets that modern imaging technologies (such as time lapse imaging, confocal microscopy, super-resolution microscopy, or light sheet microscopy) generate can be challenging for legacy tech to handle and analyze. More and more, scientists are turning to sophisticated, modern analytical tools and pipelines developed with programming languages such as Python or MatLab. 

The open-source nature of Python means it has been widely adopted, and there is a large and rapidly growing number of libraries of scientific resources and tools available for use with Python. However, these scripting-based approaches can often be difficult to adopt, especially without a graphical user interface and a way to visualize the image analysis processes.

[^mynote]: Any program you can interact with in a separate window, equipped with clickable buttons, tools, and other visual mechanisms. 

## The Power of Python

<iframe width="560" height="315" src="https://www.youtube.com/embed/VXdFOcBCto4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

At animi commodi aut dignissimos laudantium et voluptatem eveniet id deleniti voluptatibus dolorem quidem aut error repellat sed velit dolor. Est laudantium consectetur id nihil nostrum sed ducimus laudantium eos porro voluptate qui facere illum id debitis earum ut adipisci soluta.

:::{tip}
Morbi tincidunt ornare massa eget. Sit amet mattis vulputate enim nulla aliquet porttitor. Et netus et malesuada fames ac. Pulvinar mattis nunc sed blandit libero volutpat sed cras ornare.
:::

### The napari viewer

<iframe width="560" height="315" src="https://www.youtube.com/embed/sFvZcUeShoo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Et harum quisquam in consectetur quae accusantium cumque ut consequatur Quis et facere maxime qui quisquam unde. Sit optio natus in sunt pariatur ad magni distinctio. Non accusamus ratione non veniam nesciunt cum autem temporibus id quis quia vel dolore inventore ut nihil quia.

![image](images/napari-viewer.png)

## What can napari do? 

Ultricies mi eget mauris pharetra et. Lectus vestibulum mattis ullamcorper velit sed. Pellentesque habitant morbi tristique senectus et netus et malesuada.Vestibulum morbi blandit cursus risus at ultrices mi tempus imperdiet. Sit amet venenatis urna cursus eget. Sit amet purus gravida quis blandit turpis cursus in hac.

### Overview of napari

Vulputate enim nulla aliquet porttitor lacus. Elementum nibh tellus molestie nunc non blandit massa enim. Volutpat commodo sed egestas egestas fringilla phasellus faucibus. Amet consectetur adipiscing elit ut.

```{glossary}
Term one
  An indented explanation of term 1

A second term
  An indented explanation of term2
```

### napari layers

Vulputate enim nulla aliquet porttitor lacus. Elementum nibh tellus molestie nunc non blandit massa enim. Volutpat commodo sed egestas egestas fringilla phasellus faucibus. Amet consectetur adipiscing elit ut.

```{warning}
Maecenas sed enim ut sem viverra aliquet. Facilisis volutpat est velit egestas dui id. 
Erat nam at lectus urna. Lobortis scelerisque fermentum dui faucibus in ornare quam viverra orci.
```

### napari console

Lobortis feugiat vivamus at augue eget arcu. Massa placerat duis ultricies lacus sed. Elit ullamcorper dignissim cras tincidunt lobortis feugiat vivamus at augue. Vel pretium lectus quam id leo in vitae. Sit amet dictum sit amet justo donec. 

```python
from skimage import data
import napari

viewer = napari.view_image(data.cells3d(), channel_axis=1, ndisplay=3)
```

### Widgets and plugins

Est omnis adipisci est commodi provident aut dignissimos excepturi a delectus quia aut delectus fugiat qui nisi blanditiis a omnis dolore. At iure enim in voluptate unde At adipisci facere sit nesciunt iusto.

Ea assumenda dolorum et quaerat earum aut cumque culpa et dolores corrupti. Eos modi inventore est esse perferendis sed iste aliquid eum quia consequatur?

<iframe width="560" height="315" src="https://www.youtube.com/embed/9_Zo2sR75To" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Closeout

Sed doloremque voluptatibus eum quia facere est possimus illo ab quae facere qui asperiores dolorem sed nulla quasi ad tempore adipisci. Qui omnis beatae et esse minima ut nostrum dolorem et aliquam amet. Non enim maxime qui optio quia aut velit excepturi quo inventore laudantium.

Non placeat officia cum tempore officiis sit voluptate saepe ut magnam galisum sit quas consequatur. Ut asperiores cupiditate a aperiam dolorem est voluptatum molestiae a aliquid eveniet.
