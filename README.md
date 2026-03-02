# Satellite Insight Engine: Water Body Segmentation

This project implements a Deep Learning model to automatically detect and map water bodies in satellite imagery. Using a **U-Net architecture**, the model performs pixel-level classification to distinguish between water and land. This project is an evolution of previous research focused on analyzing urban water level changes in **Mumbai**.

> **Note:** This is my **first time** building and training a Neural Network from scratch! 🚀



## 🚀 Project Overview
* **Objective**: Automate the detection of lakes, rivers, and oceans from satellite photos.
* **Model**: Mini U-Net (Encoder-Decoder Architecture).
* **Dataset**: [Satellite Images of Water Bodies](https://www.kaggle.com/datasets/franciscoescobar/satellite-images-of-water-bodies) from Kaggle.
* **Performance**: Achieved **71.38% pixel accuracy** on the training set.

## 🛠️ Technical Stack
* **Language**: Python.
* **Framework**: PyTorch (Deep Learning Engine).
* **Hardware**: NVIDIA T4 GPU (Google Colab).
* **Library**: OpenCV (for image preprocessing).

## 🧠 Workflow
1. **Data Ingestion**: Connected Kaggle API to Google Colab using secure environment variables.
2. **Preprocessing**: Resized satellite imagery to 128x128 and normalized pixel values.
3. **Training**: Optimized a Mini U-Net over 10 epochs, reducing **Average Loss** from **0.5287 to 0.3811**.
4. **Inference**: Generated binary masks where white pixels represent water and black pixels represent land.



## 📊 Results & Insights
* The model successfully identifies large water bodies and coarse geographical features.
* Transitioned from traditional NDWI and Otsu's thresholding methods to an automated Neural Network approach.

