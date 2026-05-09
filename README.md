# Air Canvas: Real-Time Hand Gesture Drawing System 🎨🖐️

An interactive Computer Vision application that enables users to draw on a digital canvas using hand gestures. This project leverages deep learning and landmark detection to provide a touchless and intuitive drawing experience.

## 📌 Project Overview
This project is part of an academic exploration into AI-based interaction systems. By using **MediaPipe** for hand tracking and **OpenCV** for image processing, the system identifies the user's index finger as a virtual pen, allowing for seamless real-time interaction without any physical hardware or touch.

## ✨ Key Features
**High-Precision Tracking:** Utilizes MediaPipe Hands to track 21 3D hand landmarks at high frame rates.
* **Intelligent Gesture Logic:** Detects specific finger orientations to trigger drawing or pausing states automatically.
* **Mirrored Interaction:** Horizontal frame flipping ensures the user experiences natural, mirror-like movement.
* **Live Overlay:** Blends the drawing canvas with the webcam feed using weighted transparency for a professional visual effect.

## 🛠️ Technical Stack
* **Language:** Python
* **Core Libraries:** * `OpenCV`: For webcam stream management and canvas rendering.
    * `MediaPipe`: For real-time hand landmark detection.
    * `NumPy`: For matrix-based canvas manipulation.
* **Environment:** Developed and tested using Python 3.x and Flask.

## 📂 Project Structure
* `drawing_handtracking.py`: Main application script containing the detection logic and CV pipeline.
* `README.md`: Comprehensive project documentation.

## ⚙️ Setup and Installation

1. **Clone the Repository:**
   ```bash
   git clone git clone https://github.com/UmamaNoor174/drawing_handtracking.git
cd drawing_handtracking

2. **Install Dependencies:**
Run the following command to install required packages:
Bash
pip install opencv-python mediapipe numpy

3. **Run the Project:**
Bash
python drawing_handtracking.py

**Operational Guide**
1. Drawing Mode: Raise your Index Finger. The system tracks the tip (Landmark 8) and draws a line following your movement.

2. Pause Mode: Lower your index finger or close your fist. The system will stop drawing but maintain the current canvas state.

3. Exit: Press 'q' on your keyboard to safely terminate the application.

**Developer**
Umama Noor 
