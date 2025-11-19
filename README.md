Flood-Forecasting-using-Meachine-Learning
Developed a predictive model to forecast flood risks based on rainfall and river-level data using algorithms such as Random Forest and XGBoost.

This project predicts the possibility of floods based on monthly rainfall data using different Machine Learning classification algorithms. The system includes a Tkinter GUI that allows users to load a dataset, train models, compare algorithm accuracy, visualize rainfall patterns, and input custom values for prediction.

🧾 Project Overview

The model uses historical rainfall data to classify whether a flood is likely to occur. The system compares multiple machine learning algorithms such as:

| Algorithm | Accuracy (approx.) |
|----------|:------------------:|
| KNN      | 70.83% |
| Logistic Regression | 87.50% |
| SVM      | 79.17% |
| Decision Tree | 58.33% |
| Random Forest | 83.33% |

Logistic Regression performs best in this dataset and is also used for final flood prediction in the GUI.

🧰 Technologies Used
- Python
- Tkinter for GUI
- Pandas & NumPy for data handling
- scikit-learn for ML model training
- Matplotlib & Seaborn for visualization

 📊 Dataset
The dataset contains rainfall values for months, along with a target label:

| Feature Columns (Sample) |
|--------------------------|
| Year, JAN, FEB, MAR, APR, MAY, JUN, JUL, AUG, SEP, OCT, NOV, DEC, FLOODS |

FLOODS = 1 → Flood Occurred  
FLOODS = 0 → No Flood  

🎛️ GUI Features

| Feature | Description |
|--------|-------------|
| Upload Dataset | Load CSV rainfall dataset |
| Split Dataset | Splits data into train-test sets |
| Run Algorithms | Train KNN, Logistic, SVM, DT, RF |
| Show Accuracy Comparison | Displays bar chart results |
| Generate Histogram | Displays monthly rainfall trends |
| Enter Custom Values | Manually input rainfall data for prediction |
| Predict Flood | Predicts flood occurrence using trained model |

🏗️ How to Run the Project

1. Install Requirements
bash
pip install -r req.txt
2. Run the Application
bash
Copy code
python Flood_Forecasting_using_ML.py
A graphical window will open — follow on-screen steps.

📌 Example Output - Model Comparison Plot
makefile
Copy code
KNN: 0.7083
LR:  0.8750
SVM: 0.7917
DT:  0.5833
RF:  0.8333

🧠 Key Insights
Higher rainfall in July–September correlates strongly with flood occurrence.

Logistic Regression provided the highest balanced accuracy for this dataset.

Random Forest was a close second but slightly overfitted.

🚀 Future Improvements
Include real-time rainfall API data.

Convert GUI into a web dashboard (Flask/Streamlit).

Deploy prediction service as a cloud-based endpoint.

👤 Author
Abhilash Pitta
B.Tech – Computer Science Engineering
Email: pittaabhilash273@gmail.com
LinkedIn: https://www.linkedin.com/in/abhilash-pitta-164709204

