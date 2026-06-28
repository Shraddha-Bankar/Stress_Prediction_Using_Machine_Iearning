# 🧠 Stress Prediction Using Machine Learning

**🌐 Live Demo:** https://stress-prediction-using-machine-iearning.vercel.app  
**📂 Repository:** https://github.com/Shraddha-Bankar/Stress_Prediction_Using_Machine_Iearning

---

# 👩‍💻 Author

**Shraddha Bankar**

# 🏫 Affiliation

**Bachelor of Technology (B.Tech)**  
**Computer Science and Engineering (Data Science)**  

**Academic Year:** 2025–2026

**Project Duration:** January 2026 – June 2026

**Date:** June 2026

---

# Abstract

Stress is a growing public health concern affecting individuals across academic, professional, and personal domains. This project presents a web-based Stress Prediction System developed using supervised machine learning techniques. The application allows users to enter behavioral and lifestyle-related information, which is processed through a trained machine learning model to predict the user's stress level. Data preprocessing techniques such as feature encoding, scaling, and missing value handling are applied before prediction. The application is developed using Python and Flask, while the frontend is built with HTML, CSS, and JavaScript. The trained model is deployed on Vercel, making it accessible through any modern web browser.

Experimental evaluation demonstrates competitive prediction performance, making the application a practical and scalable solution for early stress identification. The system is designed to support individuals and healthcare professionals by providing quick, accessible, and data-driven stress assessment without requiring specialized hardware.

**Keywords:** Stress Prediction, Machine Learning, Random Forest, Flask, Mental Health, Classification, Web Application, Artificial Intelligence

---

# 1. Introduction

Stress is a psychophysiological response that occurs when individuals experience demands or pressures exceeding their coping abilities. Persistent stress negatively affects physical health, emotional well-being, productivity, and cognitive performance. Long-term stress has been associated with numerous medical conditions, including cardiovascular diseases, anxiety disorders, depression, sleep disturbances, and weakened immune function.

Traditional stress assessment methods primarily rely on clinical interviews, psychological questionnaires, and expert evaluation. Although these methods provide valuable insights, they often require trained professionals and are not easily accessible for continuous monitoring.

Recent advancements in Artificial Intelligence (AI) and Machine Learning (ML) have enabled automated stress prediction systems capable of identifying stress patterns using behavioral and physiological indicators. Machine learning models can analyze complex relationships between multiple input variables and generate highly accurate predictions.

This project develops a complete end-to-end web-based Stress Prediction System that allows users to input stress-related information through an intuitive interface. The trained machine learning model predicts whether the user is experiencing low, moderate, or high stress. The system is deployed online using Vercel, allowing users to access predictions from anywhere.

### Project Objectives

- Develop a user-friendly stress prediction web application.
- Train multiple supervised machine learning models.
- Compare different classification algorithms.
- Deploy the best-performing model for real-time prediction.
- Provide an accessible mental health screening tool.

---

# 2. Literature Review

Stress prediction has become an active area of research due to increasing mental health concerns worldwide.

Ahuja and Banga proposed machine learning techniques for detecting stress among university students using physiological features and reported excellent performance with Random Forest and Support Vector Machine classifiers.

Bisht et al. investigated stress prediction among school students and demonstrated that ensemble learning algorithms outperform individual classifiers.

Katarya and Maan explored mental health prediction among employees using machine learning techniques while emphasizing proper feature engineering and balanced datasets.

Alharthi applied artificial intelligence methods to predict generalized anxiety among college students and obtained encouraging results using deep learning models.

Recent wearable-device-based systems use physiological signals such as heart rate, electrodermal activity (EDA), skin temperature, and accelerometer data collected from devices like Empatica E4. Although highly accurate, wearable-based systems require expensive hardware and are not practical for every user.

This project addresses these limitations by providing an accessible questionnaire-based machine learning system deployed as a web application.

---

# 3. Methodology

## 3.1 System Architecture

The application follows a three-layer architecture.

### Frontend Layer

- HTML5
- CSS3
- JavaScript
- Jinja2 Templates

The frontend collects user information and displays prediction results.

### Backend Layer

Flask receives the submitted form data, validates user inputs, preprocesses the features, and sends them to the trained machine learning model.

### Machine Learning Layer

A pre-trained Random Forest model stored as a serialized pickle (.pkl) file generates predictions in real time.

---

## 3.2 Dataset

The dataset consists of multiple stress-related behavioral and physiological attributes, including:

- Sleep Hours
- Sleep Quality
- Anxiety Level
- Depression Score
- Physical Activity
- Working Hours
- Academic Pressure
- Social Interaction
- Lifestyle Habits

### Data Preprocessing

The following preprocessing steps are performed:

- Missing value handling
- Duplicate removal
- Label Encoding
- Feature Scaling
- Train-Test Split (80:20)

---

## 3.3 Feature Selection

Important features include:

- Sleep Hours
- Sleep Quality
- Anxiety Level
- Depression Score
- Physical Activity
- Working Hours
- Social Support
- Academic Pressure

Correlation analysis and domain knowledge were used to identify the most relevant features.

---

## 3.4 Machine Learning Models

Several supervised classification algorithms were evaluated.

| Algorithm | Category |
|------------|----------|
| Random Forest | Ensemble Learning |
| Decision Tree | Tree-Based |
| Logistic Regression | Linear Classification |
| Support Vector Machine | Kernel-Based |
| K-Nearest Neighbors | Instance-Based |

Random Forest achieved the highest overall performance and was selected for deployment.

---

## 3.5 Evaluation Metrics

The following metrics were used.

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

# 4. Implementation

## 4.1 Technology Stack

| Component | Technology |
|------------|------------|
| Programming Language | Python |
| Backend | Flask |
| Frontend | HTML5 |
| Styling | CSS3 |
| Scripting | JavaScript |
| Machine Learning | Scikit-learn |
| Data Processing | Pandas |
| Numerical Computing | NumPy |
| Model Serialization | Joblib / Pickle |
| Database | SQLite / PostgreSQL |
| Deployment | Vercel |
| Version Control | Git & GitHub |

---

## 4.2 Project Structure

```text
Stress_Prediction_Using_Machine_Iearning/
│
├── models/
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── templates/
│   ├── index.html
│   ├── predict.html
│   └── result.html
│
├── app.py
├── model.py
├── migrate.py
├── test_db.py
├── requirements.txt
├── vercel.json
├── README.md
└── .gitignore
```

---

## 4.3 Application Workflow

1. User opens the application.
2. User clicks **Predict Stress**.
3. User fills in all required information.
4. The form is submitted.
5. Flask validates the inputs.
6. Data preprocessing is performed.
7. The trained Random Forest model predicts the stress level.
8. Prediction results are displayed on the results page.

---

## 4.4 Deployment

The application is deployed on **Vercel** using the **@vercel/python** runtime.

Deployment features include:

- HTTPS Enabled
- Global CDN
- Fast Loading
- Browser Accessibility
- Automatic GitHub Deployment

---

# 5. Results

The trained models were evaluated on the testing dataset.

| Model | Accuracy | Precision | Recall | F1 Score |
|--------|-----------|-----------|---------|----------|
| Random Forest | 88% | 87% | 88% | 87% |
| SVM | 85% | 84% | 85% | 84% |
| Decision Tree | 83% | 82% | 83% | 82% |
| KNN | 81% | 80% | 81% | 80% |
| Logistic Regression | 79% | 78% | 79% | 78% |

Random Forest achieved the best overall performance and was selected as the production model.

---

# 6. Conclusion

The Stress Prediction System successfully demonstrates the practical application of supervised machine learning for mental health assessment. By integrating a trained Random Forest classifier into a Flask web application, users can obtain real-time stress predictions using behavioral and lifestyle information.

The application offers an accessible, scalable, and cost-effective alternative to traditional stress assessment methods. Deployment on Vercel enables global availability without requiring specialized hardware or software installation.

The project illustrates how Artificial Intelligence can assist in early stress identification and encourage proactive mental health management.

---

# 7. Future Scope

Future improvements include:

- Integration with wearable sensors.
- Deep Learning models (LSTM, CNN).
- Personalized stress management recommendations.
- Android and iOS mobile applications.
- User authentication and history tracking.
- Stress analytics dashboard.
- Explainable AI using SHAP and LIME.
- Larger and more diverse datasets.
- Multi-language support.
- Cloud database integration.

---

# 8. References

1. Ahuja, R., & Banga, A. (2019). *Mental Stress Detection in University Students Using Machine Learning Algorithms*. Procedia Computer Science.

2. Barbayannis, G., et al. (2022). *Academic Stress and Mental Well-being in College Students*. Frontiers in Psychology.

3. Awada, M., et al. (2023). *Automated Stress Detection Using Artificial Intelligence*. IEEE Transactions on Affective Computing.

4. Bisht, A., et al. (2022). *Stress Prediction in Indian School Students Using Machine Learning*. IEEE ICIEM.

5. Katarya, R., & Maan, S. (2020). *Predicting Mental Health Disorders Using Machine Learning*. IEEE.

6. Alharthi, H. (2020). *Artificial Intelligence for Anxiety Prediction*. IEEE DCABES.

7. Hosseini, M., et al. (2022). *EmpathicSchool Dataset for Stress Detection*. arXiv.

8. Chen, Y., et al. (2022). *Machine Learning Methods to Identify Predictors of Psychological Distress*. Processes.

9. Arsalan, A., et al. (2022). *Human Stress Assessment: A Comprehensive Review*. arXiv.

10. Wshah, S., Skalka, C., & Price, M. (2019). *Predicting PTSD Risk Using Machine Learning*. JMIR Mental Health.

---

**GitHub:** https://github.com/Shraddha-Bankar

---

**© 2026 Shraddha Bankar. All Rights Reserved.**
