# 🌸 ML Flower Classification

A machine learning web app that predicts Iris flower species in real time — trained on 6 different classifiers and deployed with Streamlit.

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red)
![scikit--learn](https://img.shields.io/badge/scikit--learn-ML-orange)

---

## 🚀 Live Demo
> 🔗 https://mihika-ml-app.streamlit.app/

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

All models were trained and evaluated on the classic Iris dataset (150 samples, 4 features, 3 balanced classes) with an 80/20 stratified train-test split. Test accuracy ranged from 96.67% to 100% across all six models. Full EDA, training, and evaluation (confusion matrices) is available in Flower_Classification_Project.ipynb.

## 🛠️ Tech Stack
- **Python**, **Pandas**, **NumPy**
- **scikit-learn** for model training
- **Matplotlib / Seaborn / Altair** for visualization
- **Streamlit** for the web app
- **Pickle** for model serialization

## 📂 Project Structure
```
├── App.py                                          # Streamlit app
├── Flower Classification Project.ipynb             # EDA + model training notebook
├── Logistic Regression.pkl
├── Naive Bayes.pkl
├── Decision Tree.pkl
├── Random Forest.pkl
├── SVM.pkl
├── KNN.pkl
├── requirements.txt
└── README.md
```

## 📸 Screenshots
> <img width="1920" height="865" alt="Screenshot (237)" src="https://github.com/user-attachments/assets/65d804df-2b20-4033-94c8-a054602f9a5c" />
> <img width="1920" height="856" alt="Screenshot (239)" src="https://github.com/user-attachments/assets/dbf3b341-310e-41b3-a4bb-efada6707eef" />
> <img width="1920" height="871" alt="Screenshot (240)" src="https://github.com/user-attachments/assets/cd2e5722-52bf-4b79-b9e4-e195e584f6ea" />
> <img width="1920" height="854" alt="Screenshot (241)" src="https://github.com/user-attachments/assets/83c43403-be0a-4e41-abca-245d9102f83b" />


## 📈 Results
All six models achieve strong accuracy (90%+) on the held-out test set, which is expected given how well-separated the Iris classes are. The comparison chart in the notebook shows exact scores per model.

## 🔮 Future Improvements
- Deploy on Streamlit Community Cloud and link it here
- Add model accuracy metrics directly in the app UI
- Replace per-model `.pkl` files with a single serialized dict for cleaner loading
- Add unit tests for the prediction pipeline

## 👩‍💻 Author
**Mihika Srivastava**
