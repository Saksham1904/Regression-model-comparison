# Regression-model-comparison
# Model Performance Comparison

This repository contains a Python script to evaluate the performance of various regression models using a sample dataset. The goal is to identify the model that provides the best R² score for the given data.

## Overview

The script compares the performance of multiple regression models on a dataset, with the target variable set to `Target4`. The models evaluated include:

- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- Lasso Regression
- Ridge Regression
- K-Nearest Neighbors (KNN)
- Decision Tree Regressor
- Support Vector Regressor (SVR)

The R² score is used as the performance metric, with higher values indicating better model performance.

## Results

The performance of the models is summarized below:

```markdown
| Model                      | R² Score  |
|----------------------------|------------|
| Linear Regression          | -0.0170    |
| Random Forest              | -0.0540    |
| Gradient Boosting          | -0.1198    |
| Lasso Regression           | -0.0245    |
| Ridge Regression           | **-0.0163** (Best) |
| K-Nearest Neighbors (KNN)  | -0.2175    |
| Decision Tree              | **-1.3609** (Worst) |
| Support Vector Regressor (SVR) | -0.0249 |
```

### Best Model
- **Ridge Regression** with an R² score of **-0.0163**

### Worst Model
- **Decision Tree Regressor** with an R² score of **-1.3609**

## Features
- Evaluate multiple regression models.
- Automatically identifies the best and worst performing models based on R² scores.
- Visualizes model performance using a bar chart.

## Prerequisites

- Python 3.7+
- Required libraries:
  - pandas
  - matplotlib
  - scikit-learn

Install the dependencies using pip:
```bash
pip install pandas matplotlib scikit-learn
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/model-performance-comparison.git
   ```
2. Navigate to the project directory:
   ```bash
   cd model-performance-comparison
   ```
3. Replace the placeholder dataset path (`Fuel_cell_performance_data-Full.csv`) with your dataset file path.
4. Run the script:
   ```bash
   python script_name.py
   ```
5. View the results in the console and the generated bar chart for model comparison.

## Output

The script outputs:
- A numerical comparison of R² scores for all models.
- Identification of the best and worst performing models.
- A bar chart visualizing the R² scores of all models.

## Notes

- The sample dataset used for this analysis is not included in the repository. Replace the file path with your dataset.
- Negative R² scores indicate that the model performs worse than a simple mean prediction.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for any improvements or suggestions.

