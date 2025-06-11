# ⚙️ MLops Data Science Project

An end-to-end Machine Learning pipeline built with **Python**, following MLOps best practices. This project covers everything from data preprocessing and model training to evaluation, tracking with **MLflow**, and deployment using a simple **Flask web interface**.

---

## 📸 Demo

![Demo Screenshot](https://github.com/Sarang9Gupta/MLops-Data-Science-Project/assets/demo-screenshot-placeholder)

> *(Replace the image link above with a real screenshot or gif if available)*

---

## 📦 Features

- 📊 **Data Preprocessing Pipeline**: Handles missing values, encodes features, and scales input data.
- 🧠 **Model Training Pipeline**: Trains ML models using scikit-learn and saves artifacts.
- ✅ **Model Evaluation**: Calculates R², MSE, RMSE and logs results.
- 📈 **MLflow Tracking**: Automatically logs parameters, metrics, and artifacts for every run.
- 🌐 **Flask UI**: Simple web app to input data and get predictions.
- 📁 **Modular Codebase**: Clean structure with components, pipelines, and utility scripts.
- 💾 **Model & Scaler Persistence**: Saves models and scalers using `joblib`.

---

## 🗂️ Project Structure

```bash
📁 MLops-Data-Science-Project/
├── data/                     # Raw and processed datasets
├── notebooks/                # EDA and experimentation notebooks
├── src/
│   ├── mlProject/
│   │   ├── components/       # Data transformation, training, evaluation
│   │   ├── pipeline/         # Training and prediction pipelines
│   │   ├── utils/            # Logger, file handling, config
│   ├── main.py               # Main training script (with MLflow)
│   ├── app.py                # Flask app for serving predictions
├── mlruns/                   # MLflow logging directory
├── requirements.txt          # Python dependencies
├── .gitignore                # Files to ignore in Git
└── README.md                 # Project documentation
```

---

## 🛠️ Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/Sarang9Gupta/MLops-Data-Science-Project.git
cd MLops-Data-Science-Project
```

### 2. Create Conda Environment

```bash
conda create -n mlops-env python=3.8 -y
conda activate mlops-env
```


### 3. Install Requirements

```bash
pip install -r requirements.txt
```

### 4. (Optional) Set Up MLflow UI

To view and track experiments visually:

```bash
mlflow ui
```

Then open:

```bash
http://127.0.0.1:5000
```

---

## 🚀 How to Use

### 🔧 Train the Model

```bash
python src/main.py
```

- Loads and preprocesses data
- Trains a regression model
- Logs metrics and artifacts to MLflow
- Saves model and preprocessor objects

### 🌐 Launch Flask App

```bash
python src/app.py
```

Then open:

```bash
http://127.0.0.1:5000
```

Enter input values in the form and get instant predictions.

---

## 📊 MLflow Integration

MLflow is used for:

- 📋 Logging model parameters (like algorithm type, hyperparameters)
- 📈 Tracking metrics such as R², RMSE
- 📦 Storing artifacts (models, scalers)
- 📚 Comparing multiple training runs visually through MLflow UI

> All experiments are stored in the `mlruns/` directory by default.

---

## 📌 Requirements

- Python 3.8+
- scikit-learn
- pandas
- numpy
- Flask
- joblib
- mlflow

To export your environment, use:

```bash
pip freeze > requirements.txt
```

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo  
2. Create a new branch: `git checkout -b feature/your-feature`  
3. Commit your changes  
4. Push your branch and open a Pull Request

---

## 📝 License

This project is licensed under the MIT License.  
See the [LICENSE](LICENSE) file for more details.

---

## 📬 Contact

**Created by Sarang Gupta**  
🔗 GitHub: [@Sarang9Gupta](https://github.com/Sarang9Gupta)  
✉️ Email: sarang9gupta@gmail.com

---

⭐ **If you found this helpful, consider giving it a star!**
