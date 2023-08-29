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

The five time-phase original images of each position are saved in the support directory, and the five time-phase key images of each position are saved in the query directory. The key image is cropped from the center of the original image. The latitude and longitude coordinate information of the original image is saved in the label.text.
