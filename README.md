# 🛣️ VGG16-UNet for Lane Segmentation

This repository contains a lane segmentation project using **VGG16 as encoder** and a **U-Net-style decoder** for pixel-wise road lane detection.  
Built entirely in **TensorFlow** and executed step-by-step in a **Jupyter Notebook**.

<img width="980" height="465" alt="Screenshot from 2025-07-17 16-52-20" src="https://github.com/user-attachments/assets/af49d27b-ca1a-4985-8e9e-29926747e4a7" />

Figure 1. VGG16 Architecture

<img width="836" height="559" alt="Screenshot from 2025-07-17 17-02-32" src="https://github.com/user-attachments/assets/f5fc7809-227d-4eff-a174-ee25e7c24eae" />

Figure 2. U-Net encoder-decoder Architecture

---

## 📁 Folder Structure
Folder Structure should be like that

VGG16-UNet/

├── VGG16-Unet.ipynb ← Training & testing notebook

├── requirements.txt ← All dependencies

├── dataset/

---

## 🧠 Model Architecture

This project uses a **pre-trained VGG16** encoder (without the top classifier) and a decoder with skip connections, similar to the classic U-Net.

**Input → VGG16 Encoder → Bottleneck → Decoder → Segmentation Mask**
- Input shape: `(244, 244, 3)`
- Output shape: `(244, 244, 1)`
- Activation: `sigmoid`
- Loss Function: `Dice Loss`
- Metrics: `IoU`, `Accuracy`

---
## ✅ Setup

### 1️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

⚠️ TensorFlow Note:
If you're using a CPU-only system or one without AVX-512 support, avoid latest TensorFlow versions. Use tensorflow==2.10.1 as included in this file.

### 2️⃣ Dataset 
Download Dataset in here: https://www.kaggle.com/datasets/manideep1108/tusimple

## 📈 Results & Metrics

<img width="1216" height="444" alt="Screenshot from 2025-07-17 17-07-27" src="https://github.com/user-attachments/assets/032ea15c-889e-4da4-ba86-71c1aad7596a" />


During training, the notebook will log:

Training vs Validation Loss

IoU (Intersection over Union)

Accuracy

Random sample visualizations

---
17.07.25-17.12
<img width="756" height="1157" alt="image" src="https://github.com/user-attachments/assets/aa4b6a3b-aabb-43e7-98b7-1a70edecc10e" />
---

## Model h5 file: https://drive.google.com/file/d/1aYe1wwqYwhZG3bFNMnkH17l6vyF-3CwA/view?usp=sharing
---

