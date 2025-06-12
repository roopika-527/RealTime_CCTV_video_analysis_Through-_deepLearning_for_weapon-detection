# RealTime_CCTV_video_analysis_Through-_deepLearning_for_weapon-detection
🔫 Real-Time Weapon Detection Using Deep Learning
This project implements a real-time video analysis system for weapon detection (guns and knives) using a deep learning model based on the YOLOv3 object detection framework. The application can detect weapons from live webcam streams or pre-recorded video files.

📽️ Demo Setup

A typical setup used for real-time detection.

📌 Features
Detects weapons (Gun and Knife) in real-time from a webcam or video file.

Uses YOLOv3 trained on custom weapon datasets.

Displays detection confidence and labels.

Draws bounding boxes around detected weapons.

Optionally logs detections in terminal.

Simple interface: press Esc to exit.

📂 Project Structure
bash
Copy
Edit
├── weapon_detection.py          # Main Python script
├── yolov3_testing.cfg           # YOLOv3 configuration file
├── yolov3_training_2000.weights # YOLOv3 trained weights (not uploaded here)
├── pistol.mp4                   # Sample test video
├── room_ser.jpg                 # Sample room image for testing
├── README.md                    # Project documentation
🖥️ Requirements
Python 3.x

OpenCV

NumPy

Install required packages:

bash
Copy
Edit
pip install opencv-python numpy
⚙️ How to Run
Download or clone this repository.

Make sure you have yolov3_training_2000.weights and yolov3_testing.cfg in the project directory.

Run the detection script:

bash
Copy
Edit
python weapon_detection.py
When prompted, enter:

A video file name (e.g., pistol.mp4) — or

Press Enter to use the webcam.

Press Esc key anytime to stop.

📝 YOLOv3 Configuration & Training
The model uses a custom-trained YOLOv3 detector.

classes defined in the script: ["Gun", "Knife"]

Config file: yolov3_testing.cfg

Trained weights: yolov3_training_2000.weights

Note: To train your own YOLO model on custom weapon images, you’ll need to prepare annotated datasets and configure Darknet or OpenCV’s DNN module accordingly.

📊 Example Output
On detection:

Bounding boxes are drawn around weapons.

Class label and confidence displayed.

Console prints detection event.

🔒 Applications
Public safety surveillance systems

Airport or mall security monitoring

Automated alarm systems based on video feeds

Restricted area monitoring

📌 Future Enhancements
Add alert system (email/SMS) on detection.

Integrate audio alarm triggers.

Deploy on edge devices (Raspberry Pi + camera).

Expand to multi-class detection (e.g., explosives, harmful tools).
