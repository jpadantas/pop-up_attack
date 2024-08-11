# Autonomous Pop-Up Attack Maneuvers Using Imitation Learning

This project implements an imitation learning model using Long Short-Term Memory (LSTM) networks to predict aircraft control inputs during complex maneuvers, specifically focusing on pop-up attack maneuvers. The project is structured to include data preprocessing, model training, evaluation, and visualization of the results.

## Project Structure

- `eda.ipynb`: Exploratory Data Analysis notebook. This notebook is used for initial data exploration, visualization, and understanding the characteristics of the flight data.
  
- `imitation-learning.ipynb`: Main notebook for developing the imitation learning model. This includes data preprocessing, model architecture definition, training, evaluation, and plotting the results.

- `flights/`: Directory containing the original flight data files. Each file represents a set of state-action pairs collected from flight simulations.

- `adjusted_flights/`: Directory containing preprocessed flight data files. The data in these files has been cleaned and adjusted for input into the LSTM model.

- `metrics/`: Directory where cross-validation metrics and overall model performance metrics are stored as CSV files. These metrics include mean squared error (MSE), root mean squared error (RMSE), mean absolute error (MAE), and R² scores, among others.

- `models/`: Directory where trained models are saved. The models are saved in `.keras` format, with different models saved for each fold of cross-validation.

- `plots/`: Directory containing generated plots, including comparisons between actual and predicted trajectories, as well as training and validation loss curves.

## How to Run the Project

1. **Exploratory Data Analysis:**
   - Open `eda.ipynb`.
   - Run all cells to visualize and understand the flight data.
   - This step is important to grasp the distribution and characteristics of the data before feeding it into the model.

2. **Imitation Learning Model:**
   - Open `imitation-learning.ipynb`.
   - Run all cells to preprocess the data, train the LSTM model, and evaluate its performance.
   - The notebook also generates plots comparing the predicted actions with the actual actions.

3. **Evaluate Results:**
   - The `metrics/` directory will contain CSV files with the evaluation results of the model.
   - The `plots/` directory will contain visual comparisons of actual versus predicted actions, as well as training metrics.

## Requirements

The project requires the following Python packages:

- `tensorflow`
- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`

Make sure to install these packages using pip:

```bash
pip install tensorflow numpy pandas scikit-learn matplotlib
