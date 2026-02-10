# UrbanVision 🏙️

**UrbanVision** is an end-to-end, resource-efficient pipeline for **bitemporal 3D change detection** designed specifically for **edge computing environments**. The system compares 3D point cloud scans of the same urban area captured at different times to detect **new constructions, demolitions, and structural/environmental changes** with high accuracy.

This project was developed and validated on **Raspberry Pi 4B**, focusing on lightweight models, minimal computation, and practical deployability.

---

## 🚀 Key Features

* 🔄 **Bitemporal Change Detection** using 3D point clouds
* ⚡ **Edge-optimized pipeline** with low computational overhead
* 🧠 Supports **multiple ML/DL models** (classical + deep learning)
* 🗂️ Custom **parser for non-standard point cloud formats**
* 🧪 Model comparison across accuracy, size, and inference speed
* 📦 Ready for **real-world urban monitoring & disaster assessment**

---

## 🧠 Methodology Overview

The pipeline follows these major stages:

1. **Data Acquisition** – Bitemporal 3D scans of the same region
2. **Data Preprocessing** – Cleaning, normalization, and alignment
3. **Feature Extraction** – Geometric and statistical features
4. **Model Training & Selection** – Lightweight and efficient models
5. **Edge Deployment** – Inference on Raspberry Pi 4B

---

## 📊 Dataset

* **Dataset Used:** Urb3DCD (Simulated urban dataset – Lyon, France)
* **Data Type:** Bitemporal 3D point clouds (XYZ + RGB)
* **Challenge:** Non-standard file format (incompatible with Open3D)
* **Solution:** Custom-built parser to load and preprocess data correctly

---

## 🤖 Models Used

UrbanVision experiments with a mix of classical ML and deep learning models, including:

* XGBoost
* Lightweight neural networks
* Optimized classical classifiers

Model selection prioritizes:

* Accuracy
* Inference latency
* Model size (edge constraints)

📌 **Pre-trained and optimized models are available under GitHub Releases**:
👉 [https://github.com/rushi-k12/UrbanVision/releases/tag/models-v1](https://github.com/rushi-k12/UrbanVision/releases/tag/models-v1)

You can directly download and use these models for inference without retraining.

---

## 📈 Results

* Accurate detection of **changed vs unchanged regions**
* Strong performance even with **limited compute resources**
* Clear visual distinction:

  * 🟥 Red: Changed regions
  * 🟩 Green: Unchanged regions

Comparative analysis across models highlights the trade-off between accuracy and efficiency for edge deployment.

---

## 🖥️ Edge Deployment

* **Target Device:** Raspberry Pi 4B
* **Inference:** Fully offline, minimal network dependency
* **Deployment Goal:** Real-time or near real-time urban monitoring

---

## 🔮 Future Scope

* 🔧 Model quantization for further size reduction
* ⏱️ Real-time streaming point cloud processing
* 🌍 Validation on real-world LiDAR datasets
* 🤖 Improved generalization across sensors & environments

---

## 🎥 Demo & Links

* **Live Demo:** [https://connect.raspberrypi.com/devices](https://connect.raspberrypi.com/devices)
* **YouTube Demo:** [https://youtu.be/FS80BiFMFN8](https://youtu.be/FS80BiFMFN8)

---

## 📄 Publication

This work was presented at:

**5th International Conference on Advanced Network Technologies and Intelligent Computing (ANTIC-2025)**
Paper ID: 396

**Authors:**

* Rushikesh Kusuma
* Vamshidhar Narsingoji
* Sahil Jaiswal
* Kiran Kumar Pattanaik

---

## ⭐ Acknowledgements

If you find this project useful, consider starring ⭐ the repository and exploring the released models.

Feel free to open issues or contribute!
