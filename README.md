🧠 Customer Churn Prediction using ANN

This project predicts customer churn (whether a customer is likely to leave) using an Artificial Neural Network (ANN) built with TensorFlow/Keras. The model is integrated into an interactive Streamlit app for real-time predictions.

📂 Project Structure

│
├── app.py                       # Streamlit app for churn prediction  
├── Churn_Modelling.csv          # Dataset used for training/testing  
├── model.h5                     # Trained ANN model  
├── onehot_encoder_geo.pkl       # Geography encoder  
├── label_encoder_gender.pkl     # Gender encoder  
├── scaler.pkl                   # Scaler for input normalization  
├── requirements.txt             # Dependencies  
├── experiments.ipynb            # Model training & experiments  
├── prediction.ipynb             # Prediction experiments  


🚀 Features

ANN model trained to predict customer churn

Encodes categorical features (Geography, Gender)

Scales numerical features for model input

Interactive Streamlit UI for predictions

Outputs churn probability and interprets likelihood

⚙️ Installation

Clone this repository:

git clone https://github.com/your-username/ANN_PROJ1.git
cd ANN_PROJ1


Create and activate a virtual environment (recommended):

conda create -n churn_env python=3.11 -y
conda activate churn_env


Install dependencies:

pip install -r requirements.txt

▶️ Usage

Run the Streamlit app:

streamlit run app.py


The app will open in your browser (default: http://localhost:8501).

📊 Input Features

The model expects the following inputs:

Geography (France, Spain, Germany)

Gender (Male, Female)

Age

Tenure

Balance

NumOfProducts

HasCrCard (0 = No, 1 = Yes)

IsActiveMember (0 = No, 1 = Yes)

EstimatedSalary

🧮 Output

Churn Probability (0 to 1)

Prediction Message:

Customer is likely to churn if probability > 0.5

Customer is not likely to churn otherwise

📈 Model Training

Model trained on Churn_Modelling.csv dataset

Preprocessing:

One-hot encoding (Geography)

Label encoding (Gender)

Feature scaling

Architecture: ANN (Keras Sequential)

Optimizer: Adam

Loss: Binary Crossentropy

Metrics: Accuracy

🛠 Requirements

Main dependencies (see requirements.txt):

Python 3.11

TensorFlow

Streamlit

Pandas, NumPy, Scikit-learn

Joblib (for loading encoders & scaler)

📌 Future Improvements

Add SHAP/LIME explainability

Deploy to cloud (Heroku / AWS / Azure)

Extend to multi-class classification

👨‍💻 Author

Rahul Singh
