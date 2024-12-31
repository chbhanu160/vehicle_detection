# **Vehicle Detection and Tracking Using YOLO and DeepSORT**

A machine learning-based project for real-time vehicle detection and tracking using YOLOv8 and DeepSORT. This project integrates single-lane vehicle detection and advanced tracking capabilities.

---

## **Table of Contents**
1. [Features](#features)
2. [Demo](#demo)
3. [Installation](#installation)
4. [Results](#results)
5. [Acknowledgments](#acknowledgments)
6. [Technologies Used](#technologies-used)
7. [Contributing](#contributing)
8. [Contact](#contact)

---

## **Features**
- Real-time vehicle detection and tracking
- Single-lane vehicle counting
- Traffic signal control logic
- Easy integration with YOLOv8 and DeepSORT
- Displays vehicle direction and count

---

## **Demo**
![Vehicle Detection Demo](demo.gif)  
*Example of vehicle detection and tracking in action.*

---

## **Installation**

### Prerequisites
- Python 3.10
- Pytorch 1.12 or higher
- CUDA Toolkit for GPU acceleration (optional)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/chbhanu160/vehicle_detection.git
   cd YOLOv8-DeepSORT-Object-Tracking\
2. Install the Dependencies
   ```bash
   pip install -e '.[dev]'
3. Setting the Directory.
   ```bash
   cd ultralytics/yolo/v8/segment
5. For yolov8 object detection + Tracking + Vehicle Counting
   ```bash
   python predict.py model=yolov8l.pt source="test3.mp4" show=True
---

## **Results**
### Vehicle Counting And Tracking
![figure3 (1)](https://github.com/user-attachments/assets/6d63ddb8-b2d0-47f4-9e27-80e08d7dede1)
### Single Lane Traffic Management


https://github.com/user-attachments/assets/d70ad8b7-3084-4981-a638-6addae32506c


---
## **Acknowledgements**
This project was inspired by and uses code from:
- MuhammadMoinFaisal's YOLOv8 + DeepSORT Repository: [https://github.com/MuhammadMoinFaisal/YOLOv8-DeepSORT-Object-](https://github.com/MuhammadMoinFaisal/YOLOv8-DeepSORT-Object-Tracking)

---

## **Technologies Used**
- YOLOv8: For object detection.
- DeepSORT: For object tracking.
- OpenCV: For image and video processing.
- Python: Core programming language.
- CUDA: GPU acceleration.
      
## **Contributing**

Contributions are welcome! Please fork the repository and create a pull request with your improvements.

## **Contact**
- Kumar Chandra Bhanu
- GitHub: https://github.com/chbhanu160
- Email: kr.chandra.bhanu@gmail.com
