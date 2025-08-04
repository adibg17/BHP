# Real Estate Price Prediction

## Project Overview

Developed an end-to-end machine learning system to predict residential property prices in Bangalore based on user inputs like location, square footage, BHK, and number of bathrooms. The project involved data cleaning, exploratory analysis, feature engineering, and training a linear regression model using scikit-learn. The trained model was deployed using a Flask backend and integrated with a responsive frontend built with HTML, CSS, and JavaScript.

## Features

- **Real-time Price Prediction**: Users can interact with the model through a browser-based interface and receive instant price predictions
- **User-friendly Interface**: Responsive web design built with HTML, CSS, and JavaScript
- **Machine Learning Pipeline**: Complete data preprocessing, feature engineering, and model training workflow
- **RESTful API**: Flask backend serving the trained model
- **Modular Design**: Built with scalability and future deployment in mind

## Technology Stack

- **Backend**: Python, Flask, scikit-learn
- **Frontend**: HTML, CSS, JavaScript
- **Machine Learning**: Linear Regression, Data preprocessing, Feature engineering
- **Data Processing**: Pandas, NumPy

## Project Structure

```
BHP2/
├── Client/
│   ├── Snapshot1.png
│   ├── Snapshot2.png
│   ├── Snapshot3.png
│   ├── app.css
│   ├── app.html
│   └── app.js
├── Model/
│   ├── banglore_home_prices_model.pickle
│   ├── bhp.csv
│   ├── columns.json
│   └── training_model.ipynb
├── Server/
│   ├── __pycache__/
│   ├── artifacts/
│   ├── server.py
│   └── util.py
```

## Dataset

The project uses Bangalore house price data (`bhp.csv`) containing information about:
- Location
- Size (BHK)
- Total square footage
- Number of bathrooms
- Price

## Model Development

1. **Data Cleaning**: Handled missing values, outliers, and inconsistent data formats
2. **Exploratory Data Analysis**: Analyzed price distributions, location trends, and feature correlations
3. **Feature Engineering**: Created meaningful features and encoded categorical variables
4. **Model Training**: Implemented Linear Regression using scikit-learn
5. **Model Evaluation**: Validated performance using appropriate metrics

## Installation & Setup

### Prerequisites
- Python 3.x
- pip package manager

### Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd BHP2
   ```

2. **Install required packages**
   ```bash
   pip install flask scikit-learn pandas numpy
   ```

3. **Start the Flask server**
   ```bash
   cd Server
   python server.py
   ```

4. **Open the web application**
   - Navigate to the `Client` folder
   - Open `app.html` in your web browser
   - Or serve it through a local web server

## Usage

1. Open the web interface in your browser
2. Select the desired location from the dropdown
3. Enter the square footage area
4. Choose the number of BHK (bedrooms)
5. Select the number of bathrooms
6. Click "Estimate Price" to get the predicted property price

## Screenshots

### User Interface
![Snapshot 1](Client/Snapshot1.png)

### Price Prediction Interface
![Snapshot 2](Client/Snapshot2.png)

### Results Display
![Snapshot 3](Client/Snapshot3.png)

## API Endpoints

- `GET /get_location_names` - Retrieve available locations
- `POST /predict_home_price` - Predict house price based on input parameters

## Model Performance

The Linear Regression model was trained and validated on Bangalore real estate data, providing reliable price predictions based on the input features.

## Future Enhancements

- Deploy to cloud platforms (AWS, Heroku, etc.)
- Add more advanced ML algorithms (Random Forest, XGBoost)
- Implement price trend analysis
- Add more cities and regions
- Include additional features like property age, amenities, etc.
- Mobile-responsive design improvements

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

For questions or suggestions, please feel free to reach out or create an issue in the repository.

---

**Note**: This project was developed for educational and demonstration purposes. The model's predictions should be used as estimates and not as definitive property valuations.
Run the Flask Server
cd Server
python server.py
Open the Frontend
Open Client/app.html in your browser and use the interface to test predictions.
