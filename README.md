# Starbucks Capstone Project
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

We built various ML models to predict user behavior. For BOGO and Discount, we were able to get accuracy above 80% but Information model accuracy could not be improved significantly. We discuss this in the playbook.
