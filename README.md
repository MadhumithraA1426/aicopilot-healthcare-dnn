# AI Copilot for Elderly Healthcare Monitoring

A deep learning powered Flask web app to monitor elderly individuals for inactivity, abnormal movement patterns, and trigger real-time alerts to caregivers. This application leverages a trained DNN model and structured healthcare datasets for robust and reliable predictions.

---

## Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- Deep Neural Network (DNN) model for health event prediction
- User authentication (Sign up, Login)
- Patient dashboard with prediction history
- Real-time alert and monitoring simulation
- SQLite database with SQLAlchemy ORM
- Modular, fully-documented codebase (`models.py`, `forms.py`, `/templates/`)

---

## Demo

- Localhost: [http://127.0.0.1:5000](http://127.0.0.1:5000)
- (Add your Render/Heroku live link here once deployed)

---

## Installation

1. **Clone the repository:**
git clone https://github.com/MadhumithraA1426/aicopilot-healthcare-dnn.git
cd aicopilot-healthcare-dnn

2. **Set up Python 3.11 and a virtual environment:**
py -3.11 -m venv venv
venv\Scripts\activate

3. **Install dependencies:**
pip install --upgrade pip setuptools wheel
pip install -r requirements.txt

---

## Usage

1. **Model files:**  
Place your trained model (`elderly_model.pkl`) and scaler (`scaler.pkl`) inside the `/model` folder.

2. **Run Flask app:**
python app.py

3. **Access the web interface:**  
Visit [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## Project Structure

├── app.py
├── models.py
├── forms.py
├── requirements.txt
├── setup.cfg
├── Procfile
├── README.md
├── dataset/
│ └── health_monitoring.csv
├── model/
│ ├── elderly_model.pkl
│ ├── scaler.pkl
│ └── train_model.py
├── templates/
│ ├── index.html
│ ├── login.html
│ ├── register.html
│ └── dashboard.html
├── static/
│ └── style.css
└── .gitignore

---

## Technologies Used

- Flask (Web framework)
- Flask-SQLAlchemy (ORM)
- Flask-Login (sessions)
- Flask-WTF (form validation)
- scikit-learn (ML model and scaler)
- joblib (model persistence)
- HTML, CSS (UI templates)

---

## Dataset

- [UCI "Activity Recognition with Healthy Older People"](https://archive.ics.uci.edu/ml/datasets/Activity+Recognition+with+Healthy+Older+People)
- (Alternative) ["AI for Elderly Care and Support" on Kaggle](https://www.kaggle.com/datasets)

Sample working dataset is provided in `/dataset`.

---

## Deployment

To deploy on Render or Heroku:

1. Ensure `Procfile`, `requirements.txt`, and `setup.cfg` are present.
2. Set up environment variable `SECRET_KEY`.
3. Push the repo and follow platform deployment steps.

---

## Contributing

Contributions and suggestions are welcome!  
Open issues, submit pull requests, or contact for collaboration.

---

## License

This project is licensed under the MIT License.
