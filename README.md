<div align="center">
<img src="https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/blob/main/images/LIFDlogo.png"></a>
<a href="https://www.cemac.leeds.ac.uk/">
  <img src="https://github.com/cemac/cemac_generic/blob/master/Images/cemac.png"></a>
  <br>
</div>

# Leeds Institute for Fluid Dynamics Machine Learning For Earth Sciences #

# Convolutional Neural Networks

[![GitHub release](https://img.shields.io/github/release/cemac/LIFD_ConvolutionalNeuralNetworks.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/releases) [![GitHub top language](https://img.shields.io/github/languages/top/cemac/LIFD_ConvolutionalNeuralNetworks.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks) [![GitHub issues](https://img.shields.io/github/issues/cemac/LIFD_ConvolutionalNeuralNetworks.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/issues) [![GitHub last commit](https://img.shields.io/github/last-commit/cemac/LIFD_ConvolutionalNeuralNetworks.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/commits/master) [![GitHub All Releases](https://img.shields.io/github/downloads/cemac/LIFD_ConvolutionalNeuralNetworks/total.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/releases) ![GitHub](https://img.shields.io/github/license/cemac/LIFD_ConvolutionalNeuralNetworks.svg)[![DOI](https://zenodo.org/badge/366734586.svg)](https://zenodo.org/badge/latestdoi/366734586)

[![LIFD_ConvolutionalNeuralNetworks](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/actions/workflows/python-package-conda.yml/badge.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetwork/actions/workflows/python-package-conda.yml) 
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cemac/LIFD_ConvolutionalNeuralNetwork/HEAD?labpath=CNN.ipynb)

This notebook explores Convolutional Neural Networks to detect and categorise Volcanic deformation.

## Recommended Background Reading

If you are unfamiliar with some of the concepts covered in this tutorial it's recommended to read through the background reading below either as you go through the notebook or beforehand.

* [The very basics in a Victor Zhou Blog](https://victorzhou.com/blog/intro-to-cnns-part-1/)
* [A deep dive into CNNs in towards data science](https://towardsdatascience.com/deep-dive-into-convolutional-networks-48db75969fdf)

## Quick look

If you want a quick look at the contents inside the notebook before deciding to run it please view the [md file](https://github.com/cemac/LIFD_ConvolutionalNeuralNetwork/blob/main/ConvolutionalNeuralNetworks/CNN_Volcanic_deformation.md) generated (*note some HTML code not rendered fully*)

## Installation and Requirements

This notebook is designed to run on a laptop with no special hardware required therefore recommended to do a local installation as outlined in the repository [howtorun](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/howtorun.md) and [jupyter_notebooks](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/jupyter_notebooks.md) sections.


These notebooks require some additional data from the [VolcNet](https://github.com/matthew-gaddes/VolcNet) repository

If you have not already then in your gitbash or terminal please run the following code in the LIFD_ENV_ML_NOTEBOOKS directory via the terminal(mac or Linux)  or git bash (windows)

```bash
git submodule init
git submodule update --init --recursive
```

**If this does not work please clone the [VolcNet](https://github.com/matthew-gaddes/VolcNet) repository into your ConvolutionalNeuralNetworks folder on your computer**

### Quick start

If you're already familiar with git, anaconda and virtual environments the environment you need to create is found in CNN.yml and the code below to install activate and launch the notebook

```bash
conda env create -f CNN.yml
conda activate CNN
jupyter-notebook
```
