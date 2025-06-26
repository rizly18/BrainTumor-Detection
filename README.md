# 🧠 Brain Tumor Segmentation with YOLO11 and SAM2

## 📌 Overview

This project implements an advanced pipeline for **brain tumor detection and segmentation** from MRI images using a hybrid approach that combines **YOLO11** (You Only Look Once – real-time object detection) with **SAM2** (Segment Anything Model v2 – foundation segmentation model from Meta AI).

---

## 🎯 Objectives

- ✅ Detect and localize brain tumors in MRI scans using object detection.
- ✅ Segment tumor regions at the pixel level with high precision.
- ✅ Build a unified pipeline that supports preprocessing, detection, segmentation, and visualization.

---

## 🛠️ Approach

### 1. **Data Preprocessing**
- Resize and normalize MRI images.
- Apply augmentation techniques (rotation, flipping, brightness, etc.).

### 2. **Tumor Detection (YOLO11)**
- Fine-tune YOLO11 on labeled brain MRI scans.
- Detect tumor regions with bounding boxes.
- Use high-confidence predictions to reduce false positives.

### 3. **Tumor Segmentation (SAM2)**
- Pass YOLOv8-predicted ROIs to SAM2 for detailed segmentation.
- Extract precise tumor masks from the full-resolution images.

### 4. **Post-processing & Evaluation**
- Overlay segmentation masks on original MRI scans.
- Evaluate performance using metrics such as:
  - **IoU (Intersection over Union)**
  - **Dice Score**
  - **Precision & Recall**

---

## 📊 Results

- High-accuracy detection and segmentation in various tumor types.
- Real-time inference speed with YOLO11 + high-resolution mask quality from SAM2.
