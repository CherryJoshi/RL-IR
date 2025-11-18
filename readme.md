# RL for Imgae Restoration,ISP and Enhancement
###  <img src="./imgs/icon1.png" width="20" style="vertical-align: middle;"> Reinforcement Learning for Multi-Degradation Image Restoration: A Survey


This repository provides a curated collection of papers, benchmarks, and resources from our survey:  Reinforcement Learning for Multi-Degradation Image Restoration: A Survey

---
## Abstract


---
## Content
- [📣 News](#news)
- [📄 Paper List](#paper-list)
---
## News
- 2025-03: Repository initialized.

## Paper List

We categorize recent RL-restore papers by components:
### 3.1 Based on Action Space Design
#### 3.1.1 Module selection
It defines the action space as the selection among a set of restoration modules. 
The core idea is to decompose common image restoration strategies into independent functional units, treating each strategy tailored to a specific degradation type as a "tool".
<table>
<thead>
<tr>
<th align="left">Title</th>
<th align="center">Publication</th>
<th align="center">Date</th>
<th align="center">Tags</th>
<th align="center">Code</th>
</tr>
</thead>
<tbody>
<tr>
  <td align="left">
    <a href="">
    </a>
  </td>
  <td align="center">CVPR</td>
  <td align="center">2019</td>
  <td align="center">module selection</td>
  <td align="center"><a href="">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://arxiv.org/pdf/1804.03312.pdf">
      Crafting a toolchain for image restoration by deep reinforcement learning.
    </a>
  </td>
  <td align="center">CVPR</td>
  <td align="center">2018</td>
  <td align="center">module selection</td>
  <td align="center"><a href="https://github.com/yuke93/RL-Restore">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://openaccess.thecvf.com/content_CVPR_2019/papers/Suganuma_Attention-Based_Adaptive_Selection_of_Operations_for_Image_Restoration_in_the_CVPR_2019_paper.pdf">
      Attention-Based Adaptive Selection of Operations for Image Restoration in the Presence of Unknown Combined Distortions
    </a>
  </td>
  <td align="center">CVPR</td>
  <td align="center">2019</td>
  <td align="center">module selection</td>
  <td align="center"><a href="https://github.com/sg-nm/Operation-wise-attention-network">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://ieeexplore.ieee.org/document/9746115">
      JE2NET: Joint Exploitation and Exploration in Reinforcement Learning Based Image Restoration
    </a>
  </td>
  <td align="center">ICASSP</td>
  <td align="center">2022</td>
  <td align="center">module selection</td>
  <td align="center">github</td>
</tr>
<tr>
  <td align="left">
    <a href="https://arxiv.org/abs/2207.12056">
      REPNP: Plug-and-Play with Deep Reinforcement Learning Prior for Robust Image Restoration
    </a>
  </td>
  <td align="center">ICIP</td>
  <td align="center">2022</td>
  <td align="center">module selection</td>
  <td align="center">github</td>
</tr>
<tr>
  <td align="left">
    <a href="https://dl.acm.org/doi/abs/10.1145/3532625">
      Image Quality Assessment–driven Reinforcement Learning for Mixed Distorted Image Restoration
    </a>
  </td>
  <td align="center">ACM Transactions on Multimedia Computing, Communications, and Applications</td>
  <td align="center">2023</td>
  <td align="center">module selection</td>
  <td align="center">github</td>
</tr>
<tr>
  <td align="left">
    <a href="https://ieeexplore.ieee.org/abstract/document/9751218">
      Underwater Image Enhancement With Reinforcement Learning
    </a>
  </td>
  <td align="center"> IEEE </td>
  <td align="center">2024</td>
  <td align="center">module selection</td>
  <td align="center"><a href="https://gitee.com/sunshixin_upc/underwater-image-enhancement-with-reinforcement-learning">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://www.sciencedirect.com/science/article/pii/S0167865524001181">
      Low-quality image object detection based on reinforcement learning adaptive enhancement.
    </a>
  </td>
  <td align="center"></td>
  <td align="center"> </td>
  <td align="center">module selection</td>
  <td align="center"><a href="">github</a></td>
</tr>  
</tbody>
</table>

#### 3.1.2 Restoration Degree Control
The agent makes decisions for local regions or individual pixels, determining whether to further refine, enhance, or preserve each pixel based on its current state and prior restoration outcomes.
<table>
<thead>
<tr>
<th align="left">Title</th>
<th align="center">Publication</th>
<th align="center">Date</th>
<th align="center">Tags</th>
<th align="center">Code</th>
</tr>
</thead>
<tbody>
<tr>
  <td align="left">
    <a href="">
    </a>
  </td>
  <td align="center">CVPR</td>
  <td align="center">2019</td>
  <td align="center">Restoration Degree Control</td>
  <td align="center"><a href="">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://link.springer.com/article/10.1007/s11042-019-07914-5">
     Image registration optimization mechanism based on reinforcement learning and real time denoising. 
    </a>
  </td>
  <td align="center">SPRINGER</td>
  <td align="center">2020</td>
  <td align="center">Restoration Degree Control/Multi-agent RL </td>
  <td align="center">github</td>
</tr> 
<tr>
  <td align="left">
    <a href="https://ieeexplore.ieee.org/document/8936404">
      PixelRL: Fully Convolutional Network With Reinforcement Learning for Image Processing
    </a>
  </td>
  <td align="center"> IEEE </td>
  <td align="center">2020</td>
  <td align="center">Restoration Degree Control</td>
  <td align="center"><a href="https://github.com/rfuruta/pixelRL">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://ojs.aaai.org/index.php/AAAI/article/view/5423">
      MRI Reconstruction with Interpretable Pixel-Wise Operations Using Reinforcement Learning
    </a>
  </td>
  <td align="center">AAAI</td>
  <td align="center">2020</td>
  <td align="center">Restoration Degree Control</td>
  <td align="center">github</td>
</tr>
<tr>
  <td align="left">
    <a href="https://ieeexplore.ieee.org/document/9593591">
      Pixel-wise deep reinforcement learning approach for ultrasound image denoising.
    </a>
  </td>
  <td align="center">IEEE</td>
  <td align="center">2021</td>
  <td align="center">Restoration Degree Control</td>
  <td align="center">github</td>
</tr>
<tr>
  <td align="left">
    <a href="">
      R3l: Connecting deep reinforcement learning to recurrent neural networks for image denoising via residual recovery. 
    </a>
  </td>
  <td align="center">IEEE</td>
  <td align="center">2021</td>
  <td align="center">Restoration Degree Control</td>
  <td align="center">github</td>
</tr>
<tr>
  <td align="left">
    <a href="https://arxiv.org/abs/2403.18270">
      Image deraining via self-supervised reinforcement learning
    </a>
  </td>
  <td align="center">arxiv</td>
  <td align="center">2024</td>
  <td align="center">Restoration Degree Control</td>
  <td align="center"><a href="https://github.com/JasonHippo/Image_Deraining_via_Self-supervised_Reinforcement_Learning">github</a></td>
</tr>
</tbody>
</table>

#### 3.1.3 Network Architecture Path Planning
The image restoration model is designed with multiple parallel or hierarchical branches, each tailored to handle different degradation types or extract different feature representations. 
The RL agent dynamically selects the most appropriate path through the network based on the input image characteristics or intermediate states.
<table>
<thead>
<tr>
<th align="left">Title</th>
<th align="center">Publication</th>
<th align="center">Date</th>
<th align="center">Tags</th>
<th align="center">Code</th>
</tr>
</thead>
<tbody>
<tr>
  <td align="left">
    <a href="">
    </a>
  </td>
  <td align="center">CVPR</td>
  <td align="center">2019</td>
  <td align="center">Network Architecture Path Planning</td>
  <td align="center">github</td>
</tr>
<tr>
  <td align="left">
    <a href="https://arxiv.org/abs/1904.10343">
      Path-restore: Learning network path selection for image restoration.
    </a>
  </td>
  <td align="center">IEEE</td>
  <td align="center">2019</td>
  <td align="center">Network Architecture Path Planning</td>
  <td align="center"><a href="https://www.mmlab-ntu.com/project/pathrestore/">github</td>
</tr>
<tr>
  <td align="left">
    <a href="https://ieeexplore.ieee.org/document/10409270">
      Pathnet: Path-selective point cloud denoising.
    </a>
  </td>
  <td align="center">IEEE</td>
  <td align="center">2024</td>
  <td align="center">Network Architecture Path Planning</td>
  <td align="center"><a href="https://github.com/ZeyongWei/PathNet">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://link.springer.com/article/10.1007/s11760-020-01824-y">
      Mixed distortion image enhancement method based on joint of deep residuals learning and reinforcement learning. 
    </a>
  </td>
  <td align="center">SPRINGER</td>
  <td align="center">2021</td>
  <td align="center">Network Architecture Path Planning</td>
  <td align="center">github</td>
</tr>
</tbody>
</table>

#### 3.1.4 Parameter Adjustment
Reinforcement learning can also be employed to dynamically adjust key parameters in the image restoration process, such as denoising strength, color enhancement coefficients, or blur radius. 
<table>
<thead>
<tr>
<th align="left">Title</th>
<th align="center">Publication</th>
<th align="center">Date</th>
<th align="center">Tags</th>
<th align="center">Code</th>
</tr>
</thead>
<tbody>
<tr>
  <td align="left">
    <a href="https://arxiv.org/abs/1804.04450">
      Distort-and-recover: Color enhancement using deep reinforcement learning
    </a>
  </td>
  <td align="center">CVPR</td>
  <td align="center">2018</td>
  <td align="center">Parameter Adjustment</td>
  <td align="center"><a href="https://sites.google.com/view/distort-and-recover/">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://arxiv.org/abs/2107.05830">
      Rellie: Deep reinforcement learning for customized low-light image enhancement.
    </a>
  </td>
  <td align="center">ACM MM</td>
  <td align="center">2021</td>
  <td align="center">Parameter Adjustment/image enhancement</td>
  <td align="center"><a href="https://github.com/GuoLanqing/ReLLIE">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://arxiv.org/abs/2207.03081">
      DRL-ISP: Multi-Objective Camera ISP with Deep Reinforcement Learning
    </a>
  </td>
  <td align="center">IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)</td>
  <td align="center">2022</td>
  <td align="center">Parameter Adjustment/ISP</td>
  <td align="center"><a href="https://github.com/UkcheolShin/DRL-ISP">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="">
      DPOK: Reinforcement Learning for Fine-tuning Text-to-Image Diffusion Models
    </a>
  </td>
  <td align="center">NeurIPS</td>
  <td align="center">2023</td>
  <td align="center">Parameter Adjustment/Diffusion model</td>
  <td align="center"><a href="https://github.com/google-research/google-research/tree/master/dpok">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://ieeexplore.ieee.org/document/10083088">
      Image enhancement using adaptive region- guided multi-step exposure fusion based on reinforcement learning. 
    </a>
  </td>
  <td align="center">IEEE</td>
  <td align="center">2023</td>
  <td align="center">Parameter Adjustment/image enhancement</td>
  <td align="center">github</td>
</tr>
<tr>
  <td align="left">
    <a href="https://ojs.aaai.org/index.php/AAAI/article/view/28307">
      RL-SeqISP: Reinforcement Learning-Based Sequential Optimization for Image Signal Processing
    </a>
  </td>
  <td align="center">AAAI</td>
  <td align="center">2024</td>
  <td align="center">Parameter Adjustment/ISP</td>
  <td align="center">github</td>
</tr>
<tr>
  <td align="left">
    <a href="https://arxiv.org/abs/2503.07300">
      Goal Conditioned Reinforcement Learning for Photo Finishing Tuning
    </a>
  </td>
  <td align="center">NIPS</td>
  <td align="center">2024</td>
  <td align="center">Parameter Adjustment</td>
  <td align="center"><a href="https://github.com/OpenImagingLab/RLPixTuner/tree/master">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://www.sciencedirect.com/science/article/pii/S0952197624005694">
      INSPIRATION: A reinforcement learning-based human visual perception-driven image enhancement paradigm for underwater scenes
    </a>
  </td>
  <td align="center"></td>
  <td align="center">2024</td>
  <td align="center">Parameter Adjustment</td>
  <td align="center"><a href="https://gitee.com/wanghaoupc/uie_inspiration">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://ieeexplore.ieee.org/abstract/document/10497123">
      Metalantis: A Comprehensive Underwater Image Enhancement Framework
    </a>
  </td>
  <td align="center">IEEE</td>
  <td align="center">2024</td>
  <td align="center">Parameter Adjustment/underwater enhancement</td>
  <td align="center"><a href="https://gitee.com/wanghaoupc/Metalantis_UIE">github</a></td>
</tr>

  
</tbody>
</table>

### 3.2 Based on RL Formulation/Algorithm

#### 3.2.3 Hierarchical RL
HRL typically consists of a high-level policy and a low-level policy: the high-level policy is responsible for setting global objectives—such as selecting regions to process, determining stage-wise restoration goals, or choosing action types—while the low-level policy executes fine-grained actions (e.g., pixel-level adjustments or localized enhancements) based on the high-level directives.
<table>
<thead>
<tr>
<th align="left">Title</th>
<th align="center">Publication</th>
<th align="center">Date</th>
<th align="center">Tags</th>
<th align="center">Code</th>
</tr>
</thead>
<tbody>
<tr>
  <td align="left">
    <a href="https://arxiv.org/abs/1912.03966">
     Efficient object detection in large images using deep reinforcement learning
    </a>
  </td>
  <td align="center">WACV</td>
  <td align="center">2020</td>
  <td align="center">Hierarchical RL/object detection</td>
  <td align="center"><a href="https://github.com/uzkent/EfficientObjectDetection">github</a></td>
</tr> 
<tr>
  <td align="left">
    <a href="https://ieeexplore.ieee.org/document/9747299">
      HIRL: HYBRID IMAGE RESTORATION BASED ON HIERARCHICAL DEEP REINFORCEMENT LEARNING VIA TWO-STEP ANALYSIS
    </a>
  </td>
  <td align="center">ICASSP</td>
  <td align="center">2022</td>
  <td align="center">Hierarchical RL</td>
  <td align="center"><a href="">github</a></td>
</tr>
<tr>
  <td align="left">
    <a href="https://www.mdpi.com/2072-4292/14/23/5998">
     Aerial Image Dehazing Using Reinforcement Learning
    </a>
  </td>
  <td align="center"></td>
  <td align="center">2022</td>
  <td align="center">Hierarchical RL</td>
  <td align="center">github</td>
</tr> 
<tr>
  <td align="left">
    <a href="https://ieeexplore.ieee.org/document/10574839">
      STAR-RL: Spatial-Temporal Hierarchical Reinforcement Learning for Interpretable Pathology Image Super-Resolution
    </a>
  </td>
  <td align="center">IEEE</td>
  <td align="center">2024</td>
  <td align="center">Hierarchical RL</td>
  <td align="center"><a href="https://github.com/CUHK-AIM-Group/STAR-RL">github</a></td>
</tr> 
<tr>
  <td align="left">
    <a href="https://arxiv.org/abs/2408.06803">
     Integrating saliency ranking and reinforcement learning for enhanced object detection.
    </a>
  </td>
  <td align="center">arxiv</td>
  <td align="center">2024</td>
  <td align="center">Hierarchical RL/object detection</td>
  <td align="center"><a href="https://github.com/mbar0075/SaRLVision">github</a></td>
</tr> 
</tbody>
</table>

### 3.3 Based on Reward function design


### 3.4 Based on LLM-powered and Prompt-Guided
In the field of image denoising, some studies have explored LLM-powered reinforcement learning frameworks to better cope with complex stochastic noise environments. 
<table>
<thead>
<tr>
<th align="left">Title</th>
<th align="center">Publication</th>
<th align="center">Date</th>
<th align="center">Tags</th>
<th align="center">Code</th>
</tr>
</thead>
<tbody>
<tr>
  <td align="left">
    <a href="https://arxiv.org/abs/2410.17809">
     An intelligent agentic system for complex image restoration problems
    </a>
  </td>
  <td align="center">ICLR</td>
  <td align="center">2025</td>
  <td align="center">LLM-powered</td>
  <td align="center"><a href="https://github.com/Kaiwen-Zhu/AgenticIR">github</a></td>
</tr> 

</tbody>
</table>

---
## Evaluation Metric

---

## Datasets

---
## Performance Evaluation

---
| paper | Avenue |link|Code| 创新点|year|
|--------|--------|----|----|--------|-----|
|模版：A Reinforcement Learning Paradigm of Configuring Visual Enhancement for Object Detection in Underwater Scenes<br><sub>author <sub>        |  IEEE      | [paper](https://github.com/Harbinzzy/All-in-One-Image-Restoration-Survey/blob/main/README.md?plain=1)   |  [code](https://github.com/Harbinzzy/All-in-One-Image-Restoration-Survey/blob/main/README.md?plain=1)  |  IEEE   |   |
|Underwater Image Enhancement With Reinforcement Learning<br><sub>Shixin Sun, Peng Ren  <sub>        |  IEEE      | [paper](https://ieeexplore.ieee.org/abstract/document/9751218)   |  [code](https://gitee.com/sunshixin_upc/underwater-image-enhancement-with-reinforcement-learning)  |  1.利用deepQ网络选择基本图像增强方法的动作，依次增强水下图像。2.探索开发训练方式   |2024|
|A Reinforcement Learning Paradigm of Configuring Visual Enhancement for Object Detection in Underwater Scenes<br><sub>Hao Wang , Shixin Sun ,XiaoBai<sub>        |  IEEE Xplore   | [paper]   | [code](https://gitee.com/wanghaoupc/RL_Configuring_VisualEnhancment_for_ObjectDetection) |水下图像特征作为state，【YOLOv5的检测分数增量mAP】目标检测分数作为奖励，视觉增强算法作为action。 特征提取：yolov5【获取三种尺寸的特征图 40×40×128、20×20×256和10×10×512】，模型：DDDQN [两个网络 online Q{挑选action}, target Q{估计action的价值}]|2023|
|CURL:Contrastive Unsupervised Representations for Reinforcement Learning<br><sub>Aravind Srinivas, Michael Laskin, Pieter Abbeel <sub> |  ICML2020 |[paper](https://arxiv.org/pdf/2004.04136)|[code](https://github.com/MishaLaskin/curl) |利用对比学习，自监督+RL损失，从原始像素中提取物理特征.|2020|






