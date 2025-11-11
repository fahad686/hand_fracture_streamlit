# 🦴 Hand Fracture Detection using YOLOv8 + Streamlit

This project deploys a **custom-trained YOLOv8 model** to detect **hand bone fractures** from X-ray images using an intuitive **Streamlit web interface**.  
It provides **real-time image detection**, **model performance analytics**, and **confusion matrix visualization** — all inside a modern, professional dashboard.

---

## 🚀 Features

- 🩻 Upload hand X-ray images or use a live camera (optional)  
- 🤖 Runs YOLOv8 inference using your trained `best.pt` model  
- 📊 Displays detection results (bounding boxes, confidence scores)  
- 📈 Generates model statistics and confusion matrix  
- 💬 User-friendly interface built with Streamlit  
- 🧠 Supports CPU/GPU inference  
- 🧩 Modular structure for easy extension and fine-tuning  

---

## 🧬 Model Details

- **Framework:** [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)  
- **Task:** Object Detection (Hand Fracture Detection)  
- **Weights:** `runs/detect/train/weights/best.pt`  
- **Input:** X-ray images of human hands  
- **Output:** Bounding boxes showing fracture regions with confidence values  

---

## 📂 Project Structure

hand_fracture_streamlit/
├── app.py # Main Streamlit web app
├── utils.py # Helper functions for inference and metrics
├── model/
│ └── best.pt # Trained YOLOv8 model weights
├── data/
│ ├── images/ # Test images for evaluation
│ └── labels/ # Ground-truth labels (YOLO format)
├── runs/ # YOLO training logs and metrics
├── requirements.txt # Python dependencies
└── Dockerfile # (Optional) for containerized deployment


---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/fahad686/hand-fracture-detection.git
cd hand-fracture-detection
