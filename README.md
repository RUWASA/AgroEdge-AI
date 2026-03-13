__🌱 Crop–Weed Detection using Knowledge Distillation__

**Overview**

This project implements a lightweight deep learning model for crop–weed detection in agricultural fields. The model uses knowledge distillation to transfer knowledge from a larger teacher model to a smaller student model, improving detection performance while keeping the model lightweight.

The system is evaluated using the CropWeed dataset and compared with multiple object detection models.

__Models Compared__

YOLOv11-Nano

YOLOv8-Nano

YOLOv7-Tiny

MobileNet-SSD

EfficientDet-D0

Faster R-CNN

SSD-Lite

DETR-Light

NanoDet

PP-YOLO-Tiny

__📂 Project Structure__

Crop-Weed-Detection

│
├── dataset
│   ├── images
│   └── labels
│
├── models
│   ├── teacher_model
│   └── student_model
│
├── training
│   └── train.py
│
├── evaluation
│   └── metrics.py
│
├── results
│   ├── graphs
│   └── outputs
│
└── README.md

__Results__

The proposed KD model achieved the best performance:

| Model                 | mAP@0.5  | mAP@0.5:0.95 | Precision | Recall   | F1 Score | IoU (%)   |
| --------------------- | -------- | ------------ | --------- | -------- | -------- | --------- |
| YOLOv11-Nano          | 0.83     | 0.53         | 0.86      | 0.71     | 0.77     | 53.53     |
| YOLOv8-Nano           | 0.85     | 0.53         | 0.82      | 0.76     | 0.79     | 53.55     |
| YOLOv7-Tiny           | 0.81     | 0.49         | 0.80      | 0.76     | 0.78     | 81.25     |
| MobileNet-SSD         | 0.0036   | 0.0032       | 0.70      | 0.0207   | 0.037    | 0.36      |
| EfficientDet-D0       | 0.20     | 0.18         | 0.34      | 0.58     | 0.43     | 20.014    |
| Faster R-CNN          | 0.48     | 0.43         | 0.99      | 0.49     | 0.65     | 48.88     |
| SSD-Lite              | 0.0022   | 0.0019       | 0.415     | 0.0053   | 0.01     | 0.22      |
| DETR-Light            | 0.81     | 0.52         | 0.80      | 0.74     | 0.77     | 81.74     |
| NanoDet               | 0.76     | 0.45         | 0.75      | 0.73     | 0.74     | 76.85     |
| PP-YOLO-Tiny          | 0.20     | 0.18         | 0.34      | 0.58     | 0.43     | 20.014    |
| **Proposed KD Model** | **0.86** | **0.58**     | **0.83**  | **0.78** | **0.80** | **58.11** |


__Applications__

Precision agriculture

Weed detection

Crop monitoring

Smart farming systems
