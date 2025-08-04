# 🏠 Real Estate Price Prediction - Bangalore

A complete end-to-end machine learning project to predict real estate prices in Bangalore using Linear Regression. The project includes data preprocessing, model training, and a user-friendly web interface built with HTML, CSS, JavaScript, and Flask.

---

## 🔍 About the Project

This project aims to:
- Clean and analyze real estate data
- Build a price prediction model
- Deploy the model using a Flask backend
- Create a simple frontend interface for users to input property details and get price predictions

---

## ⚙️ Technologies Used

- **Languages**: Python, HTML, CSS, JavaScript
- **Libraries**: Pandas, NumPy, scikit-learn, Flask
- **Tools**: Jupyter Notebook, Pickle
- **Frontend**: Vanilla JS, HTML5, CSS3

---

## 📊 Dataset

- `bhp.csv` – Housing data containing:
  - Location
  - Size (BHK)
  - Total square feet
  - Bathrooms
  - Price (target)

---

## 🤖 Model

- **Algorithm**: Linear Regression
- **Preprocessing**:
  - One-hot encoding for locations
  - Outlier removal based on domain knowledge
  - Feature selection for model input

The model is saved as `banglore_home_prices_model.pkl` and uses `columns.json` for feature reference during predictions.

---

## 🌐 Web Application

- Frontend (`app.html`, `app.css`, `app.js`) handles user input
- Backend (`server.py`, `util.py`) processes requests and returns predictions
- Dropdowns are dynamically loaded using JavaScript and Flask

---

## 📸 Snapshots

### 🏠 Homepage
![Snapshot 1](./Client/Snapshot%201.png)

### 🔧 Input Form
![Snapshot 2](./Client/Snapshot%202.png)

### 📈 Prediction Result
![Snapshot 3](./Client/Snapshot%203.png)

---

## 🚀 How to Run the Project

1. **Clone the Repository**
```bash
git clone https://github.com/yourusername/real-estate-price-prediction.git
cd real-estate-price-prediction
