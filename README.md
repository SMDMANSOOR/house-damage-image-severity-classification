# house-damage-image-severity-classification
End-to-end image classification solution to identify house damage types (fire, water, wind, lightning, normal) using deep learning, with business-friendly explanations and a fully documented Jupyter notebook.

# 🏠 House Damage Image Classification

An end-to-end deep learning project that classifies house damage images into categories such as **Fire Accident, Water Damage, Wind Damage, Lightning Damage, and Normal**, using transfer learning.  

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
house-damage-image-classification/
│
├── data/
│ ├── train/
│ │ ├── Fire_Accident/
│ │ ├── Water_Damage_Plumbing/
│ │ ├── Wind_Tree_Damage/
│ │ ├── Lightning_Damage/
│ │ └── Normal/
│ │
│ └── test/
│ ├── Fire_Accident/
│ ├── Water_Damage_Plumbing/
│ ├── Wind_Tree_Damage/
│ ├── Lightning_Damage/
│ └── Normal/
│
├── House_Damage_Classification_EXPLAINED_FOR_BUSINESS.ipynb
├── README.md



## 📉 Known Limitation: Small Dataset Impact

This project is intentionally built using a **limited number of training images** to demonstrate a Proof of Concept (PoC).

Due to the **small dataset size**:
- Some damage categories may be **misclassified**
- Visually similar damages (e.g., fire vs. wind damage) may confuse the model
- Rare damage types (such as lightning damage) may have lower confidence scores

This behavior is **expected** in deep learning models when trained on limited data.

### 🔍 Why This Happens
Deep learning models learn patterns from examples.  
With fewer images:
- The model cannot see enough variations of each damage type
- It may learn incomplete or biased patterns

### 🚀 How This Can Be Improved
With a **larger and more diverse dataset**, model performance can be significantly improved by:
- Adding more images per damage category
- Including variations in lighting, angles, and severity
- Balancing rare and frequent damage types
- Fine-tuning the model for additional training epochs

With sufficient data, the observed misclassification issues are expected to be **significantly reduced or eliminated**.


## 🐍 Environment & Kernel Information

- **Python Version:** 3.9.x  
- **Jupyter Kernel:** Python 3.9 (ipykernel)

This notebook was developed and tested using **Python 3.9**.  
For best compatibility and consistent results, it is recommended to run the notebook using the same Python version.
