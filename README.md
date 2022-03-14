# napari Segmentation Course

Course materials for biologists performing cell segmentation in napari

Site here: https://chanzuckerberg.github.io/napari-segmentation-workshop/

## Usage

### Building the book

If you'd like to develop and/or build the napari Segmentation Course book, you should:

1. Clone this repository
2. Run `pip install -r requirements.txt` (it is recommended you do this within a virtual environment)
3. (Optional) Edit the books source files located in the `content/` directory
4. Run `jupyter-book clean content/` to remove any existing builds
5. Run `jupyter-book build content/`

A fully-rendered HTML version of the book will be built in `content/_build/html/`.

## Code of Conduct

This project adheres to the Contributor Covenant [code of conduct](https://github.com/chanzuckerberg/.github/blob/master/CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to [opensource@chanzuckerberg.com](mailto:opensource@chanzuckerberg.com).

## Reporting Security Issues

If you believe you have found a security issue, please responsibly disclose by contacting us at [security@chanzuckerberg.com](mailto:security@chanzuckerberg.com).

## Credits

This project is created using the excellent open source [Jupyter Book project](https://jupyterbook.org/) and the [executablebooks/cookiecutter-jupyter-book template](https://github.com/executablebooks/cookiecutter-jupyter-book).
