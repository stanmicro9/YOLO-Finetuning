# YOLO-Finetuning
# Blood Cell Object Detection using YOLOv8

This repository implements a complete end-to-end pipeline for detecting White Blood Cells (WBC), Red Blood Cells (RBC), and Platelets in microscopic images. The project focuses on fine-tuning two different YOLOv8 variants to compare performance on medical imaging data.

## ❖ Project Overview
Detecting different types of blood cells is a critical task in clinical diagnostics. This project utilizes:
- **Dataset:** Blood Cell Detection Dataset.
- **Models:** YOLOv8 Nano (v8n) and YOLOv8 Medium (v8m).
- **Technique:** Fine-tuning (Transfer Learning) on pre-trained weights.

## ❖ Key Features
- **Data Conversion:** Automated script to convert CSV bounding box annotations to the normalized YOLO TXT format.
- **Data Splitting:** Strategic 80/20 split for training and testing.
- **Comparative Analysis:** Detailed performance metrics (mAP@50, Recall, Precision) for two model scales.
- **Visualization:** Integrated inference script to visualize predictions on test samples.

---

## Project Structure
```text
├── data_preparation.ipynb   # Handles CSV parsing, image normalization, and folder splitting
├── yolov8n_training.ipynb   # Fine-tuning and evaluation of YOLOv8 Nano
├── yolov8m_training.ipynb   # Fine-tuning and evaluation of YOLOv8 Medium
├── requirements.txt         # Project dependencies
└── blood_cell_config.yaml   # Dataset configuration for Ultralytics
