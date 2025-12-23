<h1 align="center">🐾 Animal Detection with YOLO</h1>
<p align="center">
  Real-time animal detection using YOLOv8 & OpenCV — runs on webcam, images, or video.  
  Deployed as a simple web app and CLI tool.
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/Kif30/animal-detection-with-yolo/main/static/demo.gif" width="600" alt="Demo GIF (replace with your actual demo)" />
</p>

---

## 🚀 Project Overview

**Animal Detection with YOLO** leverages the power of the **YOLO (You Only Look Once)** object detection algorithm to detect animals in images, videos, and real-time webcam feeds.  
This project includes:
- 🐻 Pretrained YOLOv8 model for animal detection  
- 📸 CLI and web modes for inference  
- 🐍 Python + OpenCV implementation  
- 🖼️ Example assets for testing  

This system helps with **wildlife monitoring**, **video surveillance**, or **smart camera applications** where recognizing animals automatically is required.

---

---

## 🧠 Features
✔ Real-time detection (webcam or camera)  
✔ Detects animals from images & video  
✔ Responsive web interface  
✔ Easy CLI mode (`animal.py`)  
✔ Uses YOLOv8 pretrained weights for inference

---

## 📦 Tech Stack

| Tool | Purpose |
|------|---------|
| 🐍 Python | Main language |
| 👁️ OpenCV | Image/video processing |
| 🚀 YOLOv8 | Detection model |
| 🧠 Ultralytics | YOLOv8 framework |
| 🌐 Flask | Web UI |
| 🖥️ HTML/CSS | Frontend UI |
| 📦 requirements.txt | Dependency list |

---

## 🛠️ Installation

**1) Clone the repo**
git clone https://github.com/Kif30/animal-detection-with-yolo.git

cd animal-detection-with-yolo


**2) Create virtual env**


python -m venv venv
source venv/bin/activate # Linux/Mac
venv\Scripts\activate # Windows


**3) Install dependencies**
pip install -r requirements.txt

**4) Download YOLOv8 weights**
If not included, place your `yolov8.pt` in the root.

---

## 📌 Usage

### 🟡 Run as Web App
python app.py

Open in browser:


http://127.0.0.1:5000


### 🐍 Command-Line Detection
Detect on a single image:


python animal.py --source images/lion.jpg


Or on a video:


python animal.py --source videos/wild.mp4


Or real-time from webcam:


python animal.py --source 0

---

## 📊 How It Works

1. **Load YOLOv8 Model**  
   Pretrained weights loaded using Ultralytics YOLO library.

2. **Preprocess Image**  
   Convert frames to correct size/format.

3. **Run Inference**  
   Model outputs bounding boxes and class labels.

4. **Draw & Display Results**  
   Render detections using OpenCV.

---

## 💡 Example Outputs

> Add your screenshots or GIFs here to show detection results

![Lion detection](static/lion_1732362950.jpg)  
![Crocodile detection](static/crocodile_1742442611.jpg)

---

## 📈 Model Details

| Model | Description |
|-------|-------------|
| YOLOv8 | Real-time object detector trained on COCO or custom dataset |

You can replace the default `yolov8.pt` with:
- custom-trained weights
- a dataset of your choice

---

## 📦 Dependencies
This project uses:
Output will save processed image with detections.

---

## ⚙️ Tips for Custom Training
If you want custom models:
1. Label dataset with YOLO format
2. Train using Ultralytics CLI  
3. Replace `yolov8.pt` with your weights

*(similar workflow used in YOLO animal projects online)* :contentReference[oaicite:0]{index=0}

---

## 🧠 Notes
- Ensure correct Python version (3.8+ recommended)
- GPU recommended for real-time detection
- Use `--save` to store inference results

---

## 📫 Contact
👤 **Syed Akif** — https://github.com/Kif30  
💼 LinkedIn: https://www.linkedin.com/in/kif30

---


