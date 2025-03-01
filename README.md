# SPACE-SAGE
SPACE SAGE is an advanced AI/ML-powered space exploration project designed to analyze celestial objects using cutting-edge machine learning models. It integrates multiple AI-driven models to provide valuable insights into various astrophysical phenomena.


Andromeda Motion Prediction Using Doppler Shift 🚀
This project predicts whether a galaxy is approaching or receding from Andromeda using Radial Velocity (km/s) and Distance (kpc). It applies Machine Learning (Random Forest Classifier) to analyze motion based on redshift and blueshift data.

📌 Features
✅ Calculates Redshift (z) and Radial Velocity (km/s) using observed and rest wavelengths.
✅ Classifies galaxies as Approaching (Blueshifted) or Receding (Redshifted).
✅ Trains a Random Forest Model for motion prediction.
✅ Uses astroquery to fetch real astronomical data from NED, SDSS, and Gaia.
✅ Generates visualizations for redshift distribution and velocity-distance relationships.

📂 Dataset
The dataset includes the following columns:
🔹 Observed Wavelength (nm) - Light wavelength observed from Earth.
🔹 Rest Wavelength (nm) - Actual wavelength of emitted light.
🔹 Distance from Andromeda (kpc) - Distance of the galaxy in kiloparsecs.
🔹 Radial Velocity (km/s) - Speed of the galaxy relative to Andromeda.
🔹 Motion Direction - "Approaching" or "Receding" classification.

📊 Scientific Background
1️⃣ Redshift & Blueshift
When an object moves toward us, its light shifts to shorter wavelengths (Blueshift).
When an object moves away from us, its light shifts to longer wavelengths (Redshift).
2️⃣ Radial Velocity Calculation
Using Doppler Effect:  v=ZxC

c = speed of light (299,792 km/s).

🧠 How Random Forest Works in This Model
The Random Forest Classifier is trained using known distances and velocities to classify galaxies.
Instead of setting fixed rules, the model learns decision boundaries from real data.
Example Decision Process:

If Distance < 200 kpc and Velocity < -100 km/s → Approaching
If Distance > 400 kpc and Velocity > 50 km/s → Receding
The trained model generalizes this process using multiple decision trees to improve accuracy.
