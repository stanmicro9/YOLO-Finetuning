# YOLO-Finetuning
# Blood Cell Object Detection using YOLOv8

![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
![YOLOv8](https://img.shields.io/badge/Ultralytics-YOLOv8-red.svg)

An automated pipeline for detecting **White Blood Cells (WBC)**, **Red Blood Cells (RBC)**, and **Platelets** using deep learning. This project demonstrates the transition from raw image data to comparative analysis between two YOLOv8 model variants to compare performance on medical imaging data.

## ❖ Project Overview
Detecting different types of blood cells is a critical task in clinical diagnostics. This project utilizes:
- **Dataset:** Blood Cell Detection Dataset.
- **Models:** YOLOv8 Nano (v8n) and YOLOv8 Medium (v8m).
- **Technique:** Fine-tuning (Transfer Learning) on pre-trained weights.

## ❖ Key Features
- **Data Conversion:** Automated script to convert CSV bounding box annotations to the normalized YOLO TXT format.
- **Fine-tuning**: Apply transfer learning to **YOLOv8 Nano** and **YOLOv8 Medium** rather than using generic inference.
- **Comparison**: Evaluate performance using mAP@50 and Recall/Precision metrics.
- **Visualization:** Integrated inference script to visualize predicted bounding boxes with confidence scores on random test samples.

---

## Project Structure
```text
├── images
├── data.csv
├── data_preparation.ipynb
├── yolov8n_training.ipynb
├── yolov8m_training.ipynb
├── requirements.txt
└── blood_cell_config.yaml
```
## Installation & Usage

1. **Clone the repo:**
   ```bash
   git clone [https://github.com/your-username/blood-cell-detection.git](https://github.com/your-username/blood-cell-detection.git)

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt

3. **Run pipeline:**
   Execute data_preparation.ipynb first, followed by the training notebooks.
