# house-damage-image-severity-classification
End-to-end image classification solution to identify house damage types (fire, water, wind, lightning, normal) using deep learning, with business-friendly explanations and a fully documented Jupyter notebook.

# 🏠 House Damage Image Classification

An end-to-end deep learning project that classifies house damage images into categories such as **Fire Accident, Water Damage, Wind Damage, Lightning Damage, and Normal**, using transfer learning.  
This repository is designed to be **understandable by non-AI users**, with detailed explanations embedded directly into the Jupyter notebook.

---

## 📌 Business Problem

In insurance claim processing and damage assessment:
- Manual inspection of house damage images is **time-consuming**
- Damage categorization can be **subjective**
- Rare but critical damages (e.g., lightning) are often underrepresented

This project demonstrates how **AI can assist damage classification** from images in a **transparent and explainable way**, suitable for Proof of Concept (PoC) and pilot implementations.

---

## 🎯 Objectives

- Classify house damage images into predefined categories
- Use a **pre-trained deep learning model** for better accuracy with limited data
- Handle **class imbalance** effectively
- Provide **business-friendly explanations** for every step
- Enable **image-level predictions with confidence scores**

---

## 🗂️ Damage Categories

- Fire Accident  
- Water Damage (Plumbing)  
- Wind Damage
-  Tree Damage  
- Lightning Damage  
- Normal (No Damage)

---

## 🧠 Approach (High Level)

1. **Image Preprocessing**
   - Resize images to a standard format
   - Normalize image values for consistency

2. **Transfer Learning**
   - Uses a pre-trained **ResNet-18** model
   - Only the final classification layers are trained

3. **Class Imbalance Handling**
   - Rare damage types are given higher importance during training

4. **Model Evaluation**
   - Accuracy, precision, recall
   - Confusion matrix for easy interpretation

5. **Explainability**
   - Every notebook cell contains plain-English explanations
   - Designed for non-AI and business stakeholders

---

## 📁 Repository Structure

