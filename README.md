# ml-lifecycle-webapp

## Project Overview
This project is a Machine Learning web application developed using Flask. It uses a trained Ridge Regression model and a StandardScaler to generate predictions based on user-provided input features.

The application provides a web interface where users can enter input values and view the prediction result.

## Technologies Used
- Python
- Flask
- NumPy
- Pandas
- Scikit-learn
- HTML and CSS
- Pickle for loading the trained machine learning model

## Input Features
The application accepts the following nine input features:

1. Temperature
2. Relative Humidity (RH)
3. Wind Speed (Ws)
4. Rainfall (Rain)
5. Fine Fuel Moisture Code (FFMC)
6. Duff Moisture Code (DMC)
7. Initial Spread Index (ISI)
8. Classes
9. Region

## Project Structure

```text
ml-lifecycle-webapp/
│
├── application.py
├── README.md
├── models/
│   ├── ridge.pkl
│   └── scaler.pkl
│
└── templates/
    ├── index.html
    └── home.html
```

## Installation and Setup

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd ml-lifecycle-webapp
```

### 2. Install Dependencies

```bash
pip install flask numpy pandas scikit-learn
```

### 3. Run the Application

```bash
python application.py
```

### 4. Open the Web Application

Open your browser and visit:

http://127.0.0.1:5000/

## How It Works

1. The user opens the web application.
2. The user enters the required input values.
3. Flask receives the submitted data.
4. The StandardScaler transforms the input features.
5. The Ridge Regression model generates a prediction.
6. The application displays the prediction result on the web page.

## Machine Learning Model

The application uses a trained Ridge Regression model for prediction. The model and scaler are loaded from saved pickle files located in the `models` directory.

## Requirements

- Python 3.x
- Required Python libraries
- Trained model file: `models/ridge.pkl`
- Scaler file: `models/scaler.pkl`
- HTML templates: `templates/index.html` and `templates/home.html`

## Author

Developed as a machine learning web application project.
