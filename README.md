# Startup-Funding-Prediction<br>
🚀 Startup Funding Prediction using Machine Learning<br>
🔍 Problem Statement<br>
Can we predict whether a startup will receive funding based on features such as industry, city, sub-sector,investment type, and amount?<br>
📆 Dataset<br>
Source: Indian startup funding dataset (Kaggle)<br>
Size: 2372 rows x 8 features (after cleaning)<br>
Key Features Used: IndustryVertical , SubVertical , CityLocation , InvestmentType ,AmountInUSD,Remarks<br>
Target Variable: Funded (binary: 1 for funded, 0 for not funded)<br>
🚛 Data Cleaning & Preprocessing<br>
Removed irrelevant columns: SNo , StartupName , InvestorsName<br>
Handled missing values in multiple fields ( IndustryVertical , CityLocation , etc.)<br>
Created new target column: Funded<br>
One-hot encoded categorical variables<br>
Ensured correct data types (e.g., parsed date column)<br>
📊 Exploratory Data Analysis (EDA)<br>
Visualized distribution of funding by:<br>
Industry Verticals (e.g., FinTech, Healthcare)<br>
Cities (e.g., Bangalore, Delhi)<br>
Investment Types (Seed, Series A, etc.)<br>
🧠 Feature Engineering<br>
Encoded categorical columns using One-Hot Encoding<br>
Dropped highly sparse or non-useful fields<br>
🤖 Model Building<br>
Models Used:<br>
Logistic Regression (baseline)<br>
Random Forest Classifier (main model)<br>
Train/Test Split: 80/20<br>
📈 Evaluation<br>
Used F1 Score, Confusion Matrix, and Accuracy for evaluation<br>
Final Random Forest Model (after tuning):<br>
F1 Score: ~0.74<br>
Accuracy: ~0.60<br>
⚖️ Hyperparameter Tuning<br>
Tuned n_estimators and max_depth using GridSearchCV<br>
Applied 5-fold cross-validation to avoid overfitting<br>
🔢 Feature Importance<br>
Identified key factors contributing to funding:<br>
IndustryVertical<br>
CityLocation<br>
InvestmentType<br>
📢 Tools & Libraries<br>
Python (Pandas, Numpy, Scikit-learn)<br>
Matplotlib & Seaborn<br>
Google Colab<br>
📚 Future Scope<br>
Add Streamlit app for live predictions<br>
Use more external datasets (e.g., Crunchbase, AngelList)<br>
Explore deep learning methods or NLP on remarks/comments<br>
📋 Author<br>
Athul K. | AI-Enabled Data Analyst | www.linkedin.com/in/athul-ramesan<br>
