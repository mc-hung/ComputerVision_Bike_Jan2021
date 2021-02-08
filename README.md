# Welcome to Our ComputerVision - Bike Project
### Authors: Mei-Chun Judy Hung, Wasinee Opal Sriapha
We're thrilled to show you how we built this fascinating tool using **PyTorch** to detect the legendary pedal-driven vehicles (aka the 
first "vehicle" most of us owned!) in both photos and videos (and **Yes, it is capable of analyzing any YouTube videos!** Just paste the URL link and hit run!)

---

In this project, we aim to explore the next-generation platform for object detection and segmentation, **Detectron2**. Built by Facebook AI team, Detectron2 has been integrated as part of PyTorch (a deep learning framework) to allow high-quality implementations of state-of-the-art object detection algorithms. More details to follow!

<div class="row">
  <div>
    <img src="https://github.com/sriaphaw/ComputerVision_Bike_Jan2021/blob/master/GIF5.gif" width="500">
    <img src="https://github.com/sriaphaw/ComputerVision_Bike_Jan2021/blob/master/Result/GIF2.gif" width="500">
  </div>
</div>

<br>

## Dataset

We used Sense (https://sixgill.com/) to assist with the image/data gathering and labeling process.
 
106 images were labeled, then splitted with 80%, 10% and 10% for training, validation, and testing respectively.
 
The custom dataset was saved in COCO data format and exported into JSON 3 files (Train/Val/Test) with annotations in each file.
 
Note that COCO (Common Objects in Context) is defined as a large-scale object detection, segmentation, and captioning dataset.

<br>

## Training - Detectron2

Dataset is trained using Detectron2 library in this project.

Detectron2, a PyTorch-based modular object detection library, supports novel computer vision developments by offering implementations for all models in maskrcnn-benchmark.

Below is the snapshot of the accuracy result after the model was trained and evaluated with the entire validation dataset.

**Evaluation Results on Validation Set **
| category     | AP     |
|:-------------|:-------|
| Polygon_bike | 83.450 |

<br>

<p align="left">
  <img src="https://github.com/sriaphaw/ComputerVision_Bike_Jan2021/blob/master/Result/TensorBoard%20result.PNG" width="500" title="Evaluation Results on Validation Set, 300 steps">
</p>

<br>

## Now it's time to put the **Trained Model** into action

**Ran 2 sample images**

<div class="row">
  <div>
    <img src="https://github.com/sriaphaw/ComputerVision_Bike_Jan2021/blob/master/Result/Test1.PNG" width="500">
    <img src="https://github.com/sriaphaw/ComputerVision_Bike_Jan2021/blob/master/Result/Test2.PNG" width="380">
  </div>
</div>

### 99% and 98% Bikes respectively

<br>

**Evaluation results on Test Set**
| category     | AP     |
|:-------------|:-------|
| Polygon_bike | 83.064 |

<br>

## YouTube Time!
**It's time to run the object detection model on any fun online videos.**

Here we will use this clip as an example: Video Credit: Bike Radar (https://www.youtube.com/watch?v=rZKvUO0qO-o&t=0s)

<br>
 
### Results Revealed!!

<br>

<div>
  <div>
    <img src="https://github.com/sriaphaw/ComputerVision_Bike_Jan2021/blob/master/Result/GIF1.gif" width="800" title="Isn't that cool!?">
    <img src="https://github.com/sriaphaw/ComputerVision_Bike_Jan2021/blob/master/Result/GIF3.gif" width="800" title="Isn't that cool!?">
    <img src="https://github.com/sriaphaw/ComputerVision_Bike_Jan2021/blob/master/Result/GIF4.gif" width="800" title="Isn't that cool!?">
  </div>
</div>

<br>

## Enjoy Coding!!
