<div align="center">
<img src="https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/blob/main/images/LIFDlogo.png"></a>
<a href="https://www.cemac.leeds.ac.uk/">
  <img src="https://github.com/cemac/cemac_generic/blob/master/Images/cemac.png"></a>
  <br>
</div>

# Leeds Institute for Fluid Dynamics Machine Learning For Earth Sciences #

# Convolutional Neural Networks

[![GitHub release](https://img.shields.io/github/release/cemac/LIFD_ConvolutionalNeuralNetworks.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/releases) [![GitHub top language](https://img.shields.io/github/languages/top/cemac/LIFD_ConvolutionalNeuralNetworks.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks) [![GitHub issues](https://img.shields.io/github/issues/cemac/LIFD_ConvolutionalNeuralNetworks.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/issues) [![GitHub last commit](https://img.shields.io/github/last-commit/cemac/LIFD_ConvolutionalNeuralNetworks.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/commits/master) [![GitHub All Releases](https://img.shields.io/github/downloads/cemac/LIFD_ConvolutionalNeuralNetworks/total.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/releases) ![GitHub](https://img.shields.io/github/license/cemac/LIFD_ConvolutionalNeuralNetworks.svg)[![DOI](https://zenodo.org/badge/366734586.svg)](https://zenodo.org/badge/latestdoi/366734586)

[![LIFD_ConvolutionalNeuralNetworks](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/actions/workflows/python-package-conda.yml/badge.svg)](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/actions/workflows/python-package-conda.yml)


This notebook explores Convolutional Neural Networks to detect and categorise Volcanic deformation. To cater for low performance machines additional pre-made models and processed data are provided making **this repository 3.1G**. Therefore it's advised to read the installation instructions below for a parallel git-clone. No [binder](https://mybinder.readthedocs.io/en/latest/index.html#what-is-binder) link is provided as the datasets used are too large for the free tier.

## Recommended Background Reading

If you are unfamiliar with some of the concepts covered in this tutorial it's recommended to read through the background reading below either as you go through the notebook or beforehand.

* [The very basics in a Victor Zhou Blog](https://victorzhou.com/blog/intro-to-cnns-part-1/)
* [A deep dive into CNNs in towards data science](https://towardsdatascience.com/deep-dive-into-convolutional-networks-48db75969fdf)

## Quick look

If you want a quick look at the contents inside the notebook before deciding to run it please view the [md file](https://github.com/cemac/LIFD_ConvolutionalNeuralNetworks/blob/main/ConvolutionalNeuralNetworks/CNN_Volcanic_deformation.md) generated (*note some HTML code not rendered fully*)


### Quick start

If you're already familiar with git, anaconda and virtual environments the environment you need to create is found in CNN.yml and the code below to install activate and launch the notebook. The .yml file has been tested on the latest linux, macOS and windows operating systems.

```bash
git clone  --recurse-submodules -j8 git@github.com:cemac/LIFD_ConvolutionalNeuralNetworks.git
cd LIFD_ConvolutionalNeuralNetworks
wget -O data.tar.gz https://github.com/cemachelen/LIFD_ML_LARGE_FILE_STORE/archive/refs/tags/0.1-alpha.tar.gz
tar -xvf data.tar.gz
cp -rp LIFD_ML_LARGE_FILE_STORE-0.1-alpha/ConvolutionalNeuralNetworks/synthetic_data/*.pkl data/synthetic_data/
conda env create -f CNN.yml # Use the CNN_windows.yml if on windows machine
conda activate CNN
jupyter-notebook
```

## Installation and Requirements

This notebook is designed to run on a laptop with no special hardware required therefore recommended to do a local installation as outlined in the repository [howtorun](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/howtorun.md) and [jupyter_notebooks](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/jupyter_notebooks.md) sections.


These notebooks require some additional data from the [VolcNet](https://github.com/matthew-gaddes/VolcNet) repository.

If you have cloned already without the `--recurse` flag then in your gitbash or terminal please run the following code in the LIFD_ENV_ML_NOTEBOOKS directory via the terminal(mac or Linux)  or git bash (windows)

```bash
git submodule init
git submodule update --init --recursive
```

**If this does not work please clone the [VolcNet](https://github.com/matthew-gaddes/VolcNet) repository into your ConvolutionalNeuralNetworks folder on your computer**

Some data files are also required and instructions to do this are given above in a `wget` command. The notebook will also prompt you to do this.

# Licence information #

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">LIFD_ENV_ML_NOTEBOOKS</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://cemac.leeds.ac.uk/" property="cc:attributionName" rel="cc:attributionURL">cemac</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

## Acknowledgements

Thanks to Matthew Gaddes for the basis of this tutotial. This tutorial is part of the [LIFD ENV ML NOTEBOOKS](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS) please refer to for full acknowledgements.
