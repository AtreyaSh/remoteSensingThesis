# Remote-Sensing Approach to Spatio-Temporal Analysis of Vegetation Cover in Dharamshala Tehsil Region

## Overview

This is my personal thesis entitled "Remote-Sensing Approach to Spatio-Temporal Analysis of Vegetation Cover in Dharamshala Tehsil Region, Indian Northwestern Himalayas". This thesis entails using the random forests ensemble machine learning algorithm to classify Landsat 8 surface reflectance data into various vegetation categories. Next, change detection techniques were used to identify sub-regions undergoing vegetation loss. The time period for analysis was from 2013-2017.

## Guide for Ubuntu 16.04

1. The base directory contains the `tex` files used for compiling the thesis manuscript. Compilation requires an installation of `python-pygments`, which can be done by executing the following:

```shell
$ sudo apt-get install python-pygments
```

2. Compilation of the tex files into pdf requires the following command with a `--shell-escape` for the `minted` tex-package to work.

```shell
$ pdflatex --shell-escape -synctex=1 -interaction=nonstopmode Thesis_Manuscript.tex
```

## Documents

The directory `/docs` contains the thesis defense entitled `Thesis_Defense.pdf`.
