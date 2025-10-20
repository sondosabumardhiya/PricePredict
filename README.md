

# 📱 Price Prediction using Django & Random Forest

## 🧠 Overview

This project is a **Django-based web application** that predicts  prices based on hardware specifications using a **Random Forest Machine Learning model**.
The system provides a simple web interface to input phone specs and get a predicted price range instantly.

---

## ⚙️ Technologies Used

| Category                 | Tools                            |
| ------------------------ | -------------------------------- |
| Framework                | **Django**                       |
| Machine Learning         | **scikit-learn**, **joblib**     |
| Data Processing          | **pandas**, **numpy**            |
| Visualization (Optional) | **matplotlib**                   |
| Frontend                 | **HTML**, **CSS**, **Bootstrap** |

---

## 🧩 Project Structure

```
📂 myproject/
│
├── manage.py
├── db.sqlite3
├── random_forest_model1.pkl       # Saved ML model
├── scaler1.pkl                    # Scaler used for preprocessing
│
├── 📁 myapp/                       # Main app
│   ├── views.py                    # Prediction functions
│   ├── urls.py                     # Page routes
│   ├── models.py                   # (Optional - if saving data)
│   └── templates/
│       ├── home.html              
│       └── prediction.html        
│
├── 📁 static/                      # Design files (CSS / images)
│   └── pict2.jpg                   # Example background image
│
└                    
```

---

## 🚀 How to Run

### 1️⃣ Install Requirements

```bash
pip install django pandas numpy scikit-learn matplotlib joblib
```

### 2️⃣ Run the Server

```bash
python manage.py runserver
```

Open in your browser:

```
http://127.0.0.1:8000/
```

---

## 🧮 How It Works

1. The user enters phone specifications on the homepage.
2. Django reads the values and sends them to the saved model (`random_forest_model1.pkl`).
3. The model predicts the appropriate price category ((1)Low –(2) Medium –(3) High ).
4. The result is displayed clearly on the **prediction.html** page.

---

## 📁 Important Files

| File                       | Purpose                            |
| -------------------------- | ---------------------------------- |
| `random_forest_model1.pkl` | Saved Random Forest model          |
| `scaler1.pkl`              | Data scaler used before prediction |
| `home.html`                | Information about the application  |
| `prediction.html`          | Input & Result display page        |

---

## 🌟 Example

🧩 User inputs the following values:

* RAM = 6 GB
* Battery = 4000 mAh
* Camera = 12 MP
* Storage = 128 GB

Output:

> 💰 **Predicted Price Range: (3) High**

---

## 🧑‍💻 Author

**Sondos**
Project built with ❤️ using **Django** and **Machine Learning**.

---

## 📜 License

Open-source for learning and research purposes.

