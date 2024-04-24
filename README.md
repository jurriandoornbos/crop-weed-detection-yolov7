<div align="center">
  <p>
    <a href="https://icaerus.eu" target="_blank">
      <img width="50%" src="https://icaerus.eu/wp-content/uploads/2022/09/ICAERUS-logo-white.svg"></a>
    <h3 align="center">MEGAWEEDS: Crop/Weed detection with Transfer Learning YOLOv7</h3>
    
   <p align="center">
    Pre-training dataset comparisons and effects of Transfer Learning YOLOv7 Deep Learning network on a downstream task, with a focus on Precision agriculture Weed detection.
    <br/>
    <br/>
    <br/>
    <br/>
    <a href="https://github.com/jurriandoornbos/crop-weed-detection/issues">Report Bug</a>
    -
    <a href="https://github.com/jurriandoornbos/crop-weed-detection/issues">Request Feature</a>
  </p>
</p>
</div>

![Downloads](https://img.shields.io/github/downloads/jurriandoornbos/crop-weed-detection/total) ![Contributors](https://img.shields.io/github/contributors/jurriandoornbos/crop-weed-detection?color=dark-green) ![Forks](https://img.shields.io/github/forks/jurriandoornbos/crop-weed-detection?style=social) ![Stargazers](https://img.shields.io/github/stars/jurriandoornbos/crop-weed-detection?style=social) ![Issues](https://img.shields.io/github/issues/jurriandoornbos/crop-weed-detection) ![License](https://img.shields.io/github/license/jurriandoornbos/crop-weed-detection) 

![workflow](../images/workflow.png)

## Table Of Contents

* [Content](#content)
* [Installation](#installation)
* [Authors](#authors)
* [Acknowledgments](#acknowledgments)
  
## Content
This repository covers the dataset creation/preparation, model training and evaluation code and model weights for transfer learning YOLOv7 on a agricultural-specific pretraining dataset. Compared to COCO pretraining.
All the code and methods are found in their respective notebooks in the `notebooks` folder.
Additionally, pretrained YOLOv7 model weights on are found here: [MEGAWEEDS_YOLOv7](https://zenodo.org/records/8107077)
Finally the MEGAWEEDS dataset can be found on Zenodo over here: [MEGAWEEDS dataset](https://zenodo.org/records/8077195).

## Installation
There are 2 different ways to get started: 1. Python installation or, 2. A precompiled docker-container
### 1: Anaconda
Get your preferred Python installation method (Pip, Conda, miniforge, etc.) and install ultralytics, pytorch and jupyterlab

### 2: Docker
Not wanting to deal with anaconda and environment.yamls? Run everything in a docker container:
1. Install [Docker](https://docs.docker.com/get-docker/)
2. Start Docker
3. Start the Jupyter-lab docker
from your command-line with docker installed and ready:
this pulls the most recent ddal with all packages and libraries installed.
```
    docker run --rm -it -p 8888:8888 --shm-size=5gb -v /directory/to/this/repo/on/local/machine:/home/jovyan docker/container:tag
```
Or using GPUs: Install Docker with [NVIDIA](https://github.com/NVIDIA/nvidia-docker) runtime and run a gpu-enabled docker container:
```
    docker run --rm -it --runtime=nvidia -p 8888:8888 --gpus 1 --shm-size=5gb -v /directory/to/this/repo/on/local/machine:/home/jovyan docker/container:tag
```

## Acknowledgements
This project is funded by the European Union, grant ID 101060643.

<img src="https://rea.ec.europa.eu/sites/default/files/styles/oe_theme_medium_no_crop/public/2021-04/EN-Funded%20by%20the%20EU-POS.jpg" alt="https://cordis.europa.eu/project/id/101060643" width="200"/>

## Authors
* **Sophie Wildeboer** - *Wageningen University* - [Sophie Wildeboer](https://github.com/sophie789w)
* **Jurrian Doornbos** - *Wageningen University* - [Jurrian Doornbos](https://github.com/jurriandoornbos)