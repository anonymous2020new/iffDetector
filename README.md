# iffDetector
The code is for "iffDetector: Inference-aware Feature Filtering for Object Detection".
This repository provides iff detector heads for 
[YOLOv2](https://arxiv.org/pdf/1612.08242.pdf), 
[SSD](https://link.springer.com/chapter/10.1007/978-3-319-46448-0_2), 
[FoveaBox](https://arxiv.org/pdf/1904.03797.pdf), 
[CenterNet](https://arxiv.org/pdf/1904.08189.pdf) 
and [FreeAnchor](http://papers.nips.cc/paper/8309-freeanchor-learning-to-match-anchors-for-visual-object-detection.pdf).
The corresponding config files are in the configs folder.

## Performance

### New performance on PASCAL VOC

|Detector|Backbone|Dataset|mAP|Model|
| :-------: | :-------: | :-------: | :-------: | :-------: |
|YOLOv2|Darknet-19|VOC07|60.4|[Link](https://drive.google.com/file/d/1o2BRmPvTflfELPNnYGTtRDU8rApZWLg8/view?usp=sharing)|
|SSD|vgg-16|VOC07+12|78.0|[Link](https://drive.google.com/file/d/1rI0NW0YMOx6oKxkLZ9CBoezWu0BTkn5r/view?usp=sharing)|

### New performance on MSCOCO 2017

|Detector|Backbone|Multi-scalet<br> testing|AP(test-dev)|Model|
| :-------: | :-------: | :-------: | :-------: | :-------: |
|FoveaBox|ResNet-50|N|37.6|[Link](https://drive.google.com/file/d/15EADtUjvBTwxrqAzVcu8R10hslkZSUMK/view?usp=sharing)|
|FreeAnchor|ResNet-50|N|39.6|[Link](https://drive.google.com/file/d/1OzfBEi4oxIWA6Yvz9KLd5vogqHZIvbdt/view?usp=sharing)|
|CenterNet|Hourglass-104|Y|45.8|Link|
|FreeAnchor|ResNeXt-101|Y|47.9|[Link](https://drive.google.com/file/d/1wXPE2Pc9GrWcg9O-K_ZhMWK4bo2vwAEK/view?usp=sharing)|

## Installation and Usage

Please refer to the following Code Link for corresponding requirements and usage:
[YOLOv2](https://github.com/longcw/yolo2-pytorch), [SSD](https://github.com/amdegroot/ssd.pytorch), [FoveaBox](https://github.com/open-mmlab/mmdetection), [CenterNet](https://github.com/xingyizhou/CenterNet), [FreeAnchor](https://github.com/zhangxiaosong18/FreeAnchor). 
**Note that according to the Linear [Scaling Rule](https://arxiv.org/abs/1706.02677), you need to set the learning rate proportional to the batch size if you use different GPUs or images per GPU.**

