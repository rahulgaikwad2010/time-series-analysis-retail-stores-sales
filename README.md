# Time Series Analysis Retail Stores Sales

<br/>
<br/>

# Table Of Contents
-  [Business Context](#business-context)
-  [Problem Statement](#problem-statement)
-  [Desired Outcome](#desired-outcome)
-  [Version](#version)
-  [Author](#author)
-  [References](#references)

<br/>
<br/>

### Project Structure Overview
```
├──  TextClassifier
│    │
│    ├── common_operations          - this package contains common operation tasks.
│    │    ├── __init__.py
│    │    └── common_operations.py  - this file reads config and convert to dictionary.
│    │
│    ├── data                       - this folder contains data for testing.
│    │    ├── Contraction.json      - file for text preprocessing.
│    │    └── TouchnoteReveiws.csv  - Sample reviews of touch note app.
│    │
│    └── logger                     - here's the logger package.
│    │    ├── __init__.py
│    │    ├── APILogger.py          - to send non-success code to front-end.
│    │    ├── logger.py             - to log info & error in the code.
│    │    └── LoggerError.py        - to log error while creating a logger object.
│    │
│    └── ModelPredictor             - this package is used to get prediction.
│    │    ├── __init__.py
│    │    └── ModelPredictor.py     - this code reads input and return prediction.
│    │
│    └── models                     - this folder contains exported models.
│    │    ├── model_mapping.json    - to store model metadata. ex. Path.
│    │    ├── log_reg.sav
│    │    ├── naive_bayes.sav
│    │    └── svm.sav
│    │
│    └── TextPreprocessor           - here's the package used to clean the raw input.
│    │    ├── __init__.py
│    │    └── TextPreprocessor.py   - this code takes raw text and return clean string for prediction.
│    │
│    └── TextClassifier.py          - driver code to execute operations smoothly.
│
│
├──  Touch Note App Review Analysis                        - this folder contains model training related data, models & notebook.
|    |
│    └── models                                            - this folder holds exported models.
│    │    ├── log_reg.sav                                  - Logistic Regression Model.
│    │    ├── naive_bayes.sav                              - Naive Bayes Model
│    │    └── svm.sav                                      - SVM Model.
│    │
│    └── data                                              - this folder contains data used for model training.
│    │    ├── Contraction.json                             - here's the file for text preprocessing.
│    │    └── google_play_store_apps_reviews_training.csv  - Training Dataset.
|    |
│    ├── Touch Note App Review Analysis.ipynb              - Data Analysis & Model Training Notebook.
│    └── Touch Note App Review Analysis.html               - Exported version in HTML.
|
│
├──  static                  - this folder contains bootstrap 4 files.
│    └── asset
│    └── img
│    └── js
│    └── style
│    └── index.js            - here's the file for frond-end form submission to flask app and vice versa.
│
│
├── templates                - this folder contains front-end html files.
│   └── index.html
│
│
├── kubernetes                - this folder contains yaml file for deployment.
│   └── deployment.yaml       - Kubernetes YAML file
│
│
├── Dockerfile               - here's the docker file used to create docker image.
├── README.md                - here's the ReadMe of an application.
├── config.ini               - here's the specific config file for the application.
├── requirements.txt         - here's the python package requirement txt.
└── run.py                   - here's runnable of an application.
```

<br/>
<br/>

### Business Context:

A large grocery retailer (Shop@ABC) operates multiple stores in the US. 

Demand planning for the stores is a crucial element to ensure the stores are not overstocked or under-stocked, thus enabling a competitive edge in the market. However, the business currently believe that they are not able to leverage the power of data driven analytics solution for the same. 

<hr/>

### Problem Statement

The store managers needs to be empowered with data analytics solutions/ tools, which enables them to predict daily sales for up to a month in advance.

Note that the store sales are impacted by many factors, including various types of promotions, holiday seasons, and various store demographics, among others. 

They would like to understand various factors that affects the demand of the stores and also develop accurate demand forecasting models for the stores

<hr/>

### Desired Outcome:

Using the attached sample data, please come up with your analytics approach:

- Understanding of the different data fields
- Data cleaning/ manipulations and business/ technical logics involved
- Analytical findings and insights (EDA)
- Forecast model development and performance measures
- How would you measure the improvement driven by the solution provided?
- Suggested Next steps

<br/>
<br/>

## Version

1.0.0 

<br/>

## Author

* **Rahul Gaikwad** - Initial work and development

<br/>

## References

* [Rossmann_TSA_forecasts](https://github.com/datageekette/rossmann_TSA_forecasts)
