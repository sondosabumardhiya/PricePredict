# PricePredict
This application uses artificial intelligence techniques to analyze smartphone specifications such as screen size, battery capacity, camera, and memory to estimate the expected price range of the device. It helps you make a smart purchasing decision and know the appropriate price before buying.

# Price Predictor - تنبئ بسعر

## Overview
This application predicts the **expected price range** of smartphones based on specifications like RAM, screen resolution, battery, and front camera. Users can input specs through a **web form** or interact with the **API**.

---

## Features
- Predict smartphone price range using **Random Forest** model.
- Provides a **web interface** for interactive prediction.
- Offers a **REST API** endpoint to integrate with other applications.
- Saves predictions for later use.
- Supports **scaling** of input features for accurate predictions.

---

## Installation

1. Clone the repository:
```bash
git clone https://github.com/your-username/price-predictor.git
cd price-predictor




Run the Flask app:
python app.py

4.Open in browser: http://127.0.0.1:5000/

5.Use the form to input mobile specifications and get a predicted price range.


*Django Version (Optional)

If you prefer Django, the project initially used it:

Models and forms handle user input

Views handle model inference and scaling

Admin panel to view saved predictions

Excel export of predictions

To use Django, configure views.py, urls.py, templates, and load the saved pickle model and scaler.

🧮 API Usage

Endpoint: /predict_api
Method: POST
Content-Type: application/json

Example JSON payload:
{
  "ram": 2048,
  "fc": 5,
  "px_width": 720,
  "px_height": 1280,
  "battery_power": 4000
}
Response:
{
  "Predicted Price Range": 2
}
💾 حفظ النموذج / Saving the Model

We saved the trained model and scaler using pickle:
import pickle

# Save model
with open('xgb_model.pkl', 'wb') as f:
    pickle.dump(xgb_model, f)

# Save scaler
with open('scaler.pkl', 'wb') as f:
    pickle.dump(scaler, f)

📚 وصف المشروع / Project Description

English:
This application uses AI techniques to analyze phone specifications (screen size, battery, camera, memory) and estimate the expected price range. It helps users make smart buying decisions and know the appropriate price before purchasing.
