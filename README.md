# Deep Learning–Based Arabic Sign Language Recognition for Medical Emergency Communication

This repository contains the implementation and experimental study of a **Deep Learning–based Arabic Sign Language (ArSL) recognition system** developed as part of the **Deep Learning course project**.  
The project focuses on recognizing **medical emergency–related Arabic signs** to support fast and effective communication for deaf and hard-of-hearing individuals.

---

## 📌 Project Overview
During medical emergencies, clear and rapid communication is critical. Arabic Sign Language recognition systems are still limited, especially in **emergency contexts**.  
This project explores and compares multiple **deep learning architectures** to identify the most suitable approach for recognizing **emergency-related ArSL signs**.

---

## 🎯 Objectives
- Focus on **medical emergency communication** using Arabic Sign Language
- Select a relevant subset of signs from the **KArSL-502 dataset**
- Evaluate multiple deep learning models for **spatial and temporal understanding**
- Identify the most effective model for real-world emergency scenarios

---

## 📊 Dataset
- **Dataset:** KArSL-502 (Kaggle)
- **Type:** Word-level Arabic Sign Language videos
- **Total Signs:** 502  
- **Selected Subset:** 131 medically relevant signs
- **Samples:** 19,650 video sequences  
- **Signers:** 3 professional signers  
- **Data Format:** RGB video frames

---

## 🧠 Models Implemented
The following deep learning models were implemented and evaluated:

- **ResNet**
- **ResNet + BiLSTM**
- **I3D (Inflated 3D CNN)**
- **VideoMAE (Transformer-based video model)**
- **MediaPipe + SignBart (Skeleton-based Transformer model)**

Each model was tested under:
- **Signer-Independent settings**
- **Mixed-Signer settings**

---

## ⚙️ Training Configuration
- **Framework:** PyTorch
- **Optimizer:** Adam / AdamW
- **Loss Function:** Cross-Entropy Loss
- **Evaluation Metrics:**
  - Accuracy
  - Precision
  - Recall
  - Macro F1-Score
- **Data Split:** Train / Validation / Test (no data leakage)

---

## 📈 Key Results
- **VideoMAE** achieved the highest performance  
  - ~96–97% accuracy in mixed-signer experiments
- **I3D** demonstrated strong spatiotemporal learning  
  - ~85% accuracy
- **MediaPipe + SignBart** showed strong **generalization ability**  
  - Skeleton-based approach reduces noise and improves robustness
- Frame-only models (ResNet) performed poorly in signer-independent settings

---

## 🔍 Key Takeaways
- Temporal modeling is essential for Arabic Sign Language recognition
- Transformer-based models excel at capturing complex sign dynamics
- Skeleton-based approaches are promising for **privacy-preserving** and **real-time** systems
- Emergency-focused sign recognition requires specialized datasets and evaluation strategies


