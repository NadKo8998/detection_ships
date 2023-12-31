# U-Net: Convolutional Network for Biomedical Image Segmentation 

## The u-net is convolutional network architecture for fast and precise segmentation of images.
<img src="https://pp.userapi.com/c854420/v854420774/9732f/7JeFZnZa-Xo.jpg" width=640 height=450>

## Goals, description of the competition
We are given  images, which might contain ships or other waterborne vehicles. The goal is to detect ship images.
The training data is given as images and masks for the ships (in a run length encoded format). If an image contains multiple ships, each ship has a separate record, mask. 

## Project scheme
    .
    ├── model
    │   ├── modelTrain.py             # 
    │   └── inferenceTrain.py            # 
    ├── tools                     
    │   ├── data.py             # generates data 
    │   └── image.py            # image-related functions  
    ├── images                     
    │   ├── img                 # image examples for readme
    │   └── mask                # generated by nn masks
    ├── main.py                 # main script to run
    └── ...

    ## Installation

After installing the Python 3.7 version of, clone the project
```sh
git clone https://github.com/NadKo8998/detection_ships/tree/main
```
Create and activate a tensorflow virtual environment (no GPU support):
```sh
conda create -n tensorflow_env tensorflow
conda avtivate tensorflow_env
```

Alternatively, create a tensorflow virtual environment with GPU support:
```sh
conda create --name tf_gpu tensorflow-gpu 
conda avtivate tf_gpu
```

Install other packages to the virtual environment:
```sh
conda install -c conda-forge keras   # installs Keras
```
```sh
conda install matplotlib               # installs matpoltlib
```
```sh
conda install scikit-image             # installs skimage
