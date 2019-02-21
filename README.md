# ResNet50 on Art Composition Attributes

Fine-tunes a ResNet50 (pretrained on imagenet) network by training on WikiArt images labeled with eight art composition attributes. This is a Fast.ai version of [https://github.com/hollygrimm/art-composition-cnn](https://github.com/hollygrimm/art-composition-cnn)

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

### Download Dataset
download test.tgz and train.tgz from [https://github.com/zo7/painter-by-numbers/releases/tag/data-v1.0](https://github.com/zo7/painter-by-numbers/releases/tag/data-v1.0)

```
cd data/wikiart
tar -xvf test.tgz
tar -xvf train.tgz
```

## Label Data with Attributes
Example category data is provided in [labels.csv](data/wikiart/labels.csv).