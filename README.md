# **Vehicle Detection and Tracking Using YOLO and DeepSORT**

A machine learning-based project for real-time vehicle detection and tracking using YOLOv8 and DeepSORT. This project integrates single-lane vehicle detection and advanced tracking capabilities.

---

## **Table of Contents**
1. [Features](#features)
2. [Motivation](#motivation)
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

## **Motivation**
- Detect Vehicles in Each Lane:
  - Use YOLO for vehicle detection: Detect vehicles in each lane by feeding frames from the video stream into YOLO. YOLO will provide bounding boxes for each vehicle detected.
  - Lane Division: Divide the video frame into lanes (using an algorithm or predefined positions) so that vehicles can be tracked in specific sections.
- Vehicle Tracking:
  - Use DeepSORT: Track the vehicles across frames with DeepSORT. This will help identify if a vehicle is still present in a lane or if it has exited.
  - Track Vehicle Count: Maintain a count of vehicles in each lane, updating as vehicles enter or exit the lanes.
- Implement Timer Logic:
  - Green Timer: When a vehicle is detected in a lane, set the timer to green for that lane. If a vehicle is no longer detected within a certain time frame, switch the light to red for       that lane.
  - Empty Lane Detection: If a lane is detected to be empty for a specified duration, immediately turn the light red and switch the timer to the next lane with vehicles.
- Traffic Signal Logic:
  - Signal Change: Once the timer for a lane with vehicles reaches its limit, change the signal to green for the next lane with vehicles. If no vehicles are detected, change to red and       move the timer to the next lane.

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
- GitHub: https://github.com/chbhanu160
- Email: kr.chandra.bhanu@gmail.com
