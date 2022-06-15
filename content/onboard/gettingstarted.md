Getting started with napari
=======================
**By [Bryan Millis](https://chanzuckerberg.github.io/napari-segmentation-workshop/preface/whomadethis.html#bryan-millis) 🔬**
## Learning Objectives

In this lesson, you'll learn how to install napari with *minimal coding*, how virtual environments tie into installation, to launching napari for the first time. 

1.  [Installing a Python distribution](cellpose-parameters.md)
2.  [Creating a new virtual environment](cellpose-parameters.md)
3.  [Activating a new virtual environment](cellpose-FIJI.md)
4.  [Installing napari](blahblah)
5.  [Launching napari](blahblah)

- **Time to learn**: 1 hour

## Video Introduction

<script src="https://fast.wistia.com/embed/medias/j0644yvc89.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_j0644yvc89 seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/j0644yvc89/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>

## Introduction to napari's Python requirements

Like every software package out there, napari is written with a programming language. For example, Windows is based in *C*, various statistics programs are written in *R*, and ImageJ is based on *Java*. Napari is written with a language called *Python*. 

Python is a widely popular scientific computing language with many years of contributions under its belt. As such, there are multitudes of tools (and algorithms) that a program like napari can leverage to accomplish its tasks. Python, by default, is not pre-installed on most computers, and one needs to manually install it in order to execute Python-based programs.  

Although this is likely to change in the future, there is no “quick install” of napari (and its requisite Python coding language). Here we walk through the steps necessary for doing so, including getting Python installed on your machine, and subsequently the individual commands necessary for installing napari itself. This particular tutorial will focus on installing the aforementioned on a Windows machine. 

## Installation of Python via an environment manager

To be clear, there are several ways one could install Python on your machine. For example, one could visit the [Python website](https://www.python.org/) to install solely the Python language itself. However, installation through something known as an **environment manager**, will be quite helpful as we both install, and then utilize a program like napari, particularly because it’s a program early in its development, with many evolving parts.  

The environment manager we’ll detail below is through a distribution called “miniconda”—a lightweight distribution of the Python coding language along with a few essential packages. It will also enable us to later install napari into what is known as a **virtual environment**. Technically, it is also a **package manager**, but we’ll discuss that in a bit. 

The concept of a virtual environment can be understood as a contained place, or sandbox, where both a program and its various dependencies (other related files required for elements of a program to run) are installed. This is extremely helpful, especially for programs in active development, as environments can be created and deleted at will (if for example, there was a corruption, or bug that was hard to track down).

## Steps to install miniconda

- Visit the official [conda site](conda.io).
- Locate the link for miniconda. 

![Link to download miniconda](images/installation-1.png)



