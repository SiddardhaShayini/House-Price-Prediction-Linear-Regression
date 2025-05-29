---
# House Price Prediction using Linear Regression

This project demonstrates the application of **Simple and Multiple Linear Regression** to predict house prices using a publicly available dataset. It covers data preprocessing, model training, evaluation, and interpretation of results.

---
## Dataset

The dataset used for this project is `Housing.csv`.
It includes the following features:
* `price`: The price of the house.
* `area`: The total area of the house in square feet.
* `bedrooms`: Number of bedrooms.
* `bathrooms`: Number of bathrooms.
* `stories`: Number of stories.
* `mainroad`: Connectivity to main road (Yes/No).
* `guestroom`: Presence of a guest room (Yes/No).
* `basement`: Presence of a basement (Yes/No).
* `hotwaterheating`: Hot water heating system (Yes/No).
* `airconditioning`: Air conditioning system (Yes/No).
* `parking`: Number of parking spaces.
* `prefarea`: Located in a preferred area (Yes/No).
* `furnishingstatus`: Furnishing status (Fully Furnished, Semi-Furnished, Unfurnished).

---
## Project Structure

The project follows these key steps:

1.  **Data Import & Preprocessing**:
    * Loading the dataset.
    * Converting categorical features (`Yes/No` to `1/0` and `furnishingstatus` using one-hot encoding).
    * Scaling numerical features (`price`, `area`) using `MinMaxScaler`.
2.  **Data Splitting**:
    * Dividing the dataset into training and testing sets (70% train, 30% test).
3.  **Model Training**:
    * **Simple Linear Regression**: Trained using `area` to predict `price`.
    * **Multiple Linear Regression**: Trained using all relevant features to predict `price`.
4.  **Model Evaluation**:
    * Assessing models using **Mean Absolute Error (MAE)**, **Mean Squared Error (MSE)**, and **R-squared ($R^2$) score**.
5.  **Interpretation & Visualization**:
    * Plotting the simple linear regression line.
    * Interpreting model coefficients.
    * Additional visualizations:
        * Distribution of scaled house prices.
        * Correlation heatmap of features.
        * Residuals plot for multiple linear regression.
        * Feature importance based on absolute coefficients.
        * Actual vs. Predicted prices plot for multiple linear regression.

---
## Results Summary

| Model                       | MAE   | MSE   | R-squared |
| :-------------------------- | :---- | :---- | :-------- |
| **Simple Linear Regression** | 0.120 | 0.024 | 0.258     |
| **Multiple Linear Regression** | 0.080 | 0.011 | 0.646     |

**Key Takeaways:**

* **Simple Linear Regression** (using `area` only) provides a basic understanding, explaining about **26%** of the price variation.
* **Multiple Linear Regression** significantly improves performance, explaining around **65%** of the price variation by incorporating all features. This indicates that multiple factors collectively play a crucial role in determining house prices.

---
## How to Run

1.  **Clone the repository:**
    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  **Run the Python script:**
    ```bash
    python your_script_name.py # Replace 'your_script_name.py' with the actual file name
    ```
---
## ✍️ Author

- Siddardha Shayini

---
