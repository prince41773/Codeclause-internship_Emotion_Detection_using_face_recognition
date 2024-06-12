# Emotion Detection Flask App

This Flask application allows users to upload images or videos and detect emotions in faces using a pre-trained deep learning model. The app also supports real-time emotion detection using a webcam.

## Features
- Image Emotion Detection
- Video Emotion Detection
- Real-time Webcam Emotion Detection

## Setup

### Prerequisites

- Python 3.6+
- Flask
- OpenCV
- TensorFlow
- NumPy

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/prince41773/Codeclause-internship-Face_Recognition_Application.git
    cd emotion-detection-app
    ```

2. Create and activate a virtual environment:
    ```sh
    python3 -m venv venv
    source venv/bin/activate
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

4. Download the pre-trained model files and place them in the `model` directory:
    - `emotion_model.json`
    - `emotion_model.h5`
    - You can use a model trained on the FER2013 dataset or any other emotion detection model.

5. Download the Haar Cascade classifier for face detection and place it in the `haarcascades` directory:
    - `haarcascade_frontalface_default.xml`

### Running the Application

1. Start the Flask application:
    ```sh
    python app.py
    ```

2. Open your web browser and go to `http://127.0.0.1:5000`.

## Usage

### Image Emotion Detection

1. Navigate to the home page.
2. Upload an image file (supported formats: PNG, JPG, JPEG).
3. The processed image with detected emotions will be available for download.

### Video Emotion Detection

1. Navigate to the home page.
2. Upload a video file (supported formats: MP4, AVI, MOV, MKV).
3. The processed video with detected emotions will be available for download.

### Real-time Webcam Emotion Detection

1. Navigate to the camera page by clicking on the "Live Camera" link.
2. Allow the browser to access your webcam.
3. The real-time emotion detection feed will be displayed.

## Directory Structure

```plaintext
emotion-detection-app/
│
├── app.py
├── templates/
│   ├── index.html
│   ├── camera.html
│
├── static/
│   └── (optional static files like CSS, JS)
│
├── model/
│   ├── emotion_model.json
│   └── emotion_model.h5
│
├── haarcascades/
│   └── haarcascade_frontalface_default.xml
│
├── uploads/
│   └── (uploaded files)
│
├── processed/
│   └── (processed files)
│
├── requirements.txt
└── README.md
