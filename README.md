# Training-supervised-neural-networks-for-PolSAR-despeckling-with-an-hybrid-approach

This repository contains the training dataset used in the [IEEE GRSL](https://ieeexplore.ieee.org/document/10319732) paper.

if you find it useful and use it for you research, please cite as the following 

```
@ARTICLE{10319732,
  author={Lu, Xialei and Vitale, Sergio and Aghababei, Hossein and Ferraioli, Giampaolo and Pascazio, Vito},
  journal={IEEE Geoscience and Remote Sensing Letters}, 
  title={Training Supervised Neural Networks for PolSAR Despeckling With an Hybrid Approach}, 
  year={2024},
  volume={21},
  number={},
  pages={1-5},
  doi={10.1109/LGRS.2023.3333671}}
```

In this paper study on the effect of different training approaches for PolSAR despeckling is provided.
Inspired by similar analysis on SAR amplitude case in [Hybrid-MONet](https://ieeexplore.ieee.org/document/9474572) and [G-MOnet](https://ieeexplore.ieee.org/document/10250969)
a multi-temporal and training approach for training a CNN for PolAR despeckling is provided. The dataset has been tested on [MONet](https://ieeexplore.ieee.org/document/9261137) customized for the PolSAR case.

# Team members
 Sergio Vitale    (contact person, sergio.vitale@uniparthenope.it);
 Dong-Xiao Yue (yue_dong_xiao@163.com)
 Giampaolo Ferraioli (giampaolo.ferraioli@uniparthenope.it);
 Alejandro Frery (alejandro.frery@vuw.ac.nz);
 Feng Xu (fengxu@fudan.edu.cn);
 Vito Pascazio (vito.pascazio@uniparthenope.it);
 
# License
Copyright (c) 2023 Dipartimento di Ingegneria and Dipartimento di Scienze e Tecnologie of Università degli Studi di Napoli "Parthenope".

All rights reserved. This work should only be used for nonprofit purposes.

By downloading and/or using any of these files, you implicitly agree to all the
terms of the license, as specified in the document LICENSE.txt
(included in this directory)

# Usage 
* *model* contains trained weigths
* *model.py* contains the model implementation
* *testing.py* is the main script for testing
In the folder data, an ICEYE SLC sample if GDANSK is provided. 

# Prerequisites
This code is written on Ubuntu system for Python3.7 and uses Pytorch library.
- python=3.7
- pythorc=3.9.1
- cuda = 10.2
  
For a correct usage of the code, please install the python environement saved in **./env/gmonet.yml** with the following step:

**Installing Anaconda** (if not already installed)

1. download anaconda3 from https://www.anaconda.com/products/individual#linux
2. from command line, move to the download directory and install the package by:
> sh <Anaconda_downloaded_version>.sh 
and follow the instruction for installation
3. add conda to path
> PATH=~/anaconda3/bin:$PATH

**Installing the conda environment**

The file ./insarmonet_env.yml contains the environemnt for the testing the code. You can easily installing it by command line:

1. move to the folder containing the github repository and open the terminal
2. run the following command
 > conda env create -f insarmonet_env.yml


Once environment has been set up, activate it by command line as well:

1. activate the environemnt from the command line

> conda activate insarmonet_env

2. launch spyder

> spyder

3. goes to the folder containing **testing.py**, edit and run


