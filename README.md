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
| Model                 | mAP@0.5  | Precision | Recall   | F1 Score |
| --------------------- | -------- | --------- | -------- | -------- |
| YOLOv11-Nano          | 0.83     | 0.86      | 0.71     | 0.77     |
| YOLOv8-Nano           | 0.85     | 0.82      | 0.76     | 0.79     |
| YOLOv7-Tiny           | 0.81     | 0.80      | 0.76     | 0.78     |
| MobileNet-SSD         | 0.0036   | 0.70      | 0.02     | 0.037    |
| EfficientDet-D0       | 0.20     | 0.34      | 0.58     | 0.43     |
| Faster R-CNN          | 0.48     | 0.99      | 0.49     | 0.65     |
| SSD-Lite              | 0.0022   | 0.415     | 0.005    | 0.01     |
| DETR-Light            | 0.81     | 0.80      | 0.74     | 0.77     |
| NanoDet               | 0.76     | 0.75      | 0.73     | 0.74     |
| PP-YOLO-Tiny          | 0.20     | 0.34      | 0.58     | 0.43     |
| **Proposed KD Model** | **0.86** | **0.83**  | **0.78** | **0.80** |

__Applications__
Precision agriculture
Weed detection
Crop monitoring
Smart farming systems
