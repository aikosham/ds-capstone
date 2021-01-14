# Starbucks Capstone Project
Medium Post: https://aikosham.medium.com/cappucino-tall-or-medium-analyzing-starbucks-dataset-24529af3e456

A company the size of Starbucks, with millions of daily customers, has loads of data that they can use to drive customer satisfaction and provide the service that they are looking for.

In the capstone project, we were provided with anonymized usage data from a campaign with three types of offers:
- BOGO: Buy one get one free
- Discount
- Info: Information campaign

We try to answer the following questions:
- What are the main drivers of an effective offer?
- Can we categorize whether a user will take up the offer?
- Get an idea of the demographics, income etc. of our customers during data exploration.

According to the documentation of the datasets, we divide the customers into 4 types (details in notebook).
- Type-1 customers complete the transactions when they get the offer
- Type-2 customers view the offer but don't complete it
- Type-3 customers have completed the ofer but may have seen the offer later
- Type-4 customers have not completed the offer yet (and it hasn't expired)

## Files
- `Starbucks_Capstone_notebook.ipynb` contains my solution. It is also interspersed with markdown documentation to explain my steps.
- `requirements.txt` contains the exact environment that was used during development (on python 3.8.2)
- `./data` contains the data files. 
  - `transcript.json` could not be uploaded due to Github data limits, so I uploaded a compressed version of it. 

### Libraries
The major libraries used are:
```
pandas
numpy
math
json
sklearn (various libraries, see notebook)
seaborn
matplotlib.pyplot 
time
```

## Summary
The project was very challenging. First of all, coming up with a structured approach proved to be more than I could handle but many people in the community helped.

The biggest driver of an affective offer turned out to be: income and membership tenure, which is not surprising since long-time members are the most loyal usually. Some interesting factors of the gender diversity are also presented in the notebook.

We built various ML models to predict user behavior. For BOGO and Discount, we were able to get accuracy above 80% but Information model accuracy could not be improved significantly. We discuss this in the playbook. We define "accuracy" as the Classification Accuracy returned by the classifier.


## Acknowlegements
I found these resources very useful:

- [Random forest algorithm](https://towardsdatascience.com/the-random-forest-algorithm-d457d499ffcd)  
- [Using categorical data with one hot encoding](https://www.kaggle.com/dansbecker/using-categorical-data-with-one-hot-encoding)  
- [Is there a rule-of-thumb for how to divide a dataset into training and validation sets?](https://stackoverflow.com/questions/13610074/is-there-a-rule-of-thumb-for-how-to-divide-a-dataset-into-training-and-validatio)  
- [The use of feature scaling in scikit-learn](https://stackoverflow.com/questions/51660001/the-use-of-feature-scaling-in-scikit-learn)  
- [Hyperparameter tuning the random forest in Python using scikit-learn](https://towardsdatascience.com/hyperparameter-tuning-the-random-forest-in-python-using-scikit-learn-28d2aa77dd74)  
- [Random forest feature importances](https://towardsdatascience.com/running-random-forests-inspect-the-feature-importances-with-this-code-2b00dd72b92e)  
- [Rotate axis text in Python matplotlib](https://stackoverflow.com/questions/10998621/rotate-axis-text-in-python-matplotlib)
- [datetime strptime in Python](https://stackoverflow.com/questions/44596077/datetime-strptime-in-python)  
- [Seaborn bar plots](https://seaborn.pydata.org/generated/seaborn.barplot.html)
- [Pandas and Datetime](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.to_datetime.html)
- I would also like to acknowledge everyone who did this challenge previously.
