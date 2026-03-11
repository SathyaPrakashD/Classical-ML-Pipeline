# Classical ML Pipeline — Iris Species Classifier

A beginner-to-production sklearn workflow built as a hands-on exercise to consolidate core scikit-learn concepts:
preprocessing, pipelines, model training, and evaluation.

---

## 🎯 Project Purpose

This project demonstrates a **complete classical ML workflow** using scikit-learn — from raw data to a evaluated, production-style pipeline.

Built as part of the **BITS Pilani AI & MLOps Engineering Program** learning path, following foundational study of the scikit-learn library.

---

## 🧠 Concepts Covered

| Concept | sklearn Module |
|---|---|
| Train/test splitting | `sklearn.model_selection` |
| Feature scaling | `sklearn.preprocessing` |
| Chaining steps into one object | `sklearn.pipeline` |
| Model training | `sklearn.linear_model` |
| Performance evaluation | `sklearn.metrics` |

---

## 📁 Project Structure

```
├── README.md
└── iris_classifier.ipynb       # Main Colab notebook — full workflow
```

---

## 📊 Dataset

**Iris Dataset** — built into sklearn (`sklearn.datasets.load_iris`)

- 150 samples
- 4 input features: sepal length, sepal width, petal length, petal width
- 3 target classes: Setosa, Versicolour, Virginica
- No missing values — clean, focused dataset ideal for learning workflows

---

## ⚙️ Workflow

```
Raw Data
    ↓
Train / Test Split          (80% train, 20% test)
    ↓
StandardScaler              (scale numeric features)
    ↓
Logistic Regression         (train classifier)
    ↓
classification_report       (precision, recall, F1 per class)
```

---

## 🚀 How to Run

1. Open `iris_classifier.ipynb` in [Google Colab](https://colab.research.google.com/)
2. Run all cells in sequence
3. No additional installations required — all libraries are available in Colab by default

---

## 📈 Output

Running the notebook produces a `classification_report` showing:
- **Precision** — of all predictions per class, how many were correct
- **Recall** — of all actual samples per class, how many were caught
- **F1 Score** — balance between precision and recall
- **Accuracy** — overall correctness across all classes

---

## 🔑 Key Learning

> A `Pipeline` chains preprocessing and model training into one deployable object.
> `fit()` on training data. `predict()` on test data. The pipeline handles the rest.

---

## 🗺️ What's Next

This exercise is a stepping stone toward:
- Custom preprocessors (MadeWithML `CustomPreprocessor`)
- Multi-column preprocessing with `ColumnTransformer`
- Text classification pipelines with `TfidfVectorizer`
- Production ML with Ray / Anyscale (MadeWithML training module)

---

## 👤 Author

Built by Sathya as part of the BITS Pilani Digital AI Engineering & MLOps Program learning path.
