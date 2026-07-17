# 🌸 ML Flower Classification

A machine learning web app that predicts Iris flower species in real time — trained on 6 different classifiers and deployed with Streamlit.

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red)
![scikit--learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 🚀 Live Demo
> 🔗 *Add your Streamlit Cloud link here once deployed*
> Example: [flower-classification.streamlit.app](https://share.streamlit.io)

---

## 📌 Overview
This project classifies Iris flowers (**Setosa**, **Versicolor**, **Virginica**) based on 4 features — sepal length, sepal width, petal length, and petal width.

Instead of relying on a single model, this app trains **six different classifiers**, compares their performance side by side, and combines their predictions using a **majority-vote ensemble** for the final answer.

## ✨ Features
- 🎚️ Interactive sliders to input flower measurements
- 🤖 Live predictions from **6 ML models** simultaneously
- 📊 Model confidence comparison chart (Altair)
- 🗳️ Final prediction via majority voting across all models
- 📁 Clean, ready-to-run Streamlit interface

## 🧠 Models Used
| Model | Type |
|---|---|
| Logistic Regression | Linear |
| Naive Bayes (Gaussian) | Probabilistic |
| Decision Tree | Tree-based |
| Random Forest | Ensemble |
| SVM | Margin-based |
| KNN | Instance-based |

All models were trained and evaluated on the classic **Iris dataset** (150 samples, 4 features, 3 balanced classes) with an 80/20 stratified train-test split. Full EDA, training, and evaluation (accuracy scores + confusion matrices) is available in [`Flower_Classification_Project.ipynb`](./Flower_Classification_Project.ipynb).

## 🛠️ Tech Stack
- **Python**, **Pandas**, **NumPy**
- **scikit-learn** for model training
- **Matplotlib / Seaborn / Altair** for visualization
- **Streamlit** for the web app
- **Pickle** for model serialization

## 📂 Project Structure
```
├── App.py                              # Streamlit app
├── Flower_Classification_Project.ipynb # EDA + model training notebook
├── Logistic Regression.pkl
├── Naive Bayes.pkl
├── Decision Tree.pkl
├── Random Forest.pkl
├── SVM.pkl
├── KNN.pkl
├── requirements.txt
└── README.md
```

## ⚙️ Run Locally
```bash
git clone https://github.com/Mihikaaaaa/ML_Flower.Classification.git
cd ML_Flower.Classification
pip install -r requirements.txt
streamlit run App.py
```

## 📸 Screenshots
> *Add a screenshot or GIF of the sliders + prediction + comparison chart here — this sells the project instantly to anyone browsing your repo.*

## 📈 Results
All six models achieve strong accuracy (90%+) on the held-out test set, which is expected given how well-separated the Iris classes are. The comparison chart in the notebook shows exact scores per model.

## 🔮 Future Improvements
- Deploy on Streamlit Community Cloud and link it here
- Add model accuracy metrics directly in the app UI
- Replace per-model `.pkl` files with a single serialized dict for cleaner loading
- Add unit tests for prediction pipeline

## 👩‍💻 Author
**Mihika Srivastava**
Made with ❤️ using Streamlit

## 📄 License
This project is licensed under the MIT License.
