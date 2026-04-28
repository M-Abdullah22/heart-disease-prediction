# Heart Disease Prediction 🫀

A machine learning project that predicts whether a person is at risk of heart disease based on clinical health data, using Logistic Regression and Decision Tree classifiers.

## Objective

Load, clean, and analyze the Heart Disease UCI dataset, train classification models, and evaluate their performance using standard ML metrics.

## Dataset

The [Heart Disease UCI Dataset](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data) contains clinical records of 920 patients across 4 locations (Cleveland, Hungary, Switzerland, VA Long Beach).

Each record has 13 features used to predict the presence of heart disease:

| Feature | Description |
|---|---|
| `age` | Age of the patient |
| `sex` | Sex (1 = male, 0 = female) |
| `cp` | Chest pain type (0–3) |
| `trestbps` | Resting blood pressure (mm Hg) |
| `chol` | Serum cholesterol (mg/dl) |
| `fbs` | Fasting blood sugar > 120 mg/dl |
| `restecg` | Resting ECG results |
| `thalch` | Maximum heart rate achieved |
| `exang` | Exercise-induced angina |
| `oldpeak` | ST depression induced by exercise |
| `slope` | Slope of peak exercise ST segment |
| `ca` | Number of major vessels colored by fluoroscopy |
| `thal` | Thalassemia type |
| `target` | 0 = No disease, 1 = Heart disease |

## What This Project Covers

- Data loading and inspection using **pandas**
- Data cleaning — handling missing values with **median imputation**
- Exploratory Data Analysis (EDA) with **seaborn** and **matplotlib**
- Correlation heatmap to identify feature relationships
- Training two classification models — **Logistic Regression** and **Decision Tree**
- Model evaluation using **accuracy**, **confusion matrix**, and **ROC-AUC curve**
- **Feature importance** analysis to identify key health risk factors

## Results

| Model | Accuracy |
|---|---|
| Logistic Regression | ~83% |
| Decision Tree | ~80% |

> Results may vary slightly depending on train/test split.

## Libraries Used

- `pandas` — data loading and manipulation
- `numpy` — numerical operations
- `matplotlib` — base plotting
- `seaborn` — statistical visualizations
- `scikit-learn` — machine learning models and evaluation

## Project Structure

```
heart-disease-prediction/
│
├── data/
│   └── heart_disease_uci.csv   # Dataset
├── heart_disease.ipynb          # Main notebook
└── README.md                    # Project description
```

## How to Run

### Clone the repository
```bash
git clone https://github.com/M-Abdullah22/heart-disease-prediction.git
cd heart-disease-prediction
```

### Create virtual environment
```bash
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # Mac/Linux
```

### Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter ipykernel
```

### Run the notebook
```bash
jupyter notebook heart_disease.ipynb
```

## Key Learnings

- Binary classification using scikit-learn
- Handling missing values in medical datasets
- Understanding confusion matrix — especially the cost of false negatives in healthcare
- ROC-AUC curve interpretation
- Feature importance analysis using model coefficients and tree-based importances

## Author

**Syed M. Abdullah**
[LinkedIn](https://linkedin.com/in/syedmabdullah-dev) · [GitHub](https://github.com/M-Abdullah22)
