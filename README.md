 Guidance-system-
 # 🎯 Real-Time Pedestrian Detection & Guidance System

A Python-based computer vision system that uses a live camera feed — either a Mac webcam or mobile phone camera — to detect pedestrians in real time using YOLO object detection and OpenCV. Detected individuals are highlighted with bounding boxes and tracked across frames.

---

 Demo
Live bounding boxes drawn around detected pedestrians using real-time camera input

How It Works

1. Captures a live video feed from either a Mac webcam or connected phone camera
2. Each frame is passed through a YOLO (You Only Look Once) object detection model
3. The model identifies pedestrians in the frame with a confidence score
4. Bounding boxes are drawn around each detected person in real time
5. The system runs continuously until manually stopped



Technologies Used

| Technology | Purpose |
|---|---|
| **Python** | Core programming language |
| **OpenCV** | Camera feed capture and frame processing |
| **YOLO** | Real-time object detection model |
| **NumPy** | Numerical operations on image arrays |

 Getting Started

### Prerequisites
Make sure you have Python 3.8+ installed. Then install the required libraries:

```bash
pip install opencv-python
pip install numpy
pip install ultralytics
```

### Running the System

Clone the repository:
```bash
git clone https://github.com/YOURUSERNAME/pedestrian-guidance-system
cd pedestrian-guidance-system
```

Run the detection system:
```bash
python guidance_system.py
```

To quit the live feed press **Q** on your keyboard.

 Camera Options

The system supports two camera input modes:

**Mac Webcam** — uses the built-in camera automatically when no external device is connected

**Phone Camera** — connect your phone as a webcam using a compatible app or USB connection, then update the camera index in the code:
```python
cap = cv2.VideoCapture(1)  # Change 0 to 1 for external camera
```



 Project Structure

```
pedestrian-guidance-system/
│
├── guidance_system.py      # Main detection script
├── requirements.txt        # Required libraries
└── README.md               # Project documentation
```


 Future Plans

- [ ] Add pedestrian counting across frames
- [ ] Track individual pedestrians with unique IDs
- [ ] Distance estimation from camera to detected person
- [ ] Alert system when pedestrian enters a defined zone
- [ ] Web dashboard showing live detection feed
- [ ] Support for pre-recorded video files



 What I Learned

- How to capture and process live video frames using OpenCV
- How YOLO processes each frame to detect objects in real time
- How bounding boxes are calculated and drawn on video frames
- Integrating a pre-trained deep learning model into a Python application
- Handling real-time data streams efficiently



 Author

Your Name**
IT, Business, Crim  Student — Xaverian college, Manchester 




 Licence

This project is open source and available under the [MIT Licence](LICENSE).
