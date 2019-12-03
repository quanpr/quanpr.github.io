---
layout: post
title: "Deep-learning based Vehicle Re-identification"
---

Vehicle re-identification (ReID) is an important problem and has many applications in video surveillance and intelligent transportation. The existing approaches to vehicle ReID mainly relies on the appearance information of vehicles with an oversimplified spatiotemporal information. In this project, we make use of both the appearance of vehicles and their time and geo-location relationship to improve the retrieved accuracy.

Method       | mAP (%)             | top 1 accuracy (%)               | top 5 accuracy (%) 
--------------------- | --------------------- | --------------------- | ---------------------
Single ResNet-18 | 33.5 | 77.0 | 83.3
Single ResNet-50 | 37.1 | 79.5 | 87.4
SNN (ResNet-50)  | 41.1 | 89.4 | 95.2
SNN (ResNet-18) + Spatiotemporal model | 42.4 | 89.9 | 96.3
SNN (ResNet-50) + Spatiotemporal model | 47.6 | 94.7 | 99.5
Integrated SNN (ResNet-18)| 49.7 | 94.8 | 100
Integrated SNN (ResNet-50)| **58.6** | **96.6** | **100**


Implementations and experiment details may be found in the [report](/assets/pdf/1155092203_QuanPengrui.pdf).