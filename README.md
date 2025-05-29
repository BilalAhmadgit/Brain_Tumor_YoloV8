# Brain Tumor Detection Using YOLOv8

## Overview
This project implements an automated brain tumor detection system using the YOLOv8 deep learning model. It detects and localizes brain tumors in MRI images by drawing bounding boxes around detected tumors and classifying their type.

## Features
- Uses YOLOv8 for accurate object detection.
- Custom dataset created by merging multiple MRI datasets.
- Includes training, inference, and report generation scripts.
- Outputs human-readable diagnostic reports based on detections.

## Project Structure
- `data/` - Contains MRI images and annotation files.
- `models/` - YOLOv8 model weights and configurations.
- `scripts/` - Training, inference, and report generation code.
- `reports/` - Sample diagnostic reports and result images.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/BilalAhmadgit/Brain_Tumor_YoloV8.git
   cd Brain_Tumor_YoloV8
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Usage
Train the model:

bash
Copy
Edit
python scripts/train.py --data data/brain_tumor.yaml --epochs 50 --weights yolov8.pt
Run inference on test images:

bash
Copy
Edit
python scripts/infer.py --weights runs/train/exp/weights/best.pt --source data/test_images/
Generate diagnostic report:

bash
Copy
Edit
python scripts/generate_report.py --input results/predictions.json
Results
Achieved good accuracy and detection performance on validation data.

Sample output images and reports can be found in the reports/ folder.

Contributing
Contributions are welcome! Feel free to open issues or pull requests.

License
This project is licensed under the MIT License.
