# Car Price Predictor
---
By: **Siraj Ali**

*Dataset Location*: https://www.kaggle.com/CooperUnion/cardataset

In this repository, I walk through the creation of multiple car price predicting models from scratch.

Pretend that we are a company whose service is to list cars for sale. If we can accurately predict the value of any new or used car based on technical characteristics, market popularity, etc. then we can help inform customers if the vehicles being sold are bargains, are fairly priced, or are just total ripoffs.

The dataset is located at the Kaggle link above. This data includes car prices spanning over several decades, along with technical specifications of the cars' performance, engineering, fuel economy, category, make, model, year, popularity, price, and more.

## Setup

This exercise is broken up into three different Jupyter notebooks. All dependencies are in the `environment.yml` file, which can be used to create a conda environment:

### Prerequisites:
Your machine should have Python 3.8 installed, as well as `git` and either `conda` or `miniconda`.

### Instructions:

1. Clone this repository (assuming you have git installed)  
```$ git clone https://github.com/sirajali/car-price-predictor.git```
2. Create a conda environment  
```$ conda env create -f environment.yml --name kaggle```
3. Activate the conda environment  
```$ conda activate kaggle```
4. Run Jupyter Lab  
```$ jupyter-lab```
5. Download the dataset from the link above and place it in your project space.  

## The Notebooks:

### EDA.ipynb

This notebook contains exploratory data analysis:
* Data preview and characteristics
* Check for nulls
* Check for duplicates
* Check for the distribution of the model target (price)
* Variable correlation
* Data trends over time
* Gather other additional insights that might be useful about the cars, their prices, makes, specifications, etc.

### Feature_Engineering.ipynb

This notebook contains data cleaning and feature engineering, in preparation for model training:
* Dropping duplicates
* Imputation of nulls
* Feature creation from existing variables
* Handling of outliers
* One-hot encoding

### Model_Fit.ipynb

This notebook contains the bulk of the exercise. It's further organized into multiple parts:

1. A stratified train-test split of the data
2. Generalized Linear Regression modelling
  * Model fitting
  * Model evaluation
  * Validating assumptions (or violations of assumptions) of linear regression
3. Gradient Boosted Machine regression moddeling
  * Hyperparameter tuning via gridsearch
  * Model fitting
  * Model evaluation
  * Residual analysis
  * Feature importances
4. Closing remarks and theoretical next steps

---

Thanks for reading!