# 🛣️ VGG16-UNet for Lane Segmentation

Welcome to the repository for **VGG16-UNet**, a deep learning model built for **road lane segmentation** using the power of **VGG16 as encoder** and a **U-Net-style decoder**! 🚗💨

<img width="850" height="566" alt="image" src="https://github.com/user-attachments/assets/3736508f-0fb6-4ccf-8442-0504d286ac5c" />

---

## 📌 Project Highlights

- 🔍 **Semantic Segmentation** focused on **lane detection**.
- 🧠 **VGG16** pre-trained encoder + custom decoder for semantic understanding.
- 💡 Clean, modular Jupyter Notebook for training and visualization.
- 📊 Metrics like **IoU** and **Dice Score** for evaluation.
- 🧪 Easy to test, tweak, and retrain on custom data.

---

## 🧠 Architecture Overview

The architecture is based on the classic **U-Net**, but with a twist: we replace the encoder with the convolutional layers from **VGG16** (without the top classification layers). This helps the model learn powerful low-level and mid-level features.

