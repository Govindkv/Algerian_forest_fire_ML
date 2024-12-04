# Algerian_forest_fire_ML
This project contains the analysis and prdictive model that will figure out on the basis of given data that, is there any probabilty for fire or not.

<div id="top"></div>

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/Govindkv">
    <img src="https://img.icons8.com/external-flat-wichaiwi/64/undefined/external-bush-fire-climate-change-flat-wichaiwi.png" alt="Logo" width="80" height="80"/> 
  </a>

<h3 align="center">Algerian Forest Fire Predictor</h3>

  <p align="center">
    Machine Learning Project
    <br />
    <a href="https://github.com/Govindkv/Algerian_fores_fire_ML"><strong>Explore the Repo »</strong></a>
    <br />
    <br />
    <a href="https://github.com/Govindkv/Algerian_fores_fire_ML/blob/main/application.py">View Flask app code</a>
    ·
    <a href="https://github.com/Govindkv/Algerian_forest_fire_ML/blob/main/notebooks/Algerian_Frorest_Fire_dataset_EDA.ipynb"> Model Building</a>
    ·
    <a href="https://github.com/Govindkv/Algerian_forest_fire_ML/blob/main/notebooks/Algerian_Frorest_Fire_dataset_EDA.ipynb">EDA on Forest Fires dataset</a>
  </p>
</div>


<!-- ABOUT THE PROJECT -->
## About The Project
* Using Data Science and Machine learning, we can build a model that takes in the detected fires dataset learns and detects future fires based on certain Weather report.
* Storing the Sourced dataset to local.
* Building a **Flask App** hosted on **Aws**.
* **Sklearn** for pre-processing and Model Building
* Pandas, Numpy, Matplotlib for csv reading, Data Processing, Data Cleaning, Visualization etc.

<!-- GETTING STARTED -->
## Introduction
*  I used a dataset on **Algerian Forest Fires from UCI**. The dataset contains a culmination of forest fire observations and data in two regions of Algeria: the Bejaia region and the Sidi Bel-Abbes region. 
* The timeline of this dataset is from June 2012 to September 2012. In this project, we focused on whether certain weather features could predict forest fires in these regions using few Machine Learning algorithms. 

<!-- USAGE EXAMPLES -->
## Steps

* Installing Python, Vs code, Git to Computer.
* Creating Flask app by importing `Flask` module.
* Download the source dataset from [UCI Repository](https://archive.ics.uci.edu/ml/datasets/Algerian+Forest+Fires+Dataset++#).
* For Classification algorithm decided to predict the features `Classes` from the dataset which is Binary classification `(fire, not fire)`.
* For Regression Problem algorithm decided to predict the feature `FWI` (Fire weather Index) which is 90%+ correlated to Classes Feature.

### Loading CSV and Inserting to DB
* The Downloaded CSV file is loaded as pandas Dataframe using Pandas Library.
* Pandas Dataframe is converted to Dict .

<p align="right">(<a href="#top">back to top</a>)</p> 

### EDA
* In this step, we will apply Exploratory Data Analysis (EDA) to extract insights from the data set to know which features have contributed more in predicting Forest fire by performing Data Analysis using Pandas and Data visualization using Matplotlib & Seaborn. 
* It is always a good practice to understand the data first and try to gather as many insights from it.

### Model Building 
* For Regression Problem algorithm decided to predict the feature `FWI` (Fire weather Index) which is 90%+ correlated to Classes Feature.
* Models used : **Linear regression, Lasso Regression, Ridge Regression.**
* For Classification algorithm decided to predict the features `Classes` from the dataset which is Binary classification `(fire, not fire)`.
* Models could be used : **Logistic Regression, Decision Tree, Random Forest, XGboost, K-Nearest Neighbour.**

### Model Selection
* HyperParameter Tuning Randomized Gridsearch CV is done for top 2 models for both Regression and Classification.
* For Classification `Stratified Kfold Cross-Validation metrics` is used based best Mean CV Accuracy Model is used for Model Deployment.
* For Regression `R2 score metrics` is used to select best model The R2 score is one of the performance evaluation measures for regression-based machine learning models.

### Flask
* Importing the Flask module and creating a Flask web server from the Flask module.
* Create an object **application** in flask class with `__name__` which represents current application.py file.
* Create `/` route to render default page html.
* `/predictdata` route for api testing using `chrome`
* Create a route `/predictdata` `/` to get user input for Classification and Regression respectively. 
* Run the flask app with `app.run()` code.

### AWS Deployment
* Create new repo in Github and push all the data using `Git`.
* Using github action deployed over AWS cloud.

<p align="right">(<a href="#top">back to top</a>)</p>

### **Technologies used**
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)


### **Tools used**
![PyCharm](https://img.shields.io/badge/pycharm-143?style=for-the-badge&logo=pycharm&logoColor=black&color=black&labelColor=green)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
[![Tools used | Postman](https://img.shields.io/badge/Postman-eeeeee?style=for-the-badge&logo=postman&logoColor=FF6C37&labelColor=fefefe)][postman]



<!-- CONTACT -->
## Contact
[![Govind Kumar | LinkedIn](https://img.shields.io/badge/Govind_Kumar-eeeeee?style=for-the-badge&logo=linkedin&logoColor=ffffff&labelColor=0A66C2)][reach_linkedin]
[![Govind Kumar | G Mail](https://img.shields.io/badge/Govind26663355-eeeeee?style=for-the-badge&logo=gmail&logoColor=ffffff&labelColor=EA4335)][reach_gmail]


<p align="right">(<a href="#top">back to top</a>)</p>


<!-- MARKDOWN LINKS  -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[linkedin-url]: https://linkedin.com/in/govind-kv

<!-- Tools Used -->
[PyCharm]: https://code.visualstudio.com/
[postman]: https://www.postman.com/
[git]: https://git-scm.com/
[github]: https://github.com/
[microsoft_azure]: https://azure.microsoft.com/en-in/features/azure-portal/
[python]: https://www.python.org/
[flask]: https://flask.palletsprojects.com/en/2.1.x/
[sklearn]: https://scikit-learn.org/stable/

<!--contact-->
[reach_linkedin]: https://www.linkedin.com/in/Govind-kv/
[reach_gmail]: mailto:Govind26663355@gmail.com?subject=Github
[Portfolio]: https://govindkv.github.io/

