# Real time Object Tracking using DeepSort and YOLOV5 : 

## Overview : 
Object tracking using DeepSORT and YOLOv5 is a computer vision project that aims to track persons in a video stream. The system uses a combination of two popular deep learning models: YOLOv5 for object detection and DeepSORT for object tracking.

YOLOv5 is a state-of-the-art object detection model that can detect and classify objects in real-time. It achieves high accuracy with a small model size, making it ideal for use on embedded systems. DeepSORT is a deep learning model that uses a combination of appearance and motion features to track objects across frames.

The project is implemented using Python and the popular computer vision library, OpenCV. The source code is available on GitHub and can be easily customized to track other objects besides persons.

This project has several potential applications, including surveillance systems, automated video analysis, and crowd management systems. By accurately tracking persons in a video stream, it can help improve the efficiency and effectiveness of these systems.


## How to use this repo for object tracking  ? 

- Clone this repo : `git clone https://github.com/Vinayakmane47/Object_tracking_DeepSort_YOLOV5.git` 
- Install requirements : `pip install -r yolov5 requirements.txt` 
- Install Pytorch : `conda install pytorch==1.7.0 torchvision==0.8.0 torchaudio==0.7.0 cpuonly -c pytorch`
- Install easydict : `pip install easydict`
- Make predictions : `python detect_sort.py --weights yolov5s.pt  --img 640  --source <filename>` if using webcam -> replace filename with 0


## How to train DeepSort  : 

- Train YOLOV5 with custom dataset if classes are different from COCO dataset 
- replace YOLOV5 trained model with `yolov5s.pt`
- prepare data of object you want to track which will have images of object only. 
- follow the instructions in google collab file : `https://drive.google.com/file/d/1ixRWA_fl9kS3kkFvWAuCo5qQMaQzPz9V/view?usp=sharing`
- Copy `cpkt.t7` deepsort model in `deep_sort_pytorch\deep_sort\deep\checkpoint`  for making predictions using this repo. 

## Results : 



