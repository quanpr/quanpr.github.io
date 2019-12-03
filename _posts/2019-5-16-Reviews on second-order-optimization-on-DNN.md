---
layout: post
title: "Reviews on second order optimization methods for deep learning"
---

I mainly inverstigate different second-order optimization methods in DNN in a stochastic manner, including Trust-region Method (TR) and (adaptive) Cubic Reg- ularization (CR), and compared their convergence rate, generalization error and computation efficiency with SGD.

{:refdef: style="text-align: center;"}
![Training loss of SReLU-ResNet](/assets/images/loss-srelu-resnet.png)*Training loss of SReLU-ResNet*
{: refdef}

{:refdef: style="text-align: center;"}
![Test accuracy of SReLU-ResNet](/assets/images/accu-srelu-resnet.png)*Test accuracy of SReLU-ResNet*
{: refdef}

I use the gradient based solver to solve each the inner optimization problems for both TR and CR problem. The method can effectively converge to a local minimum that has similar performance as SGD. However the overhead in each step is significant. I also compared LBFGS and Newton-CG methods in the project. The inferior performance may be caused by the noisy estimation of Hessian term.

Codes are available at [Github](https://github.com/quanpr/Second-order-method-for-Deep-Neural-Network.). Experiment details are summarized in the [report](/assets/pdf/ECE_236C_course_project_report_805227042_Pengrui.pdf).

