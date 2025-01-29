# Warning system for Drivers 
Driver Drowsiness and Yawn Detection System

## Overview

This project aims to develop a **Driver Drowsiness and Yawn Detection System** that helps improve road safety by detecting signs of drowsiness and yawning in drivers. The system uses a webcam to monitor the driver's face and detect facial landmarks. Based on the detection of the **Eye Aspect Ratio (EAR)** and **Mouth Aspect Ratio (MAR)**, the system can determine if the driver is becoming drowsy or yawning. If either of these conditions is detected, the system triggers an alert to prevent accidents.

## Features
- **Driver Drowsiness Detection:** Monitors the driver’s eyes for signs of fatigue based on the EAR.
- **Yawning Detection:** Detects yawns which can be an early indicator of drowsiness.
- **Night Vision Capability:** Uses a webcam to detect drowsiness in low-light conditions.
- **Real-time Processing:** Captures video and processes each frame in real-time.
- **Alerts:** Provides audio or visual warnings when drowsiness or yawning is detected.

## Modules

### 1. Capturing Input Video
The system captures video using the webcam, which is then processed frame by frame.

### 2. Face Detection
The system detects the face in the video stream using a face detection algorithm.

### 3. Landmark Prediction
Using dlib's 68-point facial landmark detector, the system identifies key facial features such as eyes, mouth, and jawline.

### 4. EAR and MAR Calculation
- **EAR (Eye Aspect Ratio):** Measures the eye’s openness and helps detect drowsiness.
- **MAR (Mouth Aspect Ratio):** Measures mouth openness to detect yawns.

### 5. Drowsiness and Yawn Detection
- If the driver’s eyes are closed for too long (indicating drowsiness), the system issues an alert.
- If the driver yawns, an alert is triggered to warn of potential fatigue.
  

## System Requirements

### Software Requirements:
- Python IDLE Shell
- **Libraries:** 
  - dlib
  - OpenCV
  - 68-point Face Landmark Detector
  - pygame
  - Numpy

### Hardware Requirements:
- Windows 7 or above
- Minimum 4GB RAM
- i5 Processor or above
- Webcam for capturing video

## Installation Instructions

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/drowsiness-yawn-detection.git
   cd drowsiness-yawn-detection
