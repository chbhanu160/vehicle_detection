Vehicle Detection and Tracking with YOLOv8 and DeepSORT
This project implements a vehicle detection and tracking system using machine learning techniques, leveraging YOLOv8 Segmentation and DeepSORT for accurate object detection and tracking. The project also integrates a traffic signal control logic for single-lane scenarios, enabling dynamic signal switching based on vehicle presence and movement.

Key Features
Object Detection: Uses YOLOv8 for detecting vehicles (cars, buses, motorbikes, etc.) in video streams.
Object Tracking: Integrates DeepSORT for tracking objects across frames with unique identities.
Traffic Signal Logic:
Dynamically switches traffic lights based on vehicle presence in lanes.
Ensures efficient lane management with red and green signals.
Custom Lane Detection: Implements single-lane vehicle detection to monitor entering and leaving vehicles with counting logic.
Project Inspiration
This project draws inspiration from the repository YOLOv8_Segmentation_DeepSORT_Object_Tracking. Enhancements and additional features such as traffic signal control logic and lane-specific vehicle detection have been developed.

Traffic Signal Logic Overview
Green Signal: Lights up when vehicles are detected in the lane.
Red Signal: Lights up when no vehicles are detected or when a lane is inactive.
Real-time Counting: Tracks and displays the number of vehicles entering and leaving the lane.
Project Requirements
To replicate this project, the following dependencies are required:

Python 3.8+
PyTorch
OpenCV
ultralytics (YOLOv8)
deep_sort_pytorch
NumPy
SymPy
Install dependencies using:

bash
Copy code
pip install -r requirements.txt
Usage
Clone the Repository
bash
Copy code
git clone https://github.com/yourusername/Vehicle-Detection-and-Traffic-Signal.git
cd Vehicle-Detection-and-Traffic-Signal
Initialize the DeepSORT Tracker
Ensure the deep_sort_pytorch/configs/deep_sort.yaml file is properly configured.

Run the Code
Run the vehicle detection script with:

bash
Copy code
python vehicle_detection.py --source <video_path> --weights <yolov8_weights_path>
Traffic Signal Visualization
The program displays the current status of traffic signals on the video feed, with real-time updates based on vehicle movement.

Results
The project detects and tracks vehicles accurately, while dynamically managing traffic signals. It can be adapted for various scenarios, including multi-lane management.

Sample Output
Vehicle counting on entering and leaving the lane.
Real-time traffic signal control for efficient traffic flow.
Acknowledgments
YOLOv8_Segmentation_DeepSORT_Object_Tracking for providing the base implementation for object detection and tracking.
