# Face Recognition using OpenCV

Try out real-time face detection with your webcam using OpenCV’s Haar Cascade classifier.

## Features

- Live webcam feed with face detection
- Draws bounding boxes around detected faces
- Simple keyboard control to quit

## Requirements

- Python 3.x
- Jupyter Notebook
- OpenCV (`cv2`)
- A working webcam

Install dependencies:
```bash
pip install opencv-python
```

## Usage

1. Open `facerecognition.ipynb` in Jupyter Notebook.
2. Run the notebook cell to start the camera.
3. Press `q` to quit the window.

## How It Works

- Loads the Haar cascade file: `haarcascade_frontalface_default.xml` from `cv2.data.haarcascades`.
- Captures frames from your default camera (index `0`).
- Converts each frame to grayscale and detects faces with `detectMultiScale`.
- Draws rectangles around detected faces and shows the live video.

---

Experiment with basic face detection in real time!
