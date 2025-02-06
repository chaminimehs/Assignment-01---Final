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

   
Machine Learning Models

-The following models are implemented and evaluated:

1. Random Forest Classifier

    -Hyperparameter tuning is performed using GridSearchCV.

    -The best model is selected based on cross-validation performance.

2. XGBoost Classifier

    -The model is trained using the multi:softmax objective for multi-class classification.

   -The evaluation metric used is mlogloss.

3. Gradient Boosting Classifier

   -The model is trained with default hyperparameters and evaluated.

   
Model Evaluation

        -Accuracy scores are calculated for all models.
  
        -Classification reports provide precision, recall, and F1-score metrics.
  
        -Confusion matrices visualize the performance of each model.

  
Results

The script prints:

     -Best hyperparameters for the Random Forest model.

     -Accuracy and classification reports for each model.

     -A visual representation of confusion matrices using seaborn.

     

Installation and Dependencies

To run the script, install the required Python libraries:

           -pip install pandas numpy scikit-learn matplotlib seaborn xgboost

How to Run  

1. Place Elite Sports Cars in Data.csv in the project directory.
2. Run the script:               -python script.py
3. The script will output the results and display confusion matrix visualizations.




Future Improvements

    --Feature engineering to improve model performance.

    --Hyperparameter tuning for XGBoost and Gradient Boosting.

    --Adding more data points for improved generalization.

    --Exploring deep learning models for better accuracy.
