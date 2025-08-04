# 🧠 Multi-Modal AI System for Real-Time Driver Drowsiness and Distraction Detection

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Python](https://img.shields.io/badge/Python-3.8%2B-green) ![Status](https://img.shields.io/badge/status-WIP-orange)

---

## 🚗 Overview

Driver drowsiness is a leading cause of road accidents. This AI system detects driver fatigue and distraction in **real-time** using a combination of:
- Facial landmarks (eye blink, yawning)
- Head pose estimation
- Temporal patterns via LSTM

The system uses **OpenCV**, **deep learning models (CNN + LSTM)**, and **Streamlit** for a smooth real-time dashboard.

---

## 💡 Features

- 🎥 Real-time video processing from webcam
- 💤 Blink and yawn detection
- 🔄 Temporal analysis using LSTM
- 🎯 Distraction score + Alert system
- 📊 Streamlit-based live dashboard (or PyQt)
- ⚡ Docker-ready deployment

---

## 🧰 Tech Stack

| Component | Technology |
|----------|------------|
| Language | Python 3.8+ |
| ML/DL    | OpenCV, TensorFlow / PyTorch, Scikit-learn |
| App      | Streamlit (or PyQt GUI) |
| Infra    | Docker (optional), Git |
| Optional | ONNX / TensorRT for edge deployment |

---

## 📁 Project Structure

driver-drowsiness-ai/
│
├── data/ # Instructions to download large datasets
│ └── README.md
├── notebooks/ # EDA and prototyping
│ └── 0_data_explore.ipynb
├── models/ # Saved models
├── src/ # Core logic
│ ├── detect_face.py
│ ├── blink_detector.py
│ ├── drowsiness_score.py
│ └── utils.py
├── app/ # UI code (Streamlit or PyQt)
│ └── app.py
├── report/ # Plots, architecture diagrams, PDF summary
├── requirements.txt # All Python dependencies
├── .gitignore
└── README.md

---

## 🧪 Dataset

This project uses public datasets for training:

- [YawDD – Yawning Detection Dataset](https://github.com/MayankSingal/Yawn-Detection-Dataset)
- [CEW – Closed Eyes in the Wild](https://github.com/zzh8829/yawn-detection-dataset)
- [RT-GENE Head Pose](https://github.com/Tobias-Fischer/rt-gene)

📝 Due to GitHub size limits, datasets are not included here.  
👉 Download from links above and place in `/data` folder.  

---

## 🚀 Getting Started

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/driver-drowsiness-ai.git
cd driver-drowsiness-ai```
2. **Create a virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate```
3. Install dependencies
pip install -r requirements.txt
4. Run the app
streamlit run app/app.py
📦 To Do (WIP)
^^ Add LSTM model for temporal analysis

^^ Build alerting system (sound/email)

^^ Optimize with ONNX or TensorRT

^^ Mobile/Edge support (TFLite/Jetson)
## 📄 License
This project is licensed under the MIT License – see the LICENSE file for details.

**💬 Contact**
Built with ❤️ by Yash Bhardwaj
Feel free to reach out via LinkedIn(www.linkedin.com/in/yash-bhardwaj-b28828290 ) or open an issue!
