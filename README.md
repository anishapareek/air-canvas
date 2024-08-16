# Air Canvas with OpenCV and Mediapipe

## Project Description

This project implements a fascinating computer vision application using **OpenCV** and **Mediapipe**. Ever wanted to draw your imagination just by waving your finger in the air? This project, known as **Air Canvas**, allows you to draw anything on a digital canvas simply by moving your hand. The system detects hand landmarks, specifically tracking the index finger, allowing for intuitive, real-time drawing in mid-air.

This project not only showcases the power of **OpenCV** in handling computer vision tasks but also leverages **Mediapipe's** machine learning capabilities for hand tracking.

### Key Features:
- Real-time hand landmark detection and tracking using Mediapipe.
- Drawing by tracking the index finger's motion.
- Customizable ink colors via a simple UI.

### Project Overview:

- **Hand Landmarks Detection and Tracking**: This project uses Mediapipe's hand detection module to detect and track hand landmarks, especially focusing on the index finger to create the drawing motion.
  
- **Computer Vision with OpenCV**: The project employs OpenCV for frame manipulation, color space conversion, and drawing operations on the digital canvas.

---

### Algorithm Overview:

1. **Frame Capture and Color Conversion**:
   - Start capturing frames from the webcam.
   - Convert the captured frames to HSV color space for easier color detection.

2. **Canvas Initialization**:
   - Prepare a canvas frame and add UI elements, including color selection buttons and a clear button.

3. **Mediapipe Initialization**:
   - Set up the Mediapipe hand tracking module to detect a single hand for this project.

4. **Landmark Detection**:
   - Pass the RGB frame to the Mediapipe hand detector.
   - Detect hand landmarks and extract the coordinates of the index finger.

5. **Drawing on the Canvas**:
   - Track the motion of the index finger by storing successive coordinates in an array.
   - Use these coordinates to draw on both the video feed and the canvas.

### Requirements:

To run this project, you will need:
- Python 3
- Numpy
- OpenCV
- Mediapipe

### How to Install the Dependencies:

```bash
pip install numpy opencv-python mediapipe
```

### How to Run:

1. Clone the repository.
2. Install the required libraries.
3. Run the script using Python 3:
   ```bash
   python air_canvas_ml.py
   ```

---

### Screenshot:

Here is a snapshot of the Air Canvas in action:
<img width="1442" alt="AirCanvas" src="https://github.com/user-attachments/assets/4c199522-0508-4cf6-a73d-1d6466280411">

---
