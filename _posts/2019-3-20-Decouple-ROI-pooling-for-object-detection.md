---
layout: post
title: "Decouple ROI pooling for object detection"
---

I mainly focus on region-based object detection frameworks (i.e. Faster-RCNN) which are composed of proposal modules on top of feature extraction modules and make detections. Based on the work of current region-based CNN detection, I introduced an approach to enhance the adaptive receptive capability of CNN, namely decouple ROI pooling. The module can enable the network to select the best receptive field to improve its classification accuracy without sacrificing its ability of bounding box regression.

{:refdef: style="text-align: center;"}
![Decouple ROI modules](/assets/images/module.png)*Decouple ROI modules*
{: refdef}

Codes are available at [Github](https://github.com/quanpr/decouple-roi-pooling). Experiment details are summarized in the [report](/assets/pdf/2019-3-20-Decouple-ROI-pooling-for-object-detection.md).
