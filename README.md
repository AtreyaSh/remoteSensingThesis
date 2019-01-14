# Remote-Sensing Approach to Spatio-Temporal Analysis of Vegetation Cover in Dharamshala Tehsil Region

## Overview

This repository contains the latex code for my personal thesis entitled above. This thesis entails using the random forests ensemble machine learning algorithm to classify Landsat 8 surface reflectance data into various vegetation categories. Next, change detection techniques were used to identify sub-regions undergoing vegetation loss. The time period for analysis was from 2013-2017.

The following repositories cover the methodologies of this thesis in further detail:

1. geeBulkFilter (https://github.com/AtreyaSh/geeBulkFilter)

2. vegMonitor (https://github.com/AtreyaSh/vegMonitor)

## Guide for Ubuntu 16.04

The base directory contains the `tex` files used for compiling the thesis manuscript. Compilation requires an installation of `python-pygments`, which can be done by executing the following:

```shell
$ sudo apt-get install python-pygments
```

Compilation of the tex files into pdf requires the following command with a `--shell-escape` for the `minted` tex-package to work.

```shell
$ pdflatex --shell-escape -synctex=1 -interaction=nonstopmode Thesis_Manuscript.tex
```

The output of pdflatex was further compressed using `ghostscript` (referenced from https://askubuntu.com/questions/113544/how-can-i-reduce-the-file-size-of-a-scanned-pdf-file) with the following command:

```shell
$ gs -sDEVICE=pdfwrite -dPDFSETTINGS=/prepress -dCompatibilityLevel=1.4 -dNOPAUSE -dQUIET -dBATCH -sOutputFile=reduced.pdf Thesis_Manuscript.pdf
```

## Documents

The directory `/docs` contains the thesis manuscriipt entitled `Thesis_Manuscript.pdf` and the thesis defense entitled `Thesis_Defense.pdf`.
