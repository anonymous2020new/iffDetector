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
|YOLOv2|Darknet-19|VOC07|60.4|[Link](https://drive.google.com/file/d/1MUCV6nqMA-SNc70wPraY415BAsRhn33N/view?usp=sharing)|
|SSD|vgg-16|VOC07+12|78.0|[Link](https://drive.google.com/file/d/1gZzcAnR7lE17vD2PdzyjZCyfAp-8mKBX/view?usp=sharing)|

### New performance on MSCOCO 2017

|Detector|Backbone|Multi-scalet<br> testing|AP(test-dev)|Model|
| :-------: | :-------: | :-------: | :-------: | :-------: |
|FoveaBox|ResNet-50|N|37.6|[Link](https://drive.google.com/file/d/1lg2M2UNbfX6_CrOIEEzoOztxi_s0VncT/view?usp=sharing)|
|FreeAnchor|ResNet-50|N|39.6|[Link](https://drive.google.com/file/d/1QAyLSQ2KjqPecdme6QDgHWXSE7d5xx0v/view?usp=sharing)|
|CenterNet|Hourglass-104|Y|45.8|[Link](https://drive.google.com/file/d/1D6h1SkwAveSU0_NeAKlRVWACQ_NDpGiG/view?usp=sharing)|
|FreeAnchor|ResNeXt-101|Y|47.9|[Link](https://drive.google.com/file/d/1tMqB41wAq4bd87emnavyyiIPvQJJL8mP/view?usp=sharing)|

## Installation and Usage

Please refer to the following Code Link for corresponding requirements and usage:
[YOLOv2](https://github.com/longcw/yolo2-pytorch), [SSD](https://github.com/amdegroot/ssd.pytorch), [FoveaBox](https://github.com/open-mmlab/mmdetection), [CenterNet](https://github.com/xingyizhou/CenterNet), [FreeAnchor](https://github.com/zhangxiaosong18/FreeAnchor). 
**Note that according to the Linear [Scaling Rule](https://arxiv.org/abs/1706.02677), you need to set the learning rate proportional to the batch size if you use different GPUs or images per GPU.**

