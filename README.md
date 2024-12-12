# Real-time Driver Drowsiness Detection

## Overview
This project implements a real-time driver drowsiness detection system using TensorFlow and OpenCV. The system monitors the driver’s facial features and alerts them if signs of drowsiness are detected. It leverages computer vision techniques and pre-trained Haar Cascade models to identify facial and eye patterns, ensuring safety by reducing the risk of accidents caused by drowsy driving.

## Features
- Real-time video feed analysis using a webcam.
- Detection of eyes and face using Haar Cascade classifiers.
- An alarm system that activates when signs of drowsiness are detected.
- Modular design with customizable model components.

## Prerequisites
- Python 3.7 or later
- OpenCV 4.5 or later
- TensorFlow 2.x

## Installation

1. **Clone the repository**:
   ```bash
   git clone <repository_url>
   cd driver-drowsiness-detection
   ```

2. **Install dependencies**:
   ```bash
   pip install opencv-python tensorflow numpy
   ```

3. **Download Haar Cascade XML files** (if not included):
   - `haarcascade_frontalface_alt.xml`
   - `haarcascade_lefteye_2splits.xml`
   - `haarcascade_righteye_2splits.xml`
   
   These are pre-trained models for face and eye detection.

## Usage

1. **Run the main script**:
   ```bash
   python drowsiness\ detection.py
   ```

2. **How it works**:
   - The program captures real-time video from the default camera.
   - Facial landmarks and eye states are analyzed to determine if the driver is alert or drowsy.
   - If drowsiness is detected, an alarm sound (`alarm.wav`) is played to alert the driver.

3. **Customizing Parameters**:
   - You can modify thresholds for eye closure duration in the script to suit specific requirements.

## Files in the Repository
- **drowsiness detection.py**: Main script for running the detection system.
- **model.py**: Contains the model logic for drowsiness detection.
- **alarm.wav**: Sound file for the alarm.
- **Haar Cascade XML files**: Pre-trained models for face and eye detection.
  - `haarcascade_frontalface_alt.xml`
  - `haarcascade_lefteye_2splits.xml`
  - `haarcascade_righteye_2splits.xml`

## Notes
- Ensure your system has an operational webcam for real-time video processing.
- The alarm file (`alarm.wav`) can be replaced with any desired sound.

## Future Enhancements
- Integration of deep learning models for improved accuracy.
- Support for multi-driver detection in shared environments.
- Mobile app or embedded system deployment.

## License
This project is licensed under the [MIT License](LICENSE).

---
