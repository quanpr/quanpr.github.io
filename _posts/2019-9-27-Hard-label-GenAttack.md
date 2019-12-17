---
layout: post
title: "Black-box hard-label GenAttack"
---

Existing GenAttack is a state-of-the-art methods on fooling deep learning based image classifier in black-box setting. However, it still requires probability after softmax layer for adversarial samples selection. In this work, we extend the GenAttack to hard-label case. With an appropriate amount of queries to the TOP-1 class label, the GenAttack can attack the Inception based image classifier on ImageNet.

{:refdef: style="text-align: center;"}
![L2 distance changes w.r.t. the number of queries](/assets/images/hard-label.png) 
*L2 distance changes w.r.t. the number of queries*
{: refdef}

{:refdef: style="text-align: center;"}
![Fooling the image classifier by classifying squirrel as parking meter](/assets/images/compared.png) 
*Fooling the image classifier by classifying squirrel as parking meter*
{: refdef}


