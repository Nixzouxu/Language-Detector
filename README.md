# Language-Detector
A simple Language Detection model using Multinomial Naïve Bayes trained on a balanced multilingual dataset (22 languages, 1000 samples each). Achieves 95.3% accuracy using CountVectorizer text features.

# 🌍 Language Detection using Multinomial Naïve Bayes

A Machine Learning project that detects the **language of a given text** using the **Multinomial Naïve Bayes** algorithm.  
The model is trained on a **balanced dataset** containing 22 languages with 1000 text samples each, achieving an accuracy of **95.3%**.

---

## 🧠 Project Overview
This project focuses on **text classification** for automatic **language detection**.  
By using `CountVectorizer` to convert text into numerical features, and applying the `MultinomialNB` classifier, the model learns to recognize language patterns based on word frequency.

---

## 📂 Dataset
- **Total samples:** 22,000  
- **Languages:** Estonian, Swedish, Thai, Tamil, Dutch, Japanese, Turkish, Latin, Urdu, Indonesian, Portuguese, French, Chinese, Korean, Hindi, Spanish, Pushto, Persian, Romanian, Russian, English, Arabic.  
- Each language contains **1000 text entries**, making it a **balanced dataset**.

---

## ⚙️ Technologies Used
- Python 🐍  
- NumPy  
- Pandas  
- Scikit-learn  
- Jupyter Notebook  

---

## 🚀 Model Workflow
1. **Load and inspect dataset**  
2. **Clean and check for missing data**  
3. **Vectorize text** using `CountVectorizer`  
4. **Split data** into training (67%) and testing (33%)  
5. **Train model** using `MultinomialNB`  
6. **Evaluate accuracy** (95.3%)  
7. **Predict language** for new input text

---

## 🧾 Example Usage

```python
user = input("Enter a text: ")
data = cv.transform([user]).toarray()
output = model.predict(data)
print(output)
