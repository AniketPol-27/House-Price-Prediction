# House-Price-Prediction
Predict house prices in King County, USA using a **Gradient Boosting Regressor**. This project includes feature engineering, visualization, and model evaluation to build a reliable predictive model.

---

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Libraries Used](#libraries-used)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Modeling](#modeling)
- [Results](#results)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [License](#license)

---

## Overview
This project predicts King County house prices by analyzing key features like square footage, bedrooms, bathrooms, house age, renovation status, and location bins. The model demonstrates strong predictive accuracy using Gradient Boosting Regressor.

---

## Dataset
- Source: [King County House Sales Dataset](https://www.kaggle.com/harlfoxem/housesalesprediction)
- Contains 21 features including `price`, `bedrooms`, `bathrooms`, `sqft_living`, `floors`, `waterfront`, `grade`, `zipcode`, and location coordinates (`lat`, `long`).

---

## Libraries Used
- `pandas`, `numpy` – Data manipulation
- `matplotlib`, `seaborn` – Data visualization
- `scikit-learn` – Machine learning models, train-test split, cross-validation

---

## Exploratory Data Analysis (EDA)
- Price distribution histogram
- Scatter plots: price vs living area, price vs bedrooms, price vs location
- Outlier handling: removed extreme house prices, bedrooms, bathrooms, and living area
- Feature engineering:
  - `house_age` – Age of the house
  - `renovated` – Binary renovation status
  - `lat_bin` & `long_bin` – Location bins

---

## Modeling
- **Algorithm**: Gradient Boosting Regressor
- **Hyperparameters**:
  - `n_estimators = 600`
  - `max_depth = 6`
  - `learning_rate = 0.05`
  - `loss = 'squared_error'`
- **Train-test split**: 90% training, 10% testing
- **Cross-validation**: 5-fold CV

---

## Results
- **R² Score**: `0.9041`  
- **Mean CV R²**: `0.8945`  

- Feature importance analysis highlights the most influential factors affecting house prices.
- Visualizations show key trends in the dataset.

---

## Conclusion
- Gradient Boosting Regressor effectively predicts King County house prices.
- Feature engineering and outlier handling improved model performance and reliability.
- Location, house age, and renovation status are significant predictors.

---

## Future Work
- Explore additional features like price per square foot, proximity to amenities, and school ratings.
- Experiment with other models (XGBoost, LightGBM) for potential performance improvement.
- Deploy as a web app for interactive house price predictions.

---

## License
This project is licensed under the MIT License.


