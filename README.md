# 🎓 Student Exam Performance Predictor  

## 📌 Overview  
This is an **end-to-end Machine Learning project** that predicts a student's **Math score** based on various features such as **gender, race, parental education, lunch type, test preparation course, reading score, and writing score**. The project follows a structured ML pipeline, and a **Flask web application** is built to take user input and display predictions.

```

## 🚀 Project Architecture  

- **artifacts/** 📂 *(Stores trained model and preprocessor)*  
  ├── model.pkl  
  ├── processor.pkl  
  ├── train.csv  
  ├── test.csv  
  ├── data.csv  

- **src/** 📂 *(Main source code directory)*  
  ├── **components/** 📂 *(ML pipeline components)*  
  │   ├── data_ingestion.py  
  │   ├── data_transformation.py  
  │   ├── model_trainer.py  
  │  
  ├── **pipeline/** 📂 *(Prediction pipeline)*  
  │   ├── predict_pipeline.py  
  │  
  ├── exception.py *(Custom exception handling)*  
  ├── logger.py *(Logging utility)*  
  ├── utils.py *(Helper functions)*  

- **templates/** 📂 *(HTML files for Flask app)*  
  ├── home.html  

- app.py *(Flask application file)*  
- setup.py *(Project setup script)*  
- README.md *(Project documentation - this file)*  

```

## 🔄 Project Workflow  

1. **Data Ingestion**:  
   - Reads the dataset (`data.csv`).
   - Splits it into training (`train.csv`) and testing (`test.csv`) sets.

2. **Data Transformation**:  
   - Encodes categorical variables.
   - Scales numerical features.

3. **Model Training**:  
   - Trains a **machine learning model** (e.g., Linear Regression, Decision Tree, or Random Forest).
   - Saves the model as `model.pkl`.

4. **Prediction Pipeline**:  
   - Loads the trained model and preprocessor.
   - Transforms user input and predicts the Math score.

5. **Flask App Development**:  
   - Provides a **web-based interface** for user input and predictions.
   - Runs locally (`127.0.0.1:5001`).




## 🎯 Features  

✅ **End-to-end ML pipeline** (from data ingestion to model deployment)  
✅ **Custom Exception Handling** for error tracking  
✅ **Logging** for debugging and monitoring  
✅ **Flask-based web interface** for real-time predictions



## 🖥️ Web App Interface  

Here’s a screenshot of the web interface where users can input their details and get a predicted Math score:  

 <img width="1470" alt="Screenshot 2025-03-27 at 9 56 10 PM" src="https://github.com/user-attachments/assets/420c253b-48c3-4787-ae67-19c1774c563a" />


```

## 🛠️ How to Run the Project  
### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/your-username/student-exam-performance-predictor.git
cd student-exam-performance-predictor


2️⃣ Create a Virtual Environment & Install Dependencies

pip install -r requirements.txt

3️⃣ Run the Flask App

python app.py
```

The web app will be available at: http://127.0.0.1:5001/predictdata
