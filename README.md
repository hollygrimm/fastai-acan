# fastai ResNet34 Sample Project

Fine-tunes a ResNet34 (pretrained on imagenet) network by training on dog and dingo images

## Requirements
* fastai
* pytorch
* torchvision
* jupyter

## Manual Install

### Create Conda Environment
```
conda update conda
conda create -n fastai
source activate fastai
conda install -c fastai fastai pytorch torchvision jupyter
pip install fastai --upgrade
```

### Create Dataset
Create dog and dingo folders under data/dog/folder and add images to these folders.

To use google_images_download to get images
install chromedriver https://sites.google.com/a/chromium.org/chromedriver/downloads then googleimagesdownload:



```
pip install google_images_download
googleimagesdownload -k "dingo" -s medium -l 500 -o fastai-dingo/data/dog/train -i dingo -cd ~/chromedriver
googleimagesdownload -k "dog" -s medium -l 500 -o fastai-dingo/data/dog/train -i dog -cd ~/chromedriver
```
