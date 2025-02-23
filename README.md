# Multiple-Disease-Prediction-System


#Overview

#The Multiple Disease Prediction System is a web application developed using Streamlit that enables users to predict the likelihood of having Diabetes, Heart Disease, and Parkinson's Disease using trained machine learning models. The system takes user input, processes the data, and provides predictions based on pre-trained models.

#Features
#Diabetes Prediction: Predicts if a person has diabetes based on medical input parameters.
#Heart Disease Prediction: Determines the likelihood of heart disease using patient-specific parameters.
#Parkinson's Disease Prediction: Identifies Parkinson's disease based on voice and medical parameters.
#User-friendly Interface: Developed using Streamlit for easy and intuitive use.

#**Technologies Used**

#Python
#Streamlit (for web UI)
#Scikit-learn (for ML models)
#Pickle (for saving and loading trained models)

#**Installation & Setup**

#Prerequisites
#Ensure you have the following installed:
#Python 3.7+

#**Required Python libraries:**

#pip install streamlit scikit-learn numpy pandas
#Running the Application
#Clone the repository or download the files.
#Navigate to the project folder in the terminal.

#**Run the following command:**

#streamlit run Multiple_Disease_Prediction.py

#**Project Structure**

#Multiple Disease Prediction System/
#│-- saved_models/
#│   ├── diabetes_model.sav
#│   ├── heart_disease_model.sav
#│   ├── parkinsons_model.sav
#│-- Multiple_Disease_Prediction.py
#│-- README.md

#**How It Works**

#The application loads pre-trained machine learning models from the saved_models directory.
#Users enter their medical details into the respective prediction forms.
#The system processes the inputs and predicts the disease likelihood using the ML models.
#Results are displayed to the user on the web interface.

#**Issues and Fixes**

#Common Error: ValueError: could not convert string to float: ''
#Solution: Ensure all input fields are filled before submitting the form. Modify the code to handle empty values:

#user_input = [float(x) if x.strip() else 0.0 for x in user_input]

