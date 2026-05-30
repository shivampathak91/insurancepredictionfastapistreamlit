Here’s a professional `README.md` for your GitHub project:

# Insurance Prediction Web App

Predict insurance charges based on user details using a Machine Learning model deployed with FastAPI and Streamlit.

## Project Overview

This project is an end-to-end Machine Learning application that predicts medical insurance costs based on user inputs such as:

* Age
* Gender
* BMI
* Number of Children
* Smoking Status
* Region

The application uses:

* **Machine Learning** for prediction
* **FastAPI** as the backend API
* **Streamlit** as the frontend interface

## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-Learn
* FastAPI
* Uvicorn
* Streamlit
* Joblib

## Project Structure

```bash
insurancepredictionfastapistreamlit/
│
├── app.py                  # Streamlit frontend
├── main.py                 # FastAPI backend
├── model.pkl               # Trained ML model
├── requirements.txt
├── README.md
│
├── notebooks/
│   └── insurance_model.ipynb
│
└── data/
    └── insurance.csv
```

## Features

* User-friendly Streamlit interface
* Real-time insurance charge prediction
* FastAPI REST API integration
* Machine Learning model deployment
* Easy to customize and extend

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/shivampathak91/insurancepredictionfastapistreamlit.git

cd insurancepredictionfastapistreamlit
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

#### Windows

```bash
venv\Scripts\activate
```

#### Linux/Mac

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## Run FastAPI Backend

```bash
uvicorn main:app --reload
```

Backend URL:

```text
http://127.0.0.1:8000
```

Swagger Documentation:

```text
http://127.0.0.1:8000/docs
```

## Run Streamlit Frontend

Open a new terminal and run:

```bash
streamlit run app.py
```

Frontend URL:

```text
http://localhost:8501
```

## API Request Example

### POST Request

```json
{
    "age": 25,
    "sex": "male",
    "bmi": 28.5,
    "children": 2,
    "smoker": "no",
    "region": "northwest"
}
```

### Response

```json
{
    "predicted_insurance_charge": 14567.23
}
```

## Machine Learning Workflow

1. Data Collection
2. Data Cleaning
3. Exploratory Data Analysis
4. Feature Encoding
5. Model Training
6. Model Evaluation
7. Model Saving
8. FastAPI Deployment
9. Streamlit Integration

## Future Improvements

* Docker Deployment
* Cloud Hosting (Render/AWS)
* User Authentication
* Model Monitoring
* Better UI Design

## Author

👨‍💻 **Shivam Pathak**

GitHub: [shivampathak91][(https://github.com/shivampathak91)]

## License

This project is licensed under the MIT License.

⭐ If you found this project helpful, consider giving it a star on GitHub.
