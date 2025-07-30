# 🔮 EV Vehicle-Charging Demand Prediction

> **A Machine Learning-powered Streamlit application for forecasting Electric Vehicle adoption trends in Washington State counties**

![EV Forecasting Demo](ev-car-factory.jpg)

## 🚗 Project Overview

As electric vehicle (EV) adoption surges, urban planners and policymakers need to anticipate infrastructure needs—especially charging stations. Inadequate planning can lead to bottlenecks, impacting user satisfaction and hindering sustainability goals.

This project leverages machine learning to forecast EV adoption trends, helping stakeholders make data-driven decisions for sustainable transportation infrastructure.

## 🎯 Problem Statement

Using electric vehicle dataset from Washington State Department of Licensing, create a predictive model to forecast future EV adoption patterns. The model predicts the number of electric vehicles in upcoming years based on historical trends, vehicle types, and regional data.

## 🎥 Live Demo

*[Add your website recording/demo video here]*

## ✨ Features

### 🔍 **Interactive Forecasting Dashboard**
- **County-wise Analysis**: Select any Washington State county for detailed EV adoption forecasting
- **3-Year Predictions**: Comprehensive forecasting with 36-month horizon
- **Real-time Visualizations**: Interactive charts showing historical vs predicted trends

### 📊 **Advanced Analytics**
- **Cumulative Growth Tracking**: Monitor total EV adoption over time
- **Percentage Growth Analysis**: Calculate and display growth rates
- **Multi-County Comparison**: Compare up to 3 counties simultaneously

### 🎨 **Professional UI/UX**
- **Responsive Design**: Works seamlessly across different screen sizes
- **Modern Styling**: Professional gradient backgrounds and color schemes
- **Interactive Components**: Dropdown selectors and multi-select options

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **Machine Learning**: Scikit-learn (Random Forest Regressor)
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib
- **Model Persistence**: Joblib

## 📁 Project Structure

```
EV-Adoption-Forecast/
├── app.py                              # Main Streamlit application
├── EV_Adoption_Forecasting.ipynb       # Jupyter notebook for model development
├── forecasting_ev_model.pkl            # Trained ML model
├── preprocessed_ev_data.csv            # Cleaned and processed dataset
├── ev-car-factory.jpg                  # Application header image
├── EV Vehicle-Charging Demand Prediction-dataset.csv  # Original dataset
└── README.md                           # Project documentation
```

## 🚀 Quick Start

### Prerequisites
```bash
Python 3.7+
pip install streamlit pandas numpy scikit-learn matplotlib joblib
```

### Installation & Usage
1. **Clone the repository**
   ```bash
   git clone https://github.com/vedaanth-arch/EV-Adoption-Forecast.git
   cd EV-Adoption-Forecast
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   streamlit run app.py
   ```

4. **Open your browser** and navigate to `http://localhost:8501`

## 📊 Dataset Information

**Source**: Washington State Department of Licensing (DOL)  
**Time Period**: January 2017 - February 2024  
**Geographic Coverage**: All Washington State counties

### Key Features:
- **Date**: Monthly vehicle registration counts (end of month)
- **County**: Geographic regions within Washington State
- **Vehicle Types**: Passenger vehicles (83%) and Trucks (17%)
- **EV Categories**:
  - **BEVs**: Battery Electric Vehicles (fully electric)
  - **PHEVs**: Plug-in Hybrid Electric Vehicles
- **Total Metrics**: EV totals, non-electric totals, percentage calculations

**Dataset Link**: [Kaggle - Electric Vehicle Population Size 2024](https://www.kaggle.com/datasets/sahirmaharajj/electric-vehicle-population-size-2024/data)

## 🧠 Machine Learning Model

### Model Architecture
- **Algorithm**: Random Forest Regressor
- **Features**: Lagged variables, rolling averages, percentage changes, growth slopes
- **Target**: Monthly EV adoption counts
- **Validation**: Time-series cross-validation

### Feature Engineering
- **Lag Features**: Previous 1, 2, and 3 month values
- **Rolling Statistics**: 3-month moving averages
- **Growth Metrics**: Percentage changes and trend slopes
- **Encoded Categories**: County encoding for regional patterns

## 🎯 Model Performance

The model demonstrates strong predictive capability with:
- Robust handling of seasonal patterns
- Accurate trend forecasting
- County-specific adaptation
- 3-year forecasting horizon

## 📈 Key Insights

1. **Regional Variations**: Different counties show distinct EV adoption patterns
2. **Growth Trends**: Consistent upward trajectory across most counties
3. **Seasonal Effects**: Monthly variations in registration patterns
4. **Infrastructure Planning**: Predictive insights for charging station deployment

## 🎨 Application Screenshots

*[Add screenshots of your application here]*

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Vedaanth**
- GitHub: [@vedaanth-arch](https://github.com/vedaanth-arch)
- Project Link: [EV-Adoption-Forecast](https://github.com/vedaanth-arch/EV-Adoption-Forecast)

## 🙏 Acknowledgments

- **AICTE Internship Cycle 2 by S4F** for project guidance
- **Washington State DOL** for providing comprehensive EV registration data
- **Kaggle Community** for data hosting and accessibility
- **Streamlit Team** for the amazing web app framework

---

*Prepared for the **AICTE Internship Cycle 2 by S4F***
