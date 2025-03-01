# Automated_Essay_Grading_for_TOEFL-
Automated Essay Grading Using Machine Learning An NLP and machine learning-based system for automated essay scoring (AES), trained on the ETS Corpus of Non-Native Written English to classify TOEFL essays into low, medium, and high proficiency levels. 

📌 Project Overview
Automatic essay scoring has been widely studied, but domain-specific datasets are often lacking. This project aims to:

✅ Develop an AES model using the TOEFL writing test dataset.

✅ Extract five linguistic features (text length, lexical richness, grammar correctness).

✅ Train and evaluate Random Forest, SVM, and Logistic Regression models.

✅ Identify which features and algorithms best predict student writing proficiency.


📂 Dataset
ETS Corpus of Non-Native Written English (Linguistic Data Consortium, 2014).
Contains 12,100 essays from TOEFL test-takers across 11 native languages.
Essays are labeled as low, medium, or high proficiency.
The raw CSV dataset is used without balancing to maintain real-world accuracy.

🛠️ Methods & Tools
Text Preprocessing: Tokenization, stopword removal, and punctuation cleaning (NLTK, Pandas).
Feature Engineering:

🔹 Text Length – Longer essays correlate with higher proficiency.

🔹 Lexical Richness Metrics – HDD & Yule’s K for vocabulary diversity.

🔹 Grammar Analysis – Detecting correct and incorrect passive voice using spaCy Matcher.
Machine Learning Models:

🔹 Random Forest, SVM, Logistic Regression (with hyperparameter tuning).

🔹 Evaluation Metrics: Accuracy, Precision, Recall, F1-score, and Quadratic Weighted Kappa (QWK).

📊 Key Findings
Best-performing features: TF-IDF + Text Length + HDD yielded the highest accuracy (72%).
Best-performing model: Tuned Logistic Regression (66% accuracy, QWK = 0.33).
Grammar features (passive voice detection) had a lower impact on model performance.
Future work: Adding semantic features (topic cohesion, coherence) could further improve predictions.

🚀 Future Improvements
Implement Transformer-based models (BERT, GPT) for improved scoring.
Expand feature engineering to include cohesion, argument structure, and topic relevance.
Fine-tune models using a larger and more balanced dataset.

Corpus Reference: TOEFL iBT®. (2024) _Integrated Writing Rubric._ Retrieved from https://www.ets.org/toefl.html
