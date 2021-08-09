# Reading 12: Panda

Panda :

The article shows that statistical investigation can be easier using Pandas.

Its the excel of Python, using tables (or as known Dataframe) and transform them in other forms 

* a lot of can be done using Pandas such as :

        Selection (Selection by labe or position)
        Getting/Setting

* Opeartions: 

        Stats
        Apply
        Histogramming
        String Methods

* Grouping:
* def :a process involving one or more of the following steps:

        Splitting the data into groups based on some criteria.
        Applying a function to each group independently
        Combining the results into a data structure

* Reshaping.
* Time series
* and a lot more from here : (https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

# How to run Linear regression in Python scikit-Learn: 

Linear regression using numpy, scipy, stats model and sckit learn.

Scikit-learn is very powerful python module 
this is the example the author gave abootu predicting predict the Boston housing prices

        from sklearn.linear_model import LinearRegression
        x=bos.drop('PRICE', axis=1)
        lm=LinearRegression


three main process: 

        lm.fit() -> fits a linear model

        lm.predict() -> Predict Y using the linear model with estimated coefficients

        lm.score() -> Returns the coefficient of determination (R^2).

Residual Plots you can visualize the errors in your data.