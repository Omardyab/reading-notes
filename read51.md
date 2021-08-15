# Reading 16: Data Science Primer

Exploratory analysis, data cleaning, feature engineering, algorithm selection, and model training maes up 80% of data science. 

        Machine Learning ≠ Algorithms

        Machine learning is a comprehensive approach to solving problems. 

        Machine learning is teaching the computer how to learn patterns based on data for making decisions or predictions. 

in the course there are some basic definitions as following :

        Model - a set of patterns learned from data.
        Algorithm - a specific ML process used to train a model.
        Training data - the dataset from which the algorithm learns the model.
        Test data - a new dataset for reliably evaluating model performance.
        Features - Variables (columns) in the dataset used to train the model.
        Target variable - A specific variable you're trying to predict.
        Observations - Data points (rows) in the dataset.

The two most common ML techniques: 

        Supervised Learning: build a predictive model. 

                        Regression:  modeling continuous variables.
                        Classification modeling categorical ( "class") variables.

        and Unsupervised Learning:  automated data analysis or automated signal extraction 

                        Clustering finding groups within your data.



The 3 Elements of Great Machine Learning: 

                        Human role of guidance. 
                        clean data
                        no overfitting


Exploratory Analysis: 

        know your dataset(observations, features), plotting is very importnat in order to understand your dataset. 

Data Cleaning:

         Remove Unwanted observations (Duplicate  or Irrelevant observations) filter Unwanted Outliersand, fixing errors, and handling missing data. 


Feature Engineering: 

        "Applied machine learning’ is basically feature engineering.”
        Creating new input features from your existing ones.
        Infuse Domain Knowledge: isolating based on an indicator.
        the most important question :"could I combine this information in any way that might be even more useful?"
        Add Dummy Variables: 0 or 1 variables represent single class. 
        Remove Unused Features, Redundant features 

Algorithm Selection: 

        Linear regression models overfit with many input features.
        Regularized Regression Algos:Lasso and Ridge Regression,Elastic-Net. 

Decision Tree Algos:

        Dont express non-linear relationships easily. 
        Decision trees model is the solution. 

Tree Ensembles: 

        Bagging and Boosting. 


Model Training: 

                Split the data. 
                Training data and test data. 
                Hyperparameters: tuning models, cant be learned from data and already decided.
                Cross-Validation "reliable estimate of model performance using only your training data."
                Fit and Tune Models.
                Select Winning Model:
                        Regression:MSE
                        Classification:AUROC.












