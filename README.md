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
