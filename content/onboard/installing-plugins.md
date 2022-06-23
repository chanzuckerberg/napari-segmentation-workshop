Installing napari plugins
=======================
**By [Bryan Millis](https://chanzuckerberg.github.io/napari-segmentation-workshop/preface/whomadethis.html#bryan-millis) 🔬**
## Learning Objectives

In this lesson, you'll learn how plugins relate to napari, and how to install, enable, and update them from within the napari viewer. 

1.  [Why do we need plugins?](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/gettingstarted.html#installation-of-python-via-an-environment-manager)
2.  [Revisiting virtual environments](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/gettingstarted-2.html#creating-a-virtual-environment)
3.  [Installing plugins in the napari viewer](https://github.com/chanzuckerberg/napari-segmentation-workshop/blob/main/content/onboard/gettingstarted-2.md#creating-a-virtual-environment)
4.  [Use case for installing a plugin](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/gettingstarted-2.html#installation-of-napari)
5.  [Updating plugins](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/gettingstarted-2.html#launching-napari-after-installation-session)

- **Time to learn**: 1 hour

| Napari version and plugins                                                                     | Importance | Notes |
| -------------------------------------------------------------------------------- | ---------- | ----- |
| [What is napari?](whatisnapari.md) | Mandatory  | You'll learn what napari is, how Python ties into it, and why you'd want to use it. | |
| [Getting started with napari](gettingstarted.md) | Mandatory  | A detailed walkthrough of how to successfully install napari.  | |

## Video walkthrough

<script src="https://fast.wistia.com/embed/medias/j0644yvc89.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_j0644yvc89 seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/j0644yvc89/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>

## Why do we need napari plugins? 

As a new user, you may be wondering why programs such as napari require plugins to use certain functions, or even complete segmentation workflows. There are many reasons for this, but two of the most common ones are: 

- By providing a core viewer without any pre-installed plugins, napari allows users to enjoy a so-called **“light-weight” installation**, thereby minimizing burden on machines. Given the number of plugins available, the fact that researchers use a select few at a time, and the varying performance capabilities of computers in lab cores around the world, this begins to make all the more sense. 

- When installed, each plugin brings with it an associated package of files (i.e. particular Python coding libraries). Although several plugins may share the the same libraries (or dependencies), the versions of these libraries may not always be the same.

  - e.g. Plugin A may require the newest version of a particular Python library to be functional, while Plugin B may only be compatible with the older build of that same library. Were many plugins like this pre-installed together, management of these different dependencies would get frustrating quickly. By having users install and enable plugins on a case-by-case basis, napari minimizes compatibility issues across the board. 

:::{hint} 
It's always good to remember, whenever using an open-source program with a constantly-evolving repository of plugins, that the relative “maturity” of a plugin can widely vary. Some plugins may be more intuitive to install and use, some may be well-documented, while others mays not. 
:::

## Revisiting virtual environments

Having addressed the subject of plugin dependencies, this is a good time to revisit the concept of [virtual environments](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/gettingstarted.html#installation-of-python-via-an-environment-manager). Not only do virtual environments keep particular installations "contained," but they also allow you to create (or delete) multiple virtual environments, each with different installations or sets of plugins, fitting specific types of analyses.

## Installing plugins in the napari viewer

:::{note} 
We assume you've already [installed napari](gettingstarted.md) and understand how to activate virtual environments, having completed the prerequisite lesson. 
:::

- Activate the virtual environment you have napari installed into, and launch napari.
  - e.g. **conda activate napari-env**
  - **napari**

- Once napari has launched, find the Plugins menu and click **"Install/Uninstall plugins"** in the dropdown that appears. 

- In the subsequent window, you'll see a list of all the plugins that were previously installed, as well as a list of plugins that are available to be installed. 

:::{hint} 
While you are welcome to scroll through these lists of plugins, it may be more efficient to use the **filter** field above to search for plugins by keywords related to their names or functions. 
:::

## Use case: Installing plugins to open vendor-specific file types

- Let’s say you need to open a dataset acquired on a commercial system with a file type native to that particular system (e.g. Nikon .nd2, Zeiss .czi, Leica .lif, Olympus .oif, etc.)

- When attempting to drop-and-drag one of these file types into the napari viewer, you notice the following error, alerting us that no current plugin exists to open the file:

- Heading to the Plugins menu, click **"Install/Uninstall plugins"**, and then search for “nd2” in the filter field above the list of plugins. 

- Here we see a plugin titled, “napari-nikon-nd2”, which seems appropriate. By clicking the blue **“install”** button to the right of it, we can add it to our list of installed plugins:

:::{note} 
Just because a plugin has been installed, does not mean it has been enabled! To enable/disable a plugin, toggle the checkbox next to the plugin. 
:::

- After installing and enabling the **"napari-nikon-nd2"**, and attempting to open the same [.nd2] dataset again, we are successful!

- Of course, not all plugin installations are so smooth. Depending on their state of development, some may have error messages or bugs that pop up. This is why it is important to visit the [napari hub](https://www.napari-hub.org) and read the available documentation on any plugin of interest in order to review any suggested installation notes that would differ from the aforementioned.

## Updating plugins

- Periodically, updates to installed plugins may become available. When such an update is available, it will be displayed in the “Install/Uninstall Plugins” window as seen below: 
