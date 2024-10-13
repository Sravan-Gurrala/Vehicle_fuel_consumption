# **Car Mileage Prediction Using Machine Learning**

## **Overview**
This project aims to predict car mileage (measured in miles per gallon, MPG) based on various characteristics of the vehicle using the **Auto MPG dataset** from the **UCI Machine Learning Repository**. By analyzing the attributes of the cars (e.g., cylinders, displacement, horsepower), we seek to understand what makes a car efficient and optimize target mileage predictions using several regression models.

## **Dataset**
- **Source**: Auto MPG dataset from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/auto+mpg)
- The dataset consists of:
  - 3 multivalued discrete attributes
  - 5 continuous attributes

## **Project Process**

1. **Data Collection and Preprocessing**
   - The **Auto MPG dataset** is imported and cleaned for missing values.
   - Exploratory Data Analysis (EDA) is performed to understand relationships between attributes and target variable (MPG).
   - The data is split into training and testing datasets for model evaluation.

2. **Modeling**
   - We employ various regression algorithms to predict car mileage:
     - **Linear Regression**
     - **Decision Tree Regressor**
     - **Random Forest Regressor**
     - **Support Vector Machine (SVM) Regressor**
   - Each model is trained on the training dataset and evaluated using metrics like **Mean Squared Error (MSE)** and **R² score**.

3. **Model Comparison**
   - All models are compared based on their performance metrics, and the best-performing model is selected.

4. **Deployment**
   - The best-performing model is deployed using a **Flask** web application.
   - The Flask app is hosted on **Heroku** to make the prediction service accessible to users.

## **Tech Stack**
- **Python**: Primary programming language for data manipulation and model development.
- **Jupyter Notebook**: For data analysis, model training, and experimentation.
- **Flask**: To create a web service for predictions.
- **Heroku**: To deploy the web service and make it accessible online.

## **Algorithms Used**
1. **Linear Regression**
2. **Decision Tree Regressor**
3. **Random Forest Regressor**
4. **SVM Regressor**

## **Project Structure**

```
├── app.py                # Flask web service
├── model.pkl             # Serialized trained model
├── static/               # Static files (CSS, JS, etc.)
├── templates/            # HTML templates for the Flask app
├── data/                 # Dataset files (Auto MPG dataset)
├── notebooks/            # Jupyter notebooks for analysis and model training
├── README.md             # Project documentation
└── requirements.txt      # Dependencies required to run the project
```

## **How to Run the Project**

### **Prerequisites**
- **Python 3.x**
- **pip** (Python package manager)

### **1. Clone the repository**

```bash
git clone https://github.com/Sravan-Gurrala/car-mileage-prediction.git
cd car-mileage-prediction
```

### **2. Install required dependencies**

```bash
pip install -r requirements.txt
```

### **3. Run the Jupyter notebook**
You can explore the model training process by opening the notebook in your local environment.

```bash
jupyter notebook notebooks/Car_Mileage_Prediction.ipynb
```

### **4. Running the Flask app locally**

```bash
python app.py
```
Visit `http://localhost:5000` in your browser to access the web interface for predicting car mileage.

### **5. Deploying to Heroku**
If you wish to deploy the Flask app on **Heroku**, follow these steps:

```bash
heroku create
git push heroku master
heroku open
```

## **Future Enhancements**
- Add more advanced models (e.g., **Gradient Boosting** or **Neural Networks**).
- Improve feature engineering and hyperparameter tuning for better prediction accuracy.
- Create a REST API for easier integration with other platforms.


