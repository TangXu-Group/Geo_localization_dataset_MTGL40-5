# MTGL40-5

This repository provides the dataset proposed in our paper "**MTGL40-5: A Multi-Temporal Dataset for Remote Sensing Image Geo-Localization**". (Remote Sensing 2023)

**If you have any questions, you can send me an email. My mail address is tangxu128@xidian.edu.cn.**

# Introduction

In this paper, a novel dataset for cross-time geo-localization is proposed, named MTGL40-5. This dataset comprises 40 diverse geographic locations spanning five different years. For each location, the large-scale original and key images are captured, which contain the complete and key content of the corresponding location. Subsequently, the key/original images are split into query/database images for conducting geo-localization. By analyzing the content difference of the same landmark in different years, we aim to address the cross-time challenge and enhance the practicality of geo-localization.

![GA](C:\Users\17590\Desktop\Remote sensing geo-location\GA.jpg)

## Datasets

Download the MTGL40-5 dataset in [BaiduPan](https://pan.baidu.com/s/173w53DHAmHmXTZ6cppdpZg), Extraction code is MTGL . 

Datasets into following structure,

```
├─Location index
    ├─query
    	├─0/1/2/3/4
    		├─xxx.jpg
    ├─support
    	├─0/1/2/3/4
   	 		├─xxx.jpg
    ├─label.txt
    	
```

We provide datasets with N as 1024/2048/4096. The Location index is 0-40. The query directory stores the patch images of 5 phases at each position from the key images, the support directory (database) stores the patch images of 5 phases at each position from the original image. The latitude and longitude coordinate information of the original image is saved in the label.text.

