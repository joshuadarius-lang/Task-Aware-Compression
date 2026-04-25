# Task Aware Object Detection with YOLOv11 and MobileNetV3 and compression with custom CNN-correlation

This repository demonstrates object detection and image classification on drone-captured images using YOLOv11 (Ultralytics) and MobileNetV3 (TensorFlow). The code processes sample images like 0000168_01491_d_0000170.jpg, from the VisDrone dataset, with both bounding box detection and ImageNet classification.

## Features
Real-time object detection with lightweight YOLOv11n model.

Image classification using pre-trained MobileNetV3Large.

Easy inference on single images.

Custom CNN correleation image compression module

## Prerequisites
Python 3.8+

Required packages: ultralytics, tensorflow, numpy, pillow

GPU recommended for faster inference (optional).

## Installation
Clone the repository:

Place your image (e.g., 0000168_01491_d_0000170.jpg) in the root directory and run:

python detect_and_classify.py
The script will:

Run YOLOv11 detection and save result.jpg with bounding boxes.

Display MobileNetV3 predictions (top-3 ImageNet classes).

# Expected output example:

Predicted: [('n02084071', 'Cab', 0.45), ('n02099601', 'Limosine', 0.12)]

# VisDrone dataset Links

Test on drone footage with the VisDrone2019-DET benchmark (10 classes: pedestrian, car, bicycle, etc.).

Official repo: https://github.com/VisDrone/VisDrone-Dataset

Ultralytics format: https://docs.ultralytics.com/datasets/detect/visdrone/

# Links
Model/Dataset	Documentation	Download

YOLOv11	https://docs.ultralytics.com/models/yolo11/ 

yolo11n.pt (auto-download)

MobileNetV3	https://www.tensorflow.org/api_docs/python/tf/keras/applications/mobilenet_v3/MobileNetV3Large 

Pre-trained via TensorFlow

VisDrone	https://github.com/VisDrone/VisDrone-Dataset 

## Troubleshooting
Model download fails: Ensure internet access; models cache locally.

CUDA errors: Set device='cpu' in YOLO or install TensorFlow GPU.
