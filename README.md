# MTGL40-5

This repository provides the dataset proposed in our paper "**MTGL40-5: A Multi-Temporal Dataset for Remote Sensing Image Geo-Localization**". (Remote Sensing)

**If you have any questions, you can send me an email. My mail address is 21171213974@stu.xidian.edu.cn.**

## Datasets

Download the  MTGL40-5 dataset in [here](). 

Datasets into following structure,

```
├─Location name
    ├─query
    	├─xxx.tif
    ├─support
    	├─xxx.tif
    ├─label.txt
    	
```



## Requirements

>Python 3.7<br>
>PyTorch 1.7.1

## Preparation

* Install DCNv2

```shell
cd DCNv2
python setup.py build develop
cd ..
```

**Attention:** Other versions of Python and PyTorch may cause compilation errors in DCNv2.


* Install other dependencies

All other dependencies can be installed via 'pip'.

* Pretrained weights

Place [ResNet-18](https://download.pytorch.org/models/resnet18-5c106cde.pth) and [DAT-tiny](https://drive.google.com/file/d/1I08oJlXNtDe8jJPxHkroxUi7lYX2lhVc/view?usp=sharing) pretrained weights in `./pretrained`.

## Train

```python
python train.py
```

All the hyperparameters can be adjusted in `./option`.

## Test

```python
python test.py --load_pretrain True --which_epoch 249
```

All the hyperparameters can be adjusted in `./option`.

### Acknowlogdement

This repository is built under the help of the projects [ISNet](https://github.com/xingronaldo/ISNet) and [DAT](https://github.com/LeapLabTHU/DAT) for academic use only.

