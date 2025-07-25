# Explainable AI for Skin Disease Classification

[🔗 View Project on Kaggle](https://www.kaggle.com/code/tarikeloukili/explainable-ai-for-skin-disease-classification)

This project presents an **Explainable AI (XAI)** framework for classifying various types of skin diseases using **deep learning** and **machine learning** models. We combine performance with transparency by integrating interpretability tools like **LIME**, **SHAP**, and **Partial Dependence Plots (PDP)**.

---

##  Overview

Skin cancer detection from dermoscopic images is a critical challenge in medical diagnostics. This notebook uses:

- **CNN** to classify dermoscopic images  
- **XGBoost** on structured clinical metadata  
- **LIME**, **SHAP**, and **PDP** for interpretability

The goal is not only to achieve high accuracy but also to **explain model predictions**—building trust with medical professionals and aiding in decision-making.

> **Note**: This notebook was run in a Kaggle environment.  
>  [**Explore it directly on Kaggle**](https://www.kaggle.com/code/tarikeloukili/explainable-ai-for-skin-disease-classification)

---

##  Dataset: HAM10000

> "Human Against Machine with 10,000 training images"

**Data source**: [Kaggle – HAM10000 dataset](https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000)

- 10,015 dermoscopic images
- 7 skin disease categories:
  - Melanocytic nevi
  - Melanoma
  - Benign keratosis-like lesions
  - Basal cell carcinoma
  - Actinic keratoses
  - Vascular lesions
  - Dermatofibroma
- Includes both image data and clinical metadata (CSV)

---

##  Models Used

### 1. Convolutional Neural Network (CNN)
- Input: Dermoscopic images
- Output: Disease class
- Framework: TensorFlow / Keras

### 2. Gradient Boosting (XGBoost)
- Input: Structured metadata
- Output: Disease class
- Explainability: SHAP and PDP plots

---

##  Explainability Techniques

- **LIME**: Highlights influential image regions (CNN)
- **SHAP**: Displays feature-level impact (XGBoost)
- **PDP**: Visualizes feature influence globally (XGBoost)

---

##  How to Run

>  You can also run this project on Kaggle directly:  
> [ **Kaggle Notebook Link**](https://www.kaggle.com/code/tarikeloukili/explainable-ai-for-skin-disease-classification)

### Locally:

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/skin-disease-xai.git
   cd skin-disease-xai
