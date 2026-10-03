# # Racing Lap Time Analysis

## Project Overview

This project focuses on analyzing racing lap time data and predicting lap times using machine learning regression algorithms.

The project includes data exploration, visualization, model training, and performance evaluation.

Three regression models are implemented and compared:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

## Objectives

- Explore and understand racing lap time data.
- Analyze relationships between racing conditions and lap times.
- Train machine learning regression models.
- Evaluate model performance using R², MAE, and RMSE.
- Compare the performance of different regression algorithms.

## Dataset

The dataset contains 2,000 records and 6 numerical columns.

### Features

| Feature | Description |
|---|---|
| avg_speed_kmh | Average speed during the lap (km/h) |
| tyre_wear_pct | Tire wear percentage |
| track_temp_c | Track temperature (°C) |
| wind_speed_mps | Wind speed (m/s) |
| pit_stop_flag | Indicates whether a pit stop occurred |
| lap_time_sec | Lap time in seconds (Target Variable) |

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

### 1. Data Loading and Inspection

- Loading the dataset using Pandas
- Inspecting the dataset structure
- Checking data types
- Reviewing descriptive statistics
- Checking missing values

### 2. Exploratory Data Analysis (EDA)

The following visualizations are used:

- Correlation heatmap
- Scatter plot
- Box plot
- Histograms

These visualizations help explore relationships between the features and lap time.

### 3. Data Preparation

The target variable is:

`lap_time_sec`

The remaining columns are used as input features.

The dataset is divided into training and testing sets using an 80/20 split.

### 4. Model Training

The following regression algorithms are trained:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

### 5. Model Evaluation

Model performance is evaluated using:

- **R² Score:** Measures how much of the target variable's variance is explained by the model.
- **MAE (Mean Absolute Error):** Measures the average absolute prediction error.
- **RMSE (Root Mean Squared Error):** Measures prediction error while giving greater weight to larger errors.

## Model Comparison

| Model | R² | MAE | RMSE |
|---|---:|---:|---:|
| Linear Regression | 0.9653 | 0.9671 | 1.1926 |
| Decision Tree | 0.9160 | 1.4905 | 1.8552 |
| Random Forest | 0.9602 | 1.0271 | 1.2772 |

### Results

In the current train-test split, Linear Regression achieved the highest R² score and the lowest MAE and RMSE among the three evaluated models.

These results represent performance on the selected test set.

## Project Structure

```text
racing-lap-time-analysis/
│
├── racing_lap_time_analysis.ipynb
├── racing_lap_times_numeric.csv
├── requirements.txt
├── .gitignore
└── README.md
```

## Installation and Usage

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
```

### 2. Navigate to the project directory

```bash
cd racing-lap-time-analysis
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the notebook

Open `racing_lap_time_analysis.ipynb` using Jupyter Notebook or Visual Studio Code and run the cells.

## Conclusion

This project demonstrates a basic end-to-end machine learning regression workflow, including data exploration, visualization, model training, and evaluation.

Comparing different regression algorithms provides insight into their predictive performance on the racing lap time dataset.

## Author

Machine Learning Practice Project

