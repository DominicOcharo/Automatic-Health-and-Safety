# Automatic-Health-and-Safety
# YOLOv8 Object Detection Model: Construction Site Safety

## Model Overview
This YOLOv8 object detection model is trained to recognize and detect 10 classes critical for construction site safety. The classes include:

- Hardhat
- Mask
- NO-Hardhat
- NO-Mask
- NO-Safety Vest
- Person
- Safety Cone
- Safety Vest
- Machinery
- Vehicle

Built on the YOLOv8s architecture, this model balances speed and accuracy, making it ideal for real-time safety monitoring.

## Training Details
- **Framework:** Ultralytics YOLOv8.0.203
- **Programming Language:** Python 3.8.18
- **Deep Learning Library:** PyTorch 2.1.0
- **Hardware:** NVIDIA GeForce GTX 1070 Ti GPU (8GB VRAM)
- **Epochs:** 100, with early stopping after 50 epochs of no improvement
- **Batch Size:** 8
- **Image Size:** 640x640 pixels

### Model Configuration
- **Pretrained Weights:** Initialized from `yolov8s.pt`, with 349 out of 355 items transferred.
- **Optimizer:** AdamW with an initial learning rate of 0.000714 and momentum of 0.9.

## Performance Metrics
- **Precision:** 93.43% 
- **Recall:** 78.50%
- **mAP@0.5:** 85.65%
- **mAP@0.5-0.95:** 61.41%
- **Fitness Score:** 0.6384

## Speed Metrics
- **Preprocessing Time:** 0.86 ms/image
- **Inference Time:** 6.78 ms/image
- **Post-processing Time:** 1.05 ms/image

## Model File
The model is saved as both `best.pt` and  `best.onnx` with a size of 83.5 MB (87,634,504 bytes) and 166 MB (174,702,592 bytes) respectively.

### Example model predictions:

![alt text](https://github.com/DominicOcharo/Automatic-Health-and-Safety/blob/main/images/10.jpeg?raw=true)

![alt text](https://github.com/DominicOcharo/Automatic-Health-and-Safety/blob/main/images/9.jpeg?raw=true)
