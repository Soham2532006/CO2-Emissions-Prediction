# CO2-Emissions-Prediction
🧩 Problem Statement
To develop machine learning models that accurately predict the CO₂ emissions (g/km) of vehicles based on their engine size, fuel consumption, and other technical specifications. The aim is to support environmental analysis and guide automotive decision-making for manufacturers and policy-makers.

📊 Dataset Overview
Source: Government of Canada – Vehicle Fuel Consumption Ratings.

Size: ~1000+ vehicle entries.

Features:

Categorical: Make, Model, Vehicle Class, Transmission, Fuel Type

Numerical: Engine Size (L), Cylinders, Fuel Consumption (City/Hwy/Combined), Fuel Consumption (mpg)

Target Variable: CO2 Emissions (g/km)

Goal: Predict CO₂ emissions using vehicle attributes.

🧭 Approach
Data Preprocessing:

Loaded CSV data with pandas.

Removed null values (if any).

Encoded categorical columns using Label Encoding.

Split dataset into features (X) and target (CO2 Emissions(g/km)).

Scaled features using StandardScaler.

Models Implemented:

Linear Regression: Simple baseline for continuous output.

Decision Tree Regressor: Captures feature-based splits.

Random Forest Regressor: Ensemble model for better generalization.

Polynomial Regression (degree=2): Models nonlinear relationships.

Neural Network (Keras):

2 hidden layers (64 and 32 neurons, ReLU)

Output layer: 1 neuron (linear activation)

Trained for 50 epochs, batch size 32

Evaluation Metrics:

Used R² Score for regressors.

Used MAE (Mean Absolute Error) and MSE (Mean Squared Error) for neural network evaluation.

🧾 Conclusion
The machine learning models demonstrated good ability to predict CO₂ emissions based on vehicle specifications. Among all, ensemble methods like Random Forest and the Neural Network achieved the highest accuracy, suggesting that nonlinear models perform better on this dataset. The project proves that ML can support environmental efforts by predicting emissions early in vehicle design and regulation processes.
