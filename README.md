📂 Models Overview


1️⃣ Galaxy Classifier
Purpose: Classifies galaxy images into different categories.
Approach: Uses a Convolutional Neural Network (CNN) trained on labeled galaxy images.
Key Features:
Image pre-processing (resizing, normalization).
CNN layers for feature extraction.
Softmax activation for classification.




2️⃣ AndreShift
Purpose: Predicts whether a galaxy is approaching or receding relative to the Andromeda galaxy.
Approach: Regression model using distance (kpc) and radial velocity (km/sec) as input features.
Key Features:
Uses a simple feed-forward neural network (FFNN).
Trained using Mean Squared Error (MSE) loss.
Evaluates prediction accuracy with RMSE.




3️⃣ ExoHabit
Purpose: Determines the habitability of an exoplanet based on its atmospheric conditions.
Approach: Classification model trained with labeled exoplanet data.
Key Features:
Inputs: CO2, O2, N2, H2O percentage, atmospheric pressure, albedo, temperature (K), and greenhouse effect.
Uses Random Forest / Neural Network for classification.
Outputs: "Habitable" or "Non-Habitable."




4️⃣ Orbita Analyzer
Purpose: Predicts the optimal orbit for a satellite based on its intended use.
Approach: Uses a decision tree model trained on historical satellite deployment data.
Key Features:
Input parameters include mission type, altitude, and debris risk.
Model selects the safest and most efficient orbit.
Trained using a combination of supervised learning techniques.
# 🌍 Orbital Path Predictor using BERT 🚀  

This project predicts the best orbit for a satellite based on its functionality while minimizing collision risks with active satellites and space debris.  

---

## 📜 **Model Overview**  
- **Architecture**: Fine-tuned **BERT** model for text classification.  
- **Input**: Satellite functionality in natural language.  
- **Processing**:  
  1. Converts text input into tokenized embeddings using **BERT tokenizer**.  
  2. Fine-tuned **BERTForSequenceClassification** maps input to an orbit type.  
  3. The model also considers space debris data to suggest alternative orbits if congestion is high.  
- **Output**:  
  - **Primary orbit suggestion** (e.g., LEO, MEO, GEO, HEO).  
  - **Warning if the orbit is congested**.  
  - **Suggested alternative orbit** with an estimated altitude.  

---

## 🏋️‍♂️ **Training Details**  
- **Dataset**: Labeled dataset with satellite functionalities mapped to orbit types.  
- **Pretrained Model**: `bert-base-uncased` fine-tuned with classification layers.  
- **Loss Function**: Cross-entropy loss.  
- **Optimizer**: AdamW.  
- **Metrics**: Accuracy, F1-score.  

---

## 🚀 **Inference**  
- Given an input text (e.g., `"Earth observation and climate monitoring"`), the model predicts:  

