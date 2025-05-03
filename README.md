#  Abusive Comment Detection with MuRIL & Classical Models

This project aims to detect abusive, offensive, and non-abusive comments from text using advanced natural language processing (NLP) techniques. We leverage the pretrained **MuRIL (Multilingual Representations for Indian Languages)** model for high-accuracy multilingual classification, while also comparing the results with classical machine learning models such as **TF-IDF + SVM** and **XGBoost**.

---

##  Objective

- **Problem:** Classify comments into **abusive** and **non-abusive** categories based on content.
- **Solution:** Utilize **MuRIL**, a state-of-the-art transformer model for Indian languages, to accurately classify user comments. We also implement traditional models for comparison.

---

##  Dataset

The dataset used in this project consists of labeled text comments with three categories:

- **`AWM_train.csv`** – Training dataset
- **`AWM_dev.csv`** – Validation dataset
- **`AWM_test_without_labels.csv`** – Test dataset (no labels)

Each dataset contains:
- **Text**: The comment itself.
- **Label**: The corresponding category (abusive, offensive, non-abusive).

---

##  Key Features

- **Preprocessing**: Tokenization, cleaning, and text normalization using libraries like `nltk`, `emoji`, and regex.
- **Multilingual Support**: Trained and tested for Indian languages with MuRIL.
- **Models Implemented**: 
  - **MuRIL Transformer** for high-performance NLP.
  - **TF-IDF + SVM** and **XGBoost** as traditional ML baselines for comparison.
- **Evaluation Metrics**: Precision, Recall, F1-Score, Accuracy.

---

##  Installation

To get started, install the required dependencies:

```bash
pip install emoji nltk scikit-learn xgboost transformers torch datasets evaluate indic-nlp-library
```

---

##  How to Run

Follow these steps to run the project:

1. Clone the repository and navigate to the Jupyter notebook `Abusive_comment_detection_nw.ipynb`.
2. If using **Google Colab**, mount Google Drive:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

3. Ensure the dataset files (`AWM_train.csv`, `AWM_dev.csv`, `AWM_test_without_labels.csv`) are properly uploaded.
4. Run the notebook sequentially to:
   - Preprocess the data
   - Train **MuRIL** model
   - Evaluate the performance of **MuRIL** and classical models

---

##  Model Comparison

### Results:

| Model             | Accuracy | F1-Score | Precision | Recall   |
| ----------------- | -------- | -------- | --------- | -------- |
| **MuRIL**         | ✅ High   | ✅ High   | ✅ High    | ✅ High   |
| **TF-IDF + SVM**  | Moderate | Moderate | Moderate  | Moderate |
| **XGBoost**       | Moderate | Moderate | Moderate  | Moderate |

> **MuRIL** achieved significantly better performance, especially on multilingual and code-mixed data, outperforming classical models.

---

##  Author & Contributions

This project was developed as part of an NLP initiative to moderate comments on social media and detect abusive content. Contributions, feedback, and pull requests are encouraged!

---

```


