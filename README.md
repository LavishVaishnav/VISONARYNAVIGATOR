
# Visionary Navigator

**Visionary Navigator** is an AI-based smart stick solution designed to empower visually impaired individuals with seamless mobility and safety. By leveraging advanced technologies such as **Artificial Intelligence (AI)**, **Computer Vision**, **OpenCV**, and **NLP**, this system provides real-time object detection, environment descriptions, and auditory feedback. The system enables individuals to confidently navigate their surroundings with real-time alerts about obstacles and paths, ensuring greater independence and safety.

## Table of Contents
1. [Overview](#overview)
2. [Technologies](#technologies)
3. [System Design](#system-design)
4. [Implementation](#implementation)
5. [Results and Discussion](#results-and-discussion)
6. [Future Scope](#future-scope)
7. [How to Use](#how-to-use)
8. [Contributors](#contributors)
9. [References](#references)

---

## Overview

Visionary Navigator is an AI-based smart system that assists visually impaired individuals in navigating their environments safely and independently. This project utilizes the **YOLO (You Only Look Once)** algorithm for real-time object detection, **OpenCV** for image processing, and **Natural Language Processing (NLP)** for text-to-speech feedback. 

The system is designed to detect obstacles, provide real-time feedback on surroundings, and guide the user to their destination through intuitive auditory commands. This innovative solution not only enhances mobility but also increases the safety and confidence of visually impaired individuals.

### Key Features:
- **Real-Time Object Detection:** Detect obstacles and objects using a camera and the YOLO algorithm.
- **Auditory Feedback:** Real-time voice instructions using NLP and text-to-speech for navigation.
- **User-Friendly Design:** Voice commands, haptic feedback, and intuitive control.
- **Seamless Integration:** Connects with smartphones and GPS for enhanced functionality.

---

## Technologies

The Visionary Navigator project employs cutting-edge technologies to deliver a seamless experience for users:

- **Programming Languages:**
  - Python (Core logic, image processing, and AI)
  - JavaScript, HTML, CSS (Web-based UI)
  
- **Frameworks & Tools:**
  - OpenCV (Object Detection and Image Processing)
  - TensorFlow / PyTorch (For training the YOLO algorithm)
  - Flask/Django (Web server for communication between Raspberry Pi and the server)
  - gTTS / pyttsx3 (Text-to-Speech conversion)

- **Hardware:**
  - **Raspberry Pi 4 Model B** with a camera module for capturing images.
  - **Sensors**: Integration with GPS and other sensors for navigation.

---

## System Design

### 1. **Data Acquisition and Object Detection**
   - The Raspberry Pi captures live images and transmits them to a server.
   - The **YOLO algorithm** processes the images in real time to detect objects and determine their location relative to the user.
   
### 2. **NLP and Auditory Feedback**
   - The detected objects are translated into text descriptions using NLP.
   - The descriptions are converted into speech using TTS (Text-to-Speech), providing real-time feedback to the user.

### 3. **Navigation Assistance**
   - The system guides the user to avoid obstacles and find paths using voice commands.
   - Integration with GPS enables path guidance, while object detection alerts the user of nearby obstacles.

---

## Implementation

### Steps Involved:
1. **Dataset Collection**: Images were collected and annotated to train the YOLO model.
2. **Model Training**: The YOLO model was trained using TensorFlow, focusing on object detection accuracy and speed.
3. **System Integration**: 
   - **Camera Integration**: Raspberry Pi captures video feeds for processing.
   - **NLP & TTS Integration**: The detected objects are translated into speech.
   - **Web Application**: OpenCV-based object detection runs in a web application for easy access.

### Key Components:
- **Object Detection**: YOLO algorithm for detecting objects like pedestrians, vehicles, and obstacles.
- **Text-to-Speech**: Provides real-time voice feedback for detected objects.
- **Web Interface**: Allows users to visualize object detection results via a browser-based interface.

---

## Results and Discussion

The Visionary Navigator system successfully detects objects and provides real-time voice feedback, enabling visually impaired users to navigate their surroundings confidently. The **YOLO algorithm** was optimized to run on the Raspberry Pi, achieving real-time object detection and feedback. 

Key metrics:
- **Object Detection Accuracy**: Achieved over 95% accuracy for obstacle detection in diverse environments.
- **Real-Time Performance**: The system processes video feeds with minimal delay, ensuring timely feedback for the user.
  
---

## Future Scope

Visionary Navigator holds significant potential for further development:

1. **Integration of Advanced Sensors**: Incorporate **LiDAR** and **ultrasonic sensors** for enhanced obstacle detection in low-light environments.
2. **Improved Object Detection Algorithms**: Use more advanced models and fine-tuning techniques to further improve detection accuracy.
3. **AI-Driven Path Planning**: Implement dynamic path planning for better navigation assistance.
4. **Smart City Integration**: Connect the system with IoT-based smart city infrastructure for real-time updates on traffic and obstacles.

---

## How to Use

### Requirements:
- **Hardware**: Raspberry Pi 4 Model B, Camera Module, Micro SD Card.
- **Software**: Python, OpenCV, Flask/Django, gTTS.
  
### Installation Instructions:
1. **Clone the Repository**:
   ```bash
   git clone git@github.com:LavishVaishnav/VISONARYNAVIGATOR.git
   cd VISIONARYNAVIGATOR
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application**:
   ```bash
   python app.py
   ```

4. **Connect the Raspberry Pi** and Camera, and start detecting objects in real time.

---

## Contributors
- **Lavish Vaishnav** - [vaishnavlavish27@gmail.com](mailto:vaishnavlavish27@gmail.com)
- **Smruthi D Sharma** - [smruthisharma2003@gmail.com](mailto:smruthisharma2003@gmail.com)
- **Balaji K** - [balajik.0204@gmail.com](mailto:balajik.0204@gmail.com)
- **Disha C** - [dishagowda1625@gmail.com](mailto:dishagowda1625@gmail.com)

---

## References

1. **Md Zahidul Hassan, et al.** "Real-Time Computer Vision Based Autonomous Navigation System for Assisting Visually Impaired People using Machine Learning"
2. **A Rohit Kumar, et al.** "EchoGuide: Empowering the Visually Impaired with IoT-Enabled Smart Stick and Audio Navigation"
3. **Mansi Mahendru, Sanjay Kumar Dubey.** "Real Time Object Detection with Audio Feedback using Yolo vs. Yolo_v3"
4. **Heba Najm, et al.** "Assisting Blind People Using Object Detection with Vocal Feedback"

---

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

This README provides all the essential details about your project and makes it easy for others to understand and contribute. Let me know if you need further adjustments!
