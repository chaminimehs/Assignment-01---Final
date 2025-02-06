Supercar Market Demand Prediction

This project analyzes the market demand for elite sports cars in Sri Lanka during the COVID-19 period. It employs machine learning techniques to classify market demand using a dataset of high-performance imported supercars (Horsepower > 900). The project explores different classification models, including Random Forest, XGBoost, and Gradient Boosting, to determine the best-performing model.

Dataset

The dataset used for this project is stored in Elite Sports Cars in Data.csv. It contains information on various attributes of high-end sports cars, including:

          -Condition
          -Fuel Type
          -Drivetrain
          -Transmission
          -Popularity
          -Market Demand (Target Variable)
          -Other numerical and categorical features



Data Preprocessing

   -Irrelevant columns (Brand, Model, Country, Modification, Log_Price, Log_Mileage) are removed.

   -Categorical variables (Condition, Fuel_Type, Drivetrain, Transmission, Popularity, Market_Demand) are label-encoded.

   -Features are standardized using StandardScaler.

   -The dataset is split into 80% training and 20% testing using train_test_split with stratification.

