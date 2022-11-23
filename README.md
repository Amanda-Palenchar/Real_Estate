# Real_Estate

![Logo](Images/Logo.JPG)

### Overview
The goal of this project is to determine if a connection exists between home values and the home proximity to a grocery store, specifically Trader Joe's and Walmart. Proximity to a grocery store, among other features (beds, baths, square footage), is then used to create a Flask App that will predict home prices.

**Essential Question:** What is the correlation between home value and proximity to Trader Joe’s or Walmart?

### Datasets
The real estate dataset that was used for this analysis (over 900,000 lines of data) and the subsequent clean dataset that was created after the ETL process were too large to push to GitHub. However, the initial datasets are available on Kaggle at the following links and running the code in Data_Cleaning folder will yield a clean dataset to use for the machine learning model. 
- [Real Estate Dataset](https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset)
- [Trader Joe's Dataset](https://www.kaggle.com/datasets/saejinmahlauheinert/trader-joes-locations?select=tj-locations.csv)
- [Walmart Dataset](https://www.kaggle.com/code/timmofeyy/walmart-stores-location-eda/data)

### Technologies
- **Extract, Transform, Load:** Jupyter Notebook, Pandas, Numpby, Plotly, Matplotlib, Seaborn
- **Machine Learning:** Jupyter Notebook, Pandas, Sklearn
- **Data Visualization:** Tableau
- **Real Estate Value Aoo:** HTML, JavaScript, Flask, CSS

### Extract, Transform, Load
The following processes are present in the Data_Cleaning folder in order to have data that was usable for visualization, machine learning, and the app.
- Loading the real estate, Trader Joe's, and Walmart data
- Dropping redundant (i.e. retaining address and dropping street), unnecessary (i.e. status), and/or largely blank (i.e. sell data) columns
- Filling NaNs for acre lot with 0 because NaNs indicated apartments
- Filtering location of real estate to the New England region to create some controls for location
- Returning zip codes that started with 0 to five digit zip codes (i.e. returning 1001 to 01001)
- Adding a TJs_store_count and Walmart_store_count column and merging the number of stores in a given piece of real estate's zip code into those columns
- Investigating and removing specific outliers

After these processes our finished dataframe was exported to a CSV file. Below is a sample of the dataframe after the ETL process. 

![Clean_Real_Estate](Images/Clean_Real_Estate.png)

### Data Visualization

### Machine Learning

# Real Estate Value App
