# Explainable AI for Skin Disease Classification

This project presents an **Explainable AI (XAI)** framework for classifying various types of skin diseases using **deep learning** and **machine learning** models. We combine performance with transparency by integrating interpretability tools like **LIME**, **SHAP**, and **Partial Dependence Plots (PDP)**.

##  Overview

Skin cancer detection from dermoscopic images is a critical challenge in medical diagnostics. This notebook uses:

- **CNN** to classify dermoscopic images
- **XGBoost** on structured clinical metadata
- **LIME**, **SHAP**, and **PDP** for interpretability

The goal is not only to achieve high accuracy but also to **explain model predictions**—building trust with medical professionals and aiding in decision-making.


> **Note**: This notebook was run in a Kaggle environment.

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
- Highlights:
  - Automated feature extraction
  - Image preprocessing and augmentation

### 2. Gradient Boosting (XGBoost)
- Input: Structured metadata
- Output: Disease class
- Explainability: SHAP and PDP plots

---

##  Explainability Techniques

###  LIME (Local Interpretable Model-Agnostic Explanations)
- Applied to CNN predictions
- Highlights influential regions in an image

###  SHAP (SHapley Additive exPlanations)
- Applied to XGBoost model
- Shows feature importance and individual contributions

###  PDP (Partial Dependence Plots)
- Visualizes marginal effects of features on prediction

---

##  How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/skin-disease-xai.git
   cd skin-disease-xai
   ```

2. **Download the dataset**
   - From [Kaggle HAM10000](https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000)
   - Place images and CSV in the expected directory paths

3. **Run the notebook**
   ```bash
   jupyter notebook skin-disease-classification_with_explanation.ipynb
   ```

---

##  Results (Example)

- CNN Accuracy: ~85%+
- XGBoost F1-score: ~80%+
- SHAP summary plots reveal top 5 features impacting diagnosis
- LIME heatmaps show interpretable image regions

---

##  Project Structure

```
 skin-disease-xai/
├── skin-disease-classification_with_explanation.ipynb
├── README.md


```

---


##  License

This project is licensed under the MIT License.
