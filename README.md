# 🛰️ GeoAI Hackathon - Top 3 Kaggle Solution

## 🚀 Overview

This repository showcases my approach and solution for the **GeoAI Hackathon**, where I proudly secured a **Top 3 position** on the leaderboard. The competition's goal was to detect locust breeding grounds using satellite imagery, harnessing the power of geospatial data and deep learning techniques.

## 🔍 Problem Statement

The challenge was to accurately identify locust breeding grounds across Africa using satellite imagery. Successful detection could help mitigate the devastating impact of locust swarms on agriculture and food security.

## 🧠 Approach

I divided my solution into two key phases, leveraging state-of-the-art models and fine-tuning strategies for optimal performance.

---

### Phase 1 - Prithvi 1.0 + InstaGeo Model

- **Model:** Prithvi 1.0 (backbone) combined with the InstaGeo Model.
- **Loss Function:** Replaced Cross Entropy Loss with **Focal Loss** to handle class imbalances and improve segmentation of hard-to-classify pixels.
- **Training:** Trained for **7 epochs**.

✅ **Why this worked?**

- **Proven performance:** Prithvi 1.0 excels in geospatial tasks, offering robust feature extraction.
- **Focal Loss advantage:** Focused training on difficult pixels, improving overall segmentation accuracy and handling class imbalance.

---

### Phase 2 - Fine-tuning Prithvi 2.0 (300M TL)

- **Model:** Switched to **Prithvi 2.0 (300M TL)** as the backbone.
- **Fine-tuning:** Applied transfer learning, fine-tuning the model on the provided dataset.
- **Hyperparameter Optimization:** Extensively experimented with:
  - Learning rates
  - Batch sizes
  - Weight decay

✅ **Why Prithvi 2.0 (300M TL) was relevant?**

- **Temporal-Spatial Pattern Recognition:** Pre-trained on Earth Observation (EO) data, making it effective at capturing locust habitat dynamics.
- **Transfer Learning Benefits:** Generalized well to unseen conditions and ecological zones.
- **Multi-Scale Feature Learning:** Analyzed fine-grained and large-scale patterns, enhancing detection accuracy.
- **Temporal Variations:** Recognized shifts in locust breeding grounds over time, improving segmentation robustness.

---

## 📊 Dataset

- **Source:** Provided by the GeoAI Hackathon organizers.
- **Content:** Satellite imagery of Africa with annotations for locust breeding grounds.
- **Data Preparation:** Created and downloaded using the **InstaGeo tool** by InstaDeep.

👉 Dataset link: [GeoAI Hackathon on Kaggle](https://www.kaggle.com/competitions/geo-ai-hack/overview)

---

## ⚙️ Tech Stack

- **Frameworks:** PyTorch
- **Models:** Prithvi 1.0, Prithvi 2.0 (300M TL)
- **Tools:** InstaGeo, OpenCV, NumPy, Pandas, Matplotlib
- **Environment:** NVIDIA GPUs (for model training and inference)

---

## 🏆 Results

- Achieved a Top 3 leaderboard position among competitive entries.
- Improved segmentation accuracy for locust breeding ground detection.
- Enhanced temporal robustness through fine-tuning and multi-scale feature learning.

---

## 🙌 Acknowledgment

A huge thanks to the **GeoAI Hackathon** organizers — **InstaDeep**, **Datacraft**, and **AFD** — for this amazing opportunity and challenging dataset. Special thanks to **InstaDeep** for their innovations in geospatial AI and the invaluable InstaGeo tool.

---

⭐️ **If you find this repository helpful, don’t forget to give it a star!**
