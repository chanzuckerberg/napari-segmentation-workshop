# Dannielle’s test page

This is a test page
[Image: Screen Shot 2022-02-22 at 9.16.48 AM.png]
* checklists look like this
* [napari hyperlink](https://www.napari-hub.org/)

>napari

```
20220307
#Create virtual environment
conda create --name bravo

#activate virtual environment
source activate bravo

#leave virtual environment
conda deactivate

#install this once in BASE environment to allow Jupyter to use other conda environments
conda install nb_conda_kernels

#install in each virtual environment to allow Jupyter to access it
conda install ipykernel

#ERROR: "error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun"
xcode-select --install
#xcode-select: note: install requested for command line developer tools

#clone a repository (copy URL from repository)
git clone https://github.com/chanzuckerberg/napari-segmentation-workshop.git

#enter cloned folder
cd napari-segmentation-workshop

#install requirements
pip install -r requirements.txt

#check for existing builds before building a book
jupyter-book clean content/

#build a book
jupyter-book build content/

```

1. items in a list
2. look like this
