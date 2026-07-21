# VehiSecure 🚗🛡️

## Intelligent Suspicious Vehicle Detection and Verification System

VehiSecure is an AI-powered surveillance framework for **real-time
suspicious vehicle detection and verification**. The system detects
vehicles, localizes license plates, extracts plate text using OCR, and
verifies the extracted registration number against an authorized
(registered) vehicle database. Vehicles that are not found in the
database are flagged as **blacklisted/unregistered**, and real-time
alerts can be generated.

------------------------------------------------------------------------

## ✨ Key Features

-   Real-time vehicle detection from surveillance cameras
-   License plate localization
-   Optical Character Recognition (OCR) for plate text extraction
-   Verification against a registered vehicle database
-   Automatic identification of registered vs. blacklisted/unregistered
    vehicles
-   Dashboard-ready logs and alerts
-   Comparative evaluation of multiple object detectors and OCR engines

------------------------------------------------------------------------

## 🏗️ System Workflow

``` text
Surveillance Camera
        │
        ▼
Vehicle Detection
(YOLOv8 / YOLOv8n / YOLOv8s / YOLOv8m / RT-DETR / SSD /
 Faster R-CNN / EfficientDet / RetinaNet)
        │
        ▼
License Plate Detection
        │
        ▼
OCR Recognition
(EasyOCR / PaddleOCR / Gemma / Gemini)
        │
        ▼
Database Verification
(Registered Vehicle Database)
        │
   ┌────┴────┐
   ▼         ▼
Registered   Blacklisted /
 Vehicle     Unregistered
        │
        ▼
Alert • Dashboard • Logs
```

------------------------------------------------------------------------

## 📊 Research Objectives

-   Compare modern object detection models for vehicle detection.
-   Compare OCR engines for license plate recognition.
-   Evaluate system robustness under varying environmental conditions.
-   Develop a reliable real-time suspicious vehicle verification
    framework.

------------------------------------------------------------------------

## 📂 Project Structure

``` text
├── dataset/
├── models/
├── notebooks/
├── scripts/
├── weights/
├── results/
├── README.md
└── requirements.txt
```

------------------------------------------------------------------------

## 🔬 Models Evaluated

### Object Detection

-   YOLOv8
-   YOLOv8n
-   YOLOv8s
-   YOLOv8m
-   RT-DETR
-   SSD
-   Faster R-CNN
-   EfficientDet
-   RetinaNet

### OCR Engines

-   PaddleOCR
-   EasyOCR
-   Gemma (Vision)
-   Gemini (Vision)

------------------------------------------------------------------------

## 📈 Evaluation Metrics

### Detection

-   Precision
-   Recall
-   mAP@0.5
-   mAP@0.5:0.95
-   FPS
-   Inference Time

### OCR

-   Plate Recognition Accuracy
-   Character Recognition Accuracy
-   Character Error Rate (CER)
-   Levenshtein Distance
-   Average Inference Time

### End-to-End Verification

-   Registered Vehicle Verification Accuracy
-   Blacklisted Vehicle Detection Accuracy
-   False Positive Rate
-   False Negative Rate

------------------------------------------------------------------------

## 🌦️ Environmental Robustness

The framework is evaluated under: - Daylight - Night - Rain - Fog -
Motion Blur - Shadows - Different Camera Angles

------------------------------------------------------------------------

## 💻 Technology Stack

-   Python
-   Ultralytics YOLO
-   OpenCV
-   PyTorch
-   PaddleOCR
-   EasyOCR
-   Pandas
-   NumPy
-   Streamlit (Dashboard)
-   Excel / SQL Database

------------------------------------------------------------------------

## 🚀 Future Work

-   Edge deployment on NVIDIA Jetson
-   Multi-camera support
-   Automatic gate control integration
-   Vehicle re-identification
-   Face and driver verification
-   Cloud-based dashboard and analytics

------------------------------------------------------------------------

## 📄 License

This project is intended for academic research and educational purposes.

------------------------------------------------------------------------

## 👨‍💻 Author

**Muhammad Junaid**

AI Researcher \| Computer Vision \| Intelligent Surveillance Systems
