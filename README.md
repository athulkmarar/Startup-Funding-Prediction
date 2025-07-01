# Startup-Funding-Prediction
🚀 Startup Funding Prediction using Machine Learning
🔍 Problem Statement
Can we predict whether a startup will receive funding based on features such as industry, city, sub-sector,investment type, and amount?
📆 Dataset
Source: Indian startup funding dataset (Kaggle)
Size: 2372 rows x 8 features (after cleaning)
Key Features Used: IndustryVertical , SubVertical , CityLocation , InvestmentType ,AmountInUSD,Remarks
Target Variable: Funded (binary: 1 for funded, 0 for not funded)
🚛 Data Cleaning & Preprocessing
Removed irrelevant columns: SNo , StartupName , InvestorsName
Handled missing values in multiple fields ( IndustryVertical , CityLocation , etc.)
Created new target column: Funded
One-hot encoded categorical variables
Ensured correct data types (e.g., parsed date column)
📊 Exploratory Data Analysis (EDA)
Visualized distribution of funding by:
Industry Verticals (e.g., FinTech, Healthcare)
Cities (e.g., Bangalore, Delhi)
Investment Types (Seed, Series A, etc.)
🧠 Feature Engineering
Encoded categorical columns using One-Hot Encoding
Dropped highly sparse or non-useful fields
🤖 Model Building
Models Used:
Logistic Regression (baseline)
Random Forest Classifier (main model)
Train/Test Split: 80/20
📈 Evaluation
Used F1 Score, Confusion Matrix, and Accuracy for evaluation
Final Random Forest Model (after tuning):
F1 Score: ~0.74
Accuracy: ~0.60
⚖️ Hyperparameter Tuning
Tuned n_estimators and max_depth using GridSearchCV
Applied 5-fold cross-validation to avoid overfitting
🔢 Feature Importance
Identified key factors contributing to funding:
IndustryVertical
CityLocation
InvestmentType
📢 Tools & Libraries
Python (Pandas, Numpy, Scikit-learn)
Matplotlib & Seaborn
Google Colab
📚 Future Scope
Add Streamlit app for live predictions
Use more external datasets (e.g., Crunchbase, AngelList)
Explore deep learning methods or NLP on remarks/comments
📋 Author
Athul K. | AI-Enabled Data Analyst | www.linkedin.com/in/athul-ramesan
