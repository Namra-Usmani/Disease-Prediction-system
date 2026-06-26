# 🏥 Disease Prediction System

A machine learning-powered web application built with Django that predicts diseases based on user-provided symptoms. Designed to assist users in identifying potential health conditions early and seeking appropriate medical care.

---

## 🚀 Features

- **Symptom-based disease prediction** using trained ML models
- **Multiple disease support** — predicts across a range of conditions
- **User-friendly interface** built with Django templates
- **CSV-based disease data** for model training and reference
- **SQLite database** for lightweight local storage
- **Modular Django app structure** for easy extension

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python, Django |
| ML / Data | scikit-learn, pandas, NumPy |
| Database | SQLite3 |
| Frontend | HTML, CSS (Django Templates) |
| Data | CSV datasets (`disease_csvs/`) |

---

## 📁 Project Structure

```
dp_project/
│
├── dp_project/          # Django project settings & URLs
├── dpapp/               # Main Django app (views, models, ML logic)
├── disease_csvs/        # CSV datasets used for training/prediction
├── db.sqlite3           # SQLite database
├── manage.py            # Django management script
└── requirements.txt     # Python dependencies
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/Namra-Usmani/Disease-Prediction-system.git
cd Disease-Prediction-system
```

### 2. Create and activate a virtual environment

```bash
python -m venv venv

# Windows
venv\Scripts\activate

# macOS/Linux
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Apply database migrations

```bash
python manage.py migrate
```

### 5. Run the development server

```bash
python manage.py runserver
```

Open your browser and go to: **http://127.0.0.1:8000/**

---

## 🧠 How It Works

1. The user selects or enters their symptoms through the web interface.
2. The system processes the input and passes it to a trained machine learning model.
3. The model predicts the most likely disease(s) based on the symptom pattern.
4. Results are displayed to the user along with relevant information.

---

## 📊 Dataset

The project uses CSV files located in the `disease_csvs/` folder, which contain symptom-disease mappings used to train and evaluate the prediction model.

---

## 📦 Requirements

See [`requirements.txt`](requirements.txt) for the full list. Key dependencies include:

- Django
- scikit-learn
- pandas
- NumPy

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## ⚠️ Disclaimer

This application is intended for **educational purposes only**. It is not a substitute for professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare provider for medical concerns.

---

## 👩‍💻 Author

**Namra Usmani**  
[GitHub](https://github.com/Namra-Usmani)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
