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

## Technology Stack

### Software Requirements
**Programming Language:** Python                    
**Libraries:**
OpenCV – Image processing and face detection            
dlib – Facial landmark detection                        
NumPy – Numerical computations                           
pygame – Audio alerts                                            
**Development Environment:** Python IDLE / Jupyter Notebook                      
### Hardware Requirements                           
Operating System: Windows 7 or later / Linux / macOS                                
Processor: Intel i5 or higher                                                 
RAM: Minimum 4GB                                         
Webcam: Required for video input                                        
  
## Modules

1. **Capturing Input Video**
The system captures video using the webcam, which is then processed frame by frame.

2. **Face Detection**
The system detects the face in the video stream using a face detection algorithm.

3. **Landmark Prediction**
Using dlib's 68-point facial landmark detector, the system identifies key facial features such as eyes, mouth, and jawline.

4. **EAR and MAR Calculation**
- **EAR (Eye Aspect Ratio):** Measures the eye’s openness and helps detect drowsiness.
- **MAR (Mouth Aspect Ratio):** Measures mouth openness to detect yawns.

5. **Drowsiness and Yawn Detection**
- If the driver’s eyes are closed for too long (indicating drowsiness), the system issues an alert.
- If the driver yawns, an alert is triggered to warn of potential fatigue.
  

## Installation Instructions

1. **Clone this repository:**
   ```bash
   git clone https://github.com/KeerthiP08/Warning_system_for_Drivers
   cd Warning_system_for_drivers
2. **Install Dependencies**
   Ensure you have Python installed, then install the required libraries:
   ```bash
   pip install -r requirements.txt
3. **Run the Application**
   Execute the main script:
   ```bash
   python drowsiness_yawn.py --webcam 0

## Usage

1. Ensure the webcam is properly connected.
2. Run the script to start real-time monitoring.
3. The system continuously processes video frames and detects drowsiness based on:
   - Eye closure for a prolonged time (EAR below threshold).
   - Yawning detection (MAR exceeding a set threshold).
4. If fatigue is detected, an audio alarm is triggered to alert the driver.

## Future Work
- **Improve Accuracy:** Improve the accuracy and efficiency of the detection system.
- **Lighting Conditions:** Address issues with poor lighting conditions by using infrared backlights.
- **Additional Factors:** Explore external factors (weather, vehicle state, etc.) for measuring fatigue and drowsiness.

## Conclusion
This project provides an effective and affordable solution for detecting driver fatigue and yawning, which are primary causes of road accidents. By providing timely warnings to the driver, this system can help save lives and reduce accidents on the road. The system uses an innovative approach with facial landmark detection and is cost-effective, making it an ideal choice for real-world applications.

## Contributions & Support
Contributions are welcome! Feel free to submit issues or pull requests to improve the project.   
For any questions, contact: keerthireddy0508@gmail.com
