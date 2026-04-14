# Gesture-Controlled Robotic Arm using Computer Vision

System that uses a camera to track hand gestures and control a 2DOF robotic arm in real time.

---

## Features
- Detects hand and finger positions using camera
- Maps gestures to robotic arm movement
- Controls servos via Arduino Nano
- Real-time response with basic smoothing

---

## Tech Stack
Python, OpenCV, MediaPipe Hands, Arduino Nano, Servo motors

---

## How It Works
The system uses MediaPipe Hands to extract hand landmarks from the camera feed.  
These landmarks are processed to determine finger positions and angles.  
The calculated values are mapped to servo positions using inverse kinematics for a 2-link arm.  
Commands are sent to Arduino, which controls the servos.  
Basic filtering is applied to reduce noise and stabilize movement.

---

## Demo
[Video demo](PASTE_YOUR_LINK_HERE)

---

## Installation
```bash
pip install -r requirements.txt
python src/main.py
