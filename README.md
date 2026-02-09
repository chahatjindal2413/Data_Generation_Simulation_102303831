# Data Generation using Modelling and Simulation for Machine Learning

## Project Overview
This project focuses on generating synthetic data using a simulation-based approach and applying machine learning models to analyze the generated data. A physics-based 2D projectile motion simulator is used to generate data, which is then utilized for a regression task.

The objective is to demonstrate how modelling and simulation can be effectively used to create datasets for machine learning when real-world data is limited or unavailable.

---

## Simulation Tool and Domain
- **Simulation Domain:** 2D Physics Simulation
- **Model Used:** Projectile Motion
- **Implementation:** Python-based analytical simulation
- **Platform:** Google Colab

---

## Simulation Model Description
The projectile motion model is based on classical mechanics.  
The horizontal range of a projectile is calculated using the formula:



---

## Parameters and Bounds
The simulation model uses three input parameters and one output parameter.
All input parameters are sampled randomly within predefined bounds to ensure variability and realism in the generated data.
<img width="1008" height="365" alt="image" src="https://github.com/user-attachments/assets/36d68a95-ba06-46d8-a1c1-da6b3330f42a" />

---

## Data Generation Methodology
1. Random values of velocity, angle, and gravity were generated within predefined bounds.
2. These parameters were passed to the projectile motion simulator.
3. The simulator computed the horizontal range for each instance.
4. A total of **1000 simulations** were generated.
5. The dataset was stored in tabular format and used for machine learning.

---

## Sample Generated Data

<img width="1022" height="365" alt="image" src="https://github.com/user-attachments/assets/8fed96a4-5851-4a86-a391-eee369d8abd9" />


---

## Machine Learning Models Used
The following regression models were trained and evaluated:

1. Linear Regression  
2. Decision Tree Regressor  
3. Random Forest Regressor  
4. K-Nearest Neighbors (KNN)  
5. Support Vector Regressor (SVR)  
6. Gradient Boosting Regressor  

---

## Evaluation Metrics
The performance of each model was evaluated using:
- Mean Squared Error (MSE)
- R² Score

---

## Model Comparison Results

<img width="448" height="300" alt="image" src="https://github.com/user-attachments/assets/1b9f25b5-6ad7-4f5b-a9c9-ae5b87861004" />
<img width="1154" height="667" alt="image" src="https://github.com/user-attachments/assets/23bd4d2a-4acf-497e-824a-21ad0fd68a86" />
<img width="1292" height="685" alt="image" src="https://github.com/user-attachments/assets/eecc8a70-ec4b-4fc0-bcf7-dd3e23bfa643" />



---

## Best Model Selection
- **Best Model:** Random Forest Regressor
- **Selection Criteria:** Highest R² score and lowest Mean Squared Error

---

## Visualizations
The following visualizations are included in the notebook:
- R² score comparison of all models
- Mean Squared Error comparison
- Actual vs Predicted plot for the best-performing model

---

## Final Confirmation
- 1000 simulations generated successfully
- 6 machine learning models trained and evaluated
- Best model selected using quantitative metrics
- High prediction accuracy achieved (R² ≈ 0.99+)

---

## How to Run
1. Open the Google Colab notebook.
2. Run the single combined code cell.
3. All outputs, tables, and graphs will be generated automatically.

---

## Conclusion
This project demonstrates that simulation-based data generation is a powerful approach for machine learning tasks. Ensemble models such as Random Forest and Gradient Boosting perform exceptionally well on structured, physics-based simulation data.
