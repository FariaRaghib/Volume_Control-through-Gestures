# Hand Gesture Controlled Volume Adjustment
This project implements a hand gesture-based volume control system using OpenCV, Mediapipe, and PyAutoGUI. The program detects hand gestures (specifically, the distance between the thumb and index finger) and adjusts the system's volume accordingly. When the distance between the two fingers increases, the volume is increased, and when it decreases, the volume is lowered.

## Features
-Real-time Hand Gesture Detection: Detects hand gestures using Mediapipe.\
-Volume Control: Controls system volume based on the distance between the thumb and index finger.\
-Visual Feedback: Displays hand landmarks and a line connecting the thumb and index finger on the webcam feed.
## Installation
### Prerequisites
Python 3.x

## Required Python libraries:
OpenCV (opencv-python)\
Mediapipe (mediapipe)\
PyAutoGUI (pyautogui)
## Steps to Run
- Clone the repository:
### git clone https://github.com/FariaRaghib/Volume_Control-through-Gestures
### cd your-repository-name
- Install the required dependencies:
### pip install opencv-python mediapipe pyautogui
Run the project:
### python main.py\
The program will open your webcam and start detecting hand gestures. Move your thumb and index finger closer or farther apart to control the system volume.

## How It Works
-Hand Detection: Mediapipe detects the position of hand landmarks (specifically the thumb and index finger).
-Distance Calculation: The Euclidean distance between the thumb and index finger is calculated.
-Volume Control: If the distance exceeds a threshold, the system volume is increased. If the distance is smaller, the volume is decreased.
-Visual Feedback: A line connecting the thumb and index finger is drawn on the webcam feed, along with circles representing the fingertips.
