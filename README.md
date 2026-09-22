# Employee Performance Predictor

A Streamlit web app that predicts whether an employee's performance is likely to be good or needs improvement based on two inputs:

- Training hours
- Attendance percentage

The app loads a trained Keras neural-network model and provides instant predictions in a simple dashboard.

## Features

- User-friendly interface built with Streamlit
- Real-time prediction from a saved TensorFlow model
- Input validation for training hours and attendance
- Clear result display with probability and input summary

## Project Structure

- `app.py` – Streamlit application
- `employee_performance_ann.keras` – trained ANN model
- `requirements.txt` – Python dependencies

## Requirements

- Python 3.10+
- pip

## Setup

1. Open a terminal in the project folder.
2. Create and activate a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

3. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

## Run the App

```bash
streamlit run app.py
```

Then open the local URL shown in the terminal, usually:

```text
http://localhost:8501
```

## How It Works

The app accepts:

- Training Hours: number of hours an employee spent in training
- Attendance (%): employee attendance percentage

It sends these values to the trained ANN model and displays:

- Performance result: Good or Needs Improvement
- Probability score as a percentage

## Notes

This project is a lightweight machine learning demo and is intended for educational or prototype use.
