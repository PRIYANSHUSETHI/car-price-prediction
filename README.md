
# 🚗 Car Price Prediction using Machine Learning

This project uses machine learning to predict the selling price of used cars based on key features such as present price, kilometers driven, fuel type, transmission type, ownership history, and more. The dataset used is clean, compact, and perfect for regression-based modeling.

---

## 📊 Project Highlights

- ✅ Data cleaning and preprocessing
- ✅ Feature engineering (e.g. car age, kms per year, log transform)
- ✅ Multiple ML models: Linear Regression, Lasso, and Random Forest
- ✅ Advanced metrics: R² Score, MAE, RMSE
- ✅ Outlier detection and price fairness analysis
- ✅ Feature importance visualization
- ✅ Custom price prediction simulator
- ✅ Fully executable in one cell

---

## 🧠 Technologies Used

- **Python**
- **Pandas** and **NumPy** for data manipulation
- **Matplotlib** and **Seaborn** for visualizations
- **Scikit-Learn** for machine learning models
- **Random Forest Regressor** for robust price predictions

---

## 🗂️ Dataset Features

| Feature         | Description                                 |
|----------------|---------------------------------------------|
| Car_Name        | Name of the car                             |
| Year            | Manufacturing year                          |
| Selling_Price   | Price the car is being sold for (target)    |
| Present_Price   | Current ex-showroom price                   |
| Kms_Driven      | Total kilometers driven                     |
| Fuel_Type       | Petrol / Diesel / CNG                       |
| Seller_Type     | Dealer / Individual                         |
| Transmission    | Manual / Automatic                          |
| Owner           | Number of previous owners                   |

---

## ⚙️ Feature Engineering

- **Car_Age**: `2025 - Year`
- **Kms_per_Year**: `Kms_Driven / Car_Age`
- **Kms_Driven_log**: Log-transformed kms for better modeling

---

## 📈 Model Evaluation Metrics

- **R² Score**: Measures goodness of fit
- **MAE**: Mean Absolute Error
- **RMSE**: Root Mean Squared Error

---

## 🔍 Results

- 🚀 **R² Score**: ~0.98 (Random Forest)
- 🧾 Model detects overvalued and undervalued listings
- 📊 Importance of features like `Present_Price` and `Car_Age` visualized

---

## 💡 Simulated Price Prediction

You can input a custom car profile into the model to get an instant price prediction:

```python
sim_input = pd.DataFrame([{
    'Present_Price': 7.5,
    'Fuel_Type': 1,
    'Seller_Type': 0,
    'Transmission': 1,
    'Owner': 0,
    'Car_Age': 5,
    'Kms_per_Year': 12000,
    'Kms_Driven_log': np.log1p(60000)
}])
predicted_price = model.predict(sim_input)
```

---

## 🚧 Future Improvements

- [ ] Deploy with **Streamlit** or **Gradio**
- [ ] Integrate SHAP for model explainability
- [ ] Add voice or form input interface
- [ ] Include car brand/model extraction for detailed insights

---

## 📎 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/car-price-prediction.git
   ```
2. Navigate to the project folder:
   ```bash
   cd car-price-prediction
   ```
3. Run the Python file or Jupyter Notebook:
   ```bash
   python car_price_prediction\ USING\ ML.py
   ```

---

## 🙌 Acknowledgements

- Inspired by real-world car marketplaces
- Dataset from public ML resources (e.g., Kaggle)

---

## 📬 Contact

For any inquiries or collaboration opportunities, feel free to connect:
- Email: your.email@example.com
- GitHub: [@yourusername](https://github.com/yourusername)
