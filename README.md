<div align="center">

# Machine Failure Prediction System ⚙️

<p>
  <img src="https://img.shields.io/badge/✅_Completed-2ea44f?style=flat-square" alt="Completed"/>
  &nbsp;
  <img src="https://img.shields.io/badge/🌐_Full_Stack_Web-0969da?style=flat-square" alt="Full-stack web"/>
  &nbsp;
  <img src="https://img.shields.io/badge/🤖_Machine_Learning-7c3aed?style=flat-square" alt="ML"/>
  &nbsp;
  <img src="https://img.shields.io/badge/🛢️_Aramco_Internship-006630?style=flat-square" alt="Aramco"/>
  &nbsp;
</p>

A proactive AI tracking system that predicts potential **machine failures** before they occur — built during a 2-month summer training at **Aramco's Distribution Projects Division** to enhance safety, reduce downtime, and optimize maintenance in industrial operations.

</div>

---

<div align="center">
  <img src="images/AppPortfolio.gif" alt="PreCheck App Demo" width="97%"/>
</div>

<p align="center">
  <img src="images/ResultPage.png" alt="Prediction Results" width="32%"/>
  <img src="images/PrecheckMockup.png" alt="PreCheck Mockup" width="32%"/>
  <img src="images/Database.png" alt="Records Database" width="32%"/>
</p>

---

## 📌 About The Project

In Aramco's Distribution Projects Division, equipment was frequently used without proper pre-use checks — leading to unexpected failures, safety risks, project delays, and increased maintenance costs.

**PreCheck** solves this by leveraging machine learning to analyze equipment parameters (torque, tool wear time, process temperature) and predict whether a machine will fail — and what type of failure to expect — before it happens. The system was built end-to-end: from data analysis and model training to a full web interface accessible to non-technical stakeholders.

### ✨ Key Features

| Feature | Description |
|:--|:--|
| **Failure Prediction Engine** | Input machine parameters and receive real-time predictions on failure type and probability |
| **Multi-Class Classification** | Detects 5 failure types: Heat Dissipation, Power, Overstrain, Tool Wear, and Random Failures |
| **Equipment Records Database** | Save predictions with Equipment IDs and browse historical records with pagination |
| **User-Friendly Web Interface** | Built for non-technical users with a How-to-Use guide, FAQs, and clean navigation |

---

## 🏆 Results & Performance

| Metric | Score |
|:--|:--|
| Final Model | **BalancedRandomForestClassifier** |
| F1 Score | **89%** |
| Geometric Mean Score | **89%** |
| Failure Types Detected | **5 categories** |

The model was selected after experimenting with SVM, Neural Networks (MLPClassifier), and Ensemble Methods (ExtraTreeClassifier), then optimized via GridSearchCV hyperparameter tuning with cross-validation to ensure robustness and generalization.

---

## 🛠️ Built With

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" alt="Flask"/>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" alt="scikit-learn"/>
  <img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" alt="Colab"/>
</p>

| Layer | Technology | Role |
|:--|:--|:--|
| **ML Model** | Python, scikit-learn | BalancedRandomForestClassifier with SMOTEENN, PCA, GridSearchCV |
| **Backend** | Flask | API endpoints, model integration, data storage & retrieval |
| **Frontend** | HTML, CSS, JavaScript | Responsive UI with predictor form, results display, and records table |
| **Data Analysis** | Python, Google Colab | EDA, feature engineering, visualization, model experimentation |

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────┐
│           Frontend (HTML / CSS / JS)            │
│    Main Page · Predictor · Records · FAQs       │
└──────────────────────┬──────────────────────────┘
                       │
              ┌────────▼────────┐
              │  Flask Backend  │
              │  API · Routing  │
              │  Data Storage   │
              └────────┬────────┘
                       │
              ┌────────▼────────┐
              │   ML Pipeline   │
              │ ┌─────────────┐ │
              │ │Preprocessing│ │
              │ │ SMOTEENN +  │ │
              │ │ PCA + Scale │ │
              │ └─────────────┘ │
              │ ┌─────────────┐ │
              │ │  Balanced   │ │
              │ │ RandomForest│ │
              │ │ Classifier  │ │
              │ └─────────────┘ │
              └────────┬────────┘
                       │
              ┌────────▼────────┐
              │    Prediction   │
              │ Failure Type +  │
              │  Probability    │
              └─────────────────┘
```

---

<div align="center">

<img src="https://img.shields.io/badge/+2-Languages-E8912D?style=flat-square&labelColor=1a1a2e" alt="Languages"/>
&nbsp;
<img src="https://img.shields.io/badge/+1-Framework-000000?style=flat-square&labelColor=1a1a2e" alt="Framework"/>
&nbsp;
<img src="https://img.shields.io/badge/+3-ML_Algorithms-7c3aed?style=flat-square&labelColor=1a1a2e" alt="ML"/>
&nbsp;
<img src="https://img.shields.io/badge/+3-Frontend_Stack-e34f26?style=flat-square&labelColor=1a1a2e" alt="Frontend"/>
&nbsp;
<img src="https://img.shields.io/badge/+2-Platforms_&_Tools-16a34a?style=flat-square&labelColor=1a1a2e" alt="Tools"/>
&nbsp;
<img src="https://img.shields.io/badge/+11-Technologies_Total-e05d44?style=flat-square&labelColor=1a1a2e" alt="Total"/>

</div>
