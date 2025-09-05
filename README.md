# Safe Drinking Water Prediction

A machine learning project that predicts the potability of water based on various chemical and physical properties. The project includes a complete end-to-end pipeline from data preprocessing to deployment as an interactive web application.

🌐 **[Live Web Application](https://safe-drinking-water.streamlit.app/)** *(Replace with your actual URL)*

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Installation](#installation)
- [Usage](#usage)
- [Model Performance](#model-performance)
- [Repository Structure](#repository-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This project addresses a critical public health challenge by developing a machine learning model to classify water samples as safe or unsafe for human consumption. The model analyzes multiple water quality parameters to make predictions, helping ensure access to safe drinking water.

## ✨ Features

- **Interactive Web Interface**: User-friendly Streamlit application for real-time predictions
- **Robust ML Pipeline**: Complete workflow from data preprocessing to model deployment
- **Class Imbalance Handling**: SMOTE technique for balanced model training
- **Model Interpretability**: Feature importance analysis to understand key water quality factors
- **Optimized Performance**: Hyperparameter tuning using GridSearchCV

## 📊 Dataset

The model uses water quality parameters including:
- pH levels
- Hardness
- Solids content
- Chloramines
- Sulfate
- Conductivity
- Organic carbon
- Trihalomethanes
- Turbidity

## 🔬 Methodology

### 1. Data Preprocessing
- **Missing Value Treatment**: Systematic handling of null values
- **Feature Scaling**: StandardScaler normalization for consistent feature ranges
- **Data Validation**: Quality checks and outlier detection

### 2. Class Imbalance Resolution
- **SMOTE Implementation**: Synthetic Minority Over-sampling Technique
- **Balanced Dataset**: Equal representation of "Potable" and "Not Potable" classes

### 3. Model Development
- **Algorithm**: Random Forest Classifier
- **Hyperparameter Optimization**: GridSearchCV for optimal performance
- **Cross-Validation**: Robust model evaluation techniques

### 4. Model Interpretation
- **Feature Importance Analysis**: Identification of critical water quality parameters
- **Performance Metrics**: Comprehensive evaluation using accuracy, precision, recall, and F1-score

## 🚀 Installation

### Prerequisites
- Python 3.10 or higher
- pip package manager

### Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/krnike96/safe-drinking-water.git
   cd safe-drinking-water-prediction
   ```

2. **Create Virtual Environment (Recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 💻 Usage

### Running the Web Application

```bash
streamlit run app.py
```

The application will open in your browser at `http://localhost:8501`

### Making Predictions

1. Open the web application
2. Input water quality parameters in the sidebar
3. Click "Predict Water Potability"
4. View the prediction result and confidence score

## 📈 Model Performance

| Metric | Score |
|--------|--------|
| Accuracy | XX.X% |
| Precision | XX.X% |
| Recall | XX.X% |
| F1-Score | XX.X% |

*(Update with your actual model performance metrics)*

## 📁 Repository Structure

```
safe-drinking-water-prediction/
│
├── Safe_Drinking_Water_Prediction.ipynb    # Main analysis notebook
├── app.py                                  # Streamlit web application
├── best_rf_model.pkl                      # Trained Random Forest model
├── scaler.pkl                             # Fitted StandardScaler
├── requirements.txt                       # Python dependencies
├── README.md                              # Project documentation
```

## 🛠️ Technologies Used

- **Python 3.x**: Core programming language
- **Scikit-learn**: Machine learning library
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Streamlit**: Web application framework
- **Matplotlib/Seaborn**: Data visualization
- **Imbalanced-learn**: SMOTE implementation
- **Pickle**: Model serialization

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



## 🙏 Acknowledgments

- Water quality dataset providers
- Open-source community for excellent libraries
- Contributors and maintainers

---

⭐ If you found this project helpful, please give it a star!
