# RL for Imgae Restoration,ISP and Enhancement
###  <img src="./imgs/icon1.png" width="20" style="vertical-align: middle;"> Reinforcement Learning for Multi-Degradation Image Restoration: A Survey


This repository provides a curated collection of papers, benchmarks, and resources from our survey:  Reinforcement Learning for Multi-Degradation Image Restoration: A Survey

---
## Abstract
Image restoration (IR) and Image Enhancement tasks aim to improve visual quality and remove various degrading factors such as noise, blur, weather effects and compression artifacts. However, traditional methods rely on hand-designed prior models, making it difficult to handle the coupled relationships of multiple degradations in real-world scenes. While deep learning methods have made significant progress on specific tasks, they still face challenges such as insufficient interpretability, static processing flow and difficulty in adapting to different degradation patterns. To address these challenges, reinforcement learning (RL), as an intelligent learning paradigm capable of sequential decision-making and dynamic policy optimization, is gradually emerging as a potential solution in the IR field. RL methods can adaptively adjust restoration strategies based on intermediate results.
This review focuses on the application of RL in image restoration and enhancement, systematically discussing its algorithmic mechanisms and methodological design. It also comprehensively reviews the rapidly developing RL-based IR research in recent years. We first introduce the basic modeling methods of RL in IR. Subsequently, based on core dimensions such as action granularity, RL algorithm category, reward design and large model-driven agent structure, existing methods are systematically classified. Their theoretical characteristics and applicable scenarios are analyzed. Next, we summarize commonly used IR evaluation metrics, implementation details, evaluation criteria and compile typical public RL datasets to objectively compare the public results of mainstream RL methods, providing researchers with intuitive performance references.
Finally, this paper delves into the challenges faced by RL-based IR models, including reward sparsity, training efficiency, stability, generalization ability, difficulties in deploying them in real-world scenarios. Then it proposes possible RL-based IR future research directions. This review aims to serve as a systematic reference in this field, providing researchers and practitioners with a clear research framework and practical guidance, and promoting the further development of reinforcement learning in image restoration and enhancement.
<img src="./imgs/framework.svg" width="20" style="vertical-align: middle;">
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
We include commonly used datasets for evaluating RL performance.

### Synthetic datasets
| **Dataset**                       | **Year** | **Tasks**                           | **Description**                                                                                                                  |
| --------------------------------- | -------- | ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| BSD [[link]]()                    | 2005     | Deblur / Super-Resolution           | The BSD500 dataset contains 500 natural images (200 train / 100 val / 200 test), mostly 481×321 resolution.                      |
| CSIQ [[link]]()                   | 2010     | Deblur / Denoise / JPEG compression | 30 reference images with 6 distortion types (Gaussian blur, JPEG, JPEG2000, noise, etc.) for quality assessment and restoration. |
| MIT-Adobe FiveK [[link]]()        | 2011     | Image enhancement                   | 5,000 RAW images, each edited by 5 experts → 25,000 enhancement pairs; used for enhancement, color correction, white balance.    |
| LIVEMD [[link]]()                 | 2012     | Mixed distortions                   | 15 reference images → 405 distorted images (Gaussian noise + JPEG compression).                                                  |
| KITTI [[link]]()                  | 2012     | Enhancement / ISP simulation        | Autonomous driving dataset with 40,000+ stereo/RGB images at ~1240×376 resolution.                                               |
| MS-COCO [[link]]()                | 2014     | Enhancement / ISP simulation        | 118k train + 5k val images for detection/segmentation; widely used for augmentation, anti-ISP learning, composite degradation.   |
| ILSVRC [[link]]()                 | 2015     | Denoise / SR / Deblur / JPEG        | 1.28M train, 50k val, 100k test images (ImageNet 2012).                                                                          |
| MICCAI Grand Challenge [[link]]() | 2015     | Medical reconstruction / Deblur     | ~250 microscopic images (2048×1536) for cancer cell segmentation, reconstruction, blur correction.                               |
| DIV2K [[link]]()                  | 2017     | Deblur / Denoise / JPEG             | 1000 high-quality 2K images (800 train / 100 val / 100 test) for SR and restoration.                                             |
| Waterloo Exploration [[link]]()   | 2017     | Denoise                             | 4,744 pristine images + 94,880 distorted images (5 degradations × 4 intensity levels).                                           |
| OASBUD [[link]]()                 | 2017     | Ultrasound denoise                  | 1,000+ ultrasound images (B-mode & RF), used for noise reduction & tissue segmentation.                                          |
| Rain100L [[link]]()               | 2017     | Derain                              | 100 rainy images with GT, designed for light-rain removal benchmarking.                                                          |
| fastMRI [[link]]()                | 2018     | Medical reconstruction              | 1.5 TB MRI dataset: 40k+ knee/brain scans with raw k-space & reconstructions.                                                    |
| Rain800 [[link]]()                | 2019     | Derain                              | 700 train + 100 test synthetic rain images using multi-layer rain textures.                                                      |
| PU-GAN [[link]]()                 | 2019     | Point cloud upsampling              | 60 training + 20 test models (point cloud) for 3D upsampling tasks.                                                              |
| VOC-HyBrid [[link]]()             | 2024     | Low-quality object detection        | 10,000+ VOC-based images with synthetic degradations (noise, blur, low-light, JPEG).                                             |
| MiO100 [[link]]()                 | 2024     | Denoise / Deblur / JPEG             | 100 sets of composite-degradation images (noise+blur+compression), ~5,000 total.                                                 |



### Real-world datasets
| **Dataset**             | **Tasks**                                        | **Papers and Year**                            |
| ----------------------- | ------------------------------------------------ | ---------------------------------------------- |
| DICM (2012)             | Low-light image enhancement                      | ReLLIE                                         |
| NPE (2013)              | Low-light image enhancement                      | ReLLIE                                         |
| Paris-rue-Madame (2014) | Point cloud denoise                              | PathNet (2024)                                 |
| CLIVE (2015)            | Illumination, noise, blur, compression artifacts | JE2NET (2022); Image Quality Assessment (2023) |
| HDR+ (2016)             | ISP / Image enhancement                          | Photo Fine-Tuning (2024)                       |
| DND (2017)              | Denoising                                        | Path-Restore (2021)                            |
| LOL (2018)              | Low-light image enhancement                      | ReLLIE                                         |
| RENOIR (2018)           | Denoising                                        | Path-Restore (2021)                            |
| SIDD (2018)             | Denoising                                        | Path-Restore (2021)                            |
| Raindrop (2018)         | Derain                                           | Operation-wise Attention (2019)                |
| RTTS (2018)             | Dehaze                                           | Low-quality object detection (2024)            |
| UIEB (2019)             | Underwater enhancement                           | Underwater-RL (2023)                           |
| DDN-SIRR (2019)         | Derain                                           | Deraining RL (2024)                            |
| WB (2019)               | White balance correction                         | DRL-ISP (2022)                                 |
| U45 (2019)              | Underwater enhancement                           | INSPIRATION (2024)                             |
| RUIE (2020)             | Underwater enhancement                           | INSPIRATION (2024)                             |

---
## Performance Evaluation

---










