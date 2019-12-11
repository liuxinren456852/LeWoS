# LeWoS <br/> 
[![DOI](https://zenodo.org/badge/202789309.svg)](https://zenodo.org/badge/latestdoi/202789309) <br/>

Unsupervised tree leaf-wood classification from point cloud data <br/> 

# Usage<br/> 
There are many ways to use this tool.<br/> 
**(a) if you have Matlab installed:**<br/>
Option 1. Call the entry level funtion "RecursiveSegmentation_release.m".<br/> 
Option 2. Type "LeWoS_RS" in Matlab workspace. This will open up an interface by calling the classdef "LeWoS_RS.m". This classdef file defines the interface.<br/> 
Option 3. Drag "LeWoS.mlappinstall" into Matlab workspace. This will install a Matlab App for you. <br/> 
**(b) if you don't have Matlab installed, and don't want to install it:**<br/>
Run "LeWoS_installer.exe" for win64. If you need an excutable for other systems, please contact me.<br/> (PS: Matlab Runtime 2019b is required. You can either install it in advance or do it during the installation of LeWoS.)

*Note that if you load an ascii point cloud with the interface, only space delimiter is supported. (Recommend to use las files) <br/> 
*This method does not implement any post-processing filters. Users can design and apply post-processing steps to [potentially] further improve the results.

# Examples
![example 1](plot.png)
Plot-level separation<br/>
![example 2](crown.png)
Inside a crown
![example 3](e3.png)
Very thin branches are difficult to detect

# Acknowledgement
This repo contains code from Loic Landrieu's repo on point-cloud-regularization (https://github.com/loicland/point-cloud-regularization), and Inverse Tampere's repo on TreeQSM (https://github.com/InverseTampere/TreeQSM).

# Bibtex
@article{doi:10.1111/2041-210X.13342,
author = {Di, Wang and Momo Takoudjou, Stéphane and Casella, Eric},
title = {LeWoS: A Universal Leaf-wood Classification Method to Facilitate the 3D Modelling of Large Tropical Trees Using Terrestrial LiDAR},
journal = {Methods in Ecology and Evolution},
volume = {n/a},
number = {n/a},
pages = {},
keywords = {component separation, point cloud, regularization, segmentation, Terrestrial LiDAR, TreeQSM, tropical forest trees, volume},
doi = {10.1111/2041-210X.13342},
url = {https://besjournals.onlinelibrary.wiley.com/doi/abs/10.1111/2041-210X.13342}
}
(Current code is a slightly updated version of the one used in publication. With current one, the results are further improved a bit. e.g., 0.925 ± 0.035 vs 0.91 ± 0.03 in the paper.)
# Contact
Di Wang<br/> 
di.wang@aalto.fi
