# Activity Recognition using Deep Learning and Explainable AI

## Overview

This project focuses on video-based **human activity recognition** using deep learning models, with a strong emphasis on **explainability** through Explainable AI (XAI) techniques. It includes dataset preparation, implementation of advanced neural network architectures, and comparative evaluation of XAI methods to ensure model transparency and trust.

---

## 1. Dataset Preparation and Preprocessing

- Video frames were extracted and resized to maintain consistent input dimensions.
- The dataset was split into **training**, **validation**, and **test** sets to support robust and unbiased evaluation.

---

## 2. Deep Learning Models

Three models were implemented for recognizing activities from video data:

- **LRCN (Long-term Recurrent Convolutional Network)**  
  Combines CNNs for spatial feature extraction and RNNs for capturing temporal patterns.

- **3D CNN (3D Convolutional Neural Network)**  
  Uses 3D convolutions to simultaneously model spatial and temporal information.

- **ConvLSTM (Convolutional Long Short-Term Memory)**  
  Integrates convolutional operations within LSTM units for spatiotemporal processing in a unified manner.

✅ **ConvLSTM** achieved the highest accuracy and was selected for further analysis.

---

## 3. Explainable AI (XAI) Techniques

To interpret the ConvLSTM model’s predictions and enhance transparency, the following XAI methods were applied:

- **Grad-CAM (Gradient-weighted Class Activation Mapping)**  
  Produces heatmaps highlighting influential regions in the input frames.

- **SHAP (SHapley Additive exPlanations)**  
  Offers detailed insights into feature importance across frames.

- **LRP (Layer-wise Relevance Propagation)**  
  Tracks the contribution of features throughout the model layers to the final prediction.

---

## 4. Performance Evaluation of XAI Methods

Each XAI method was evaluated using the following metrics:

- **Interpretability**: Clarity and intuitiveness of the explanation for human users.
- **Ambiguity**: Degree of uncertainty or confusion introduced by the explanation.
- **Fidelity**: How accurately the explanation reflects the model’s internal decision-making process.

---

## 5. Comparison of XAI Methods

- Evaluation scores and visualizations were used to determine the **most effective XAI technique**.
- This ensured that the **ConvLSTM** model is not only accurate but also **transparent and explainable**, boosting user confidence in its predictions.

---


## Conclusion

This project demonstrates that combining deep learning with explainable AI can significantly enhance both **performance** and **trustworthiness** in activity recognition systems. The ConvLSTM model, supported by robust XAI tools, serves as an effective and interpretable solution.

