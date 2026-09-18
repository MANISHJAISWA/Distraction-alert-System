# 🎯 Distraction Alert System for Online Meeting

## 📌 Project Overview

The **Distraction Alert System for Online Meeting** is a computer-vision-based system designed to monitor a user's attention during online meetings or virtual learning sessions.

The system uses the computer's camera to analyze the user's face and provide an alert when the user is detected as distracted. It also performs **facial emotion analysis** and displays the detected emotion information.

The project is developed using **Python, OpenCV, DeepFace, TensorFlow, NumPy, Matplotlib, and PyVirtualCam**.

---

## 🎯 Objectives

* Monitor user attention during online meetings.
* Detect whether a user's face is present in the camera frame.
* Identify distracted/attentive states.
* Generate an alert when distraction is detected.
* Analyze facial emotions using DeepFace.
* Display emotion information on the video frame.
* Maintain an attention log for attentive and distracted states.
* Provide visual and audio alerts.
* Support virtual camera functionality.

---

## ✨ Features

### 👤 Face Monitoring

The system processes the camera feed using OpenCV and monitors the user's face.

### 🚨 Distraction Alert

When the user is detected as distracted for the configured threshold, the system generates an alert.

### 🔊 Audio Alert

The system can produce an audio alert when distraction is detected.

### 😊 Emotion Detection

DeepFace is used to analyze facial emotions and display emotion confidence percentages.

### 📊 Live Visualization

Matplotlib is used to display live information such as:

* Emotion analysis
* Attentive time
* Distracted time

### 📝 Attention Logging

The system maintains an `attention_log` containing attentive and distracted states.

### 📹 Virtual Camera

`pyvirtualcam` is included to support virtual-camera functionality for online meeting applications.

---

## 🛠️ Technologies Used

| Technology   | Purpose                                  |
| ------------ | ---------------------------------------- |
| Python       | Main programming language                |
| OpenCV       | Computer vision and camera processing    |
| DeepFace     | Facial emotion analysis                  |
| TensorFlow   | Deep-learning framework used by DeepFace |
| NumPy        | Numerical processing                     |
| Matplotlib   | Live graphs and visualization            |
| PyVirtualCam | Virtual camera support                   |
| Threading    | Background processing                    |
| OBS Studio   | Project demonstration / screen recording |

> **Note:** OBS Studio was used for recording/demonstrating the project. It is not a core component of the distraction-detection algorithm.

---

## ⚙️ Main Libraries

```text
opencv-python
deepface
tensorflow
numpy
matplotlib
pyvirtualcam
tf-keras
```

---

## 📂 Project Structure

```text
Distraction-Alert-System/
│
├── Distraction Alert System.ipynb
├── README.md
└── requirements.txt
```

---

## 🔄 System Workflow

```text
Camera Input
     ↓
OpenCV Frame Processing
     ↓
Face Detection
     ↓
Attention / Distraction Analysis
     ↓
Emotion Analysis using DeepFace
     ↓
Display Alert + Emotion Information
     ↓
Attention Logging
     ↓
Live Graph Visualization
```

---

## 🚨 Alert Mechanism

The project uses a configurable alert threshold:

```python
ALERT_THRESHOLD_SECONDS = 3.0
```

When the distraction condition continues beyond the configured threshold, the system generates an alert.

The alert mechanism supports different operating systems, including Windows, macOS, and Linux.

---

## 😊 Emotion Analysis

The system uses DeepFace to analyze facial emotions.

The emotion analysis is performed periodically rather than on every frame:

```python
EMOTION_ANALYSIS_INTERVAL_FRAMES = 15
```

The detected emotions and their confidence percentages are displayed on the video frame.

---

## 📊 Attention Monitoring

The project maintains an attention log:

```python
attention_log = []
```

The log records states such as:

```text
attentive
distracted
```

These values are used to generate attention-related visualizations.

---

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/distraction-alert-system.git
```

### 2. Open the Project

```bash
cd distraction-alert-system
```

### 3. Install Required Libraries

```bash
pip install opencv-python numpy matplotlib deepface tensorflow pyvirtualcam tf-keras
```

### 4. Run the Notebook

Open:

```text
Distraction Alert System.ipynb
```

using Jupyter Notebook, JupyterLab, or Google Colab where the required dependencies and camera/GUI functionality are supported.

### 5. Start the Camera

Run the notebook cells and allow access to the webcam.

---

## 🎥 Project Demonstration

**OBS Studio** was used to record the project demonstration and showcase the working of the Distraction Alert System.

The demonstration can show:

* Camera input
* Face monitoring
* Distraction alert
* Audio alert
* Emotion detection
* Attention visualization

---

## 🔮 Future Scope

The system can be further enhanced with:

* More accurate eye-gaze detection.
* Face-landmark-based attention estimation.
* Automatic focus-time calculation.
* CSV or database-based attendance/attention reports.
* Firebase integration.
* Multiple-user monitoring.
* Admin dashboard.
* Integration with online meeting platforms.
* Improved distraction classification using machine learning/deep learning.
* Additional behavioral indicators for attention monitoring.

---

## ⚠️ Disclaimer

This project is developed for **educational and demonstration purposes**. Facial emotion and attention predictions are algorithmic estimates and should not be treated as definitive measurements of a person's actual mental state or intentions.

---

## 👨‍💻 Author

**Manish Jaiswal**

Computer Science / AIML Student

---

## ⭐ Project

If you find this project useful for learning computer vision and AI-based attention monitoring, consider giving the repository a ⭐.
