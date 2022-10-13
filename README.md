# A Real-Time Support with Haptic Feedback for Safer Driving using Monocular Camera
Project repository for the course of Visual Perception for Human-Robot Collaboration 2021, Sapienza University of Rome. 

The project has been developed by:
- Francesco Starna
- Lorenzo Guercio

## Abstract
In recent years, Artificial Intelligence for autonomous driving systems has become more and more important and is having a huge impact in our life. Our goal is to help increasing the safety of the drivers thanks to a feedback system based exclusively on the use of a monocular camera mounted on the top of the vehicle. The proposed idea is a real-time application that warns the driver of imminent dangers on the road classified according to their risk level. This method takes into consideration various techniques related to computer vision, such as object detection, tracking and image processing. All these already existing techniques had the purpose of allowing us to do a detailed danger analysis in order to be able to carry out a potential hazard evaluating objects in the vehicle’s range of motion.

## The project
At each frame we first take the image coming from a monocular camera, placed above the vehicle roof. Then we detect and classify the objects in the scene using YOLOv4, that is a one-stage object detector. We manipulate the camera calibration matrix in order to recover longitudinal and lateral distances from the vehicle to the objects detected. After that, we apply an object tracking algorithm on the objects in order to track their motion. Then, for each object detected, we evaluate the potential danger based on different specific criteria. We evaluate our method on the KITTI raw dataset, using mean average precision (mAP) for object detection, and root mean square error (RMSE) for distance estimation.

## Demonstration


## [Report](https://github.com/Starnino/eaivp-project/blob/main/EAI_Project.pdf)
## [Notebook](https://github.com/Starnino/eaivp-project/blob/main/eai-project.ipynb)
