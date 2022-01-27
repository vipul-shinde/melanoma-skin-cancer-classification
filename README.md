[![forthebadge](https://forthebadge.com/images/badges/powered-by-coffee.svg)]()
[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)]()
[![forthebadge](images/badges/uses-deep-learning.svg)]()

<h1 align="center">Melanoma Skin Cancer Detection using Convolutional Neural Networks and Transfer Learning</h1>

<div align="center">

  [![Status](https://img.shields.io/badge/status-active-success.svg)]()
  [![License](https://img.shields.io/badge/license-MIT-blue.svg)]()
  ![GitHub repo size](https://img.shields.io/github/repo-size/vipul-shinde/melanoma-skin-cancer-classification)

</div>

---

<p align="center"> This is a Kaggle competition in which we have to identify if the given lesion image is malignant or not for Melanoma which is a type of skin cancer.
    <br>
</p>

## 📝 Table of Contents

- [🧐 About](#about)
- [📊 Dataset Overview](#data-overview)
- [🧠 Model Building](#neural-network-model)
- [🎯 Model Performance](#model-performance)
- [🏅 Model Evaluation](#model-evaluation)

## 🧐 About <a name = "about"></a>

Melanoma is a type of skin cancer that occurs when pigment-producing cells (melanocytes) mutate and become cancerous. Melanoma is the most serious form of skin cancer and 5th most common cancer. 

The American Cancer Society estimates around 207,390 new melanoma cases will be diagnosed in 2021. As with other cancers, early and accurate detection—potentially aided by data science—can make treatment more effective.

Currently, dermatologists evaluate every one of a patient's moles to identify outlier lesions that are most likely to be melanoma.

## 📊 Dataset Overview <a name="data-overview"></a>

The dataset was taken from the competition hosted by <a href = "https://www.kaggle.com/c/siim-isic-melanoma-classification/data">SIIM-ISIC</a> on Kaggle.

<p align="center">
    <img src="images\data-overview.png" alt="data-overview" width="500px">
</p>

- Malignant: A cancerous growth that can spread very quickly and invade nearby tissues
- Benign: A non-cancerous growth that usually grows very slowly and does not spread to other areas

### Click to view 👇:

[![forthebadge](images/badges/solution-exploratory-data-analysis.svg)](https://github.com/vipul-shinde/melanoma-skin-cancer-classification/blob/main/notebooks/01-eda-and-tabular-data-model.ipynb)

## 🧠 Model Building <a name="neural-network-model">

Here, the bottom layers of pre-trained Xception model were used and the top layers were fine-tuned for our particular task to classify skin cancer images as malignant or not. The architecture of xception model is as follows:

<p align="center">
    <img src="images\xception-architecture.png" alt="xception-architecture">
</p>

## 🎯 Model Performance <a name="model-performance">

Since the dataset is highly imbalanced, accuracy wouldn't be a good metric to judge the model performnace hence we have used the AOC as a performance metric along with BinaryCrossentropy as the loss function. Here is the model's performance.

<p align="center">
    <img src="images\live-loss-plot.png" alt="live-loss-plot" width="500px">
</p>

<p align="center">
    <img src="images\performance-results.png" alt="performance-result" width="600px">
</p>

## 🏅 Model Evaluation <a name="model-evaluation">

We evaluated our model on the test dataset and we were able to achieve an AUC of 0.8459. Here is the curve:

<p align="center">
    <img src="images\auc-curve.png" alt="auc-curve" width="500px">
</p>

<p align="center">
    <img src="images\test-data-evaluation.png" alt="test-data-evaluation" width="600px">
</p>

### Click to view 👇:

[![forthebadge](images/badges/solution-transfer-learning-using-xception-model.svg)](https://github.com/vipul-shinde/melanoma-skin-cancer-classification/blob/main/notebooks/02-transfer-learning-using-xception.ipynb)

# Thank you!