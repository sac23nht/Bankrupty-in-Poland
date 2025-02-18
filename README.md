# Bankruptcy in Poland
This project aims to explore and analyze data collected by a team of Polish economists studying bankruptcy. The main objective of this project is to build a model that can predict whether a company will go bankrupt or not using machine learning algorithms such as Random Forest and Gradient Boosting. The project also includes an interactive dashboard that shows how company profit and losses change in relationship to the model's probability threshold.

# Data Source
The data used in this project was sourced from [here](https://www.emis.com/). The dataset was compressed into a gzip file and was stored in JSON format. The dataset contains information about various companies in Poland, including their financial information, legal information, and other relevant variables. 


# Data Wrangling
The initial data was in JSON format and compressed, so it was converted to a dictionary after decompression and then turned into a Pandas dataframe. The dataset contained missing data, which were imputed using the median, considering its skewness. The data was also imbalanced, so I used oversampling to balance the dataset. 

# Exploratory Data Analysis (EDA)
 I started by checking the distribution of the target variable, which is the bankruptcy status. I found out that only a few of the companies in the dataset went bankrupt. This means that the dataset was highly imbalanced, and I needed to address this issue before building the models.

I also checked the distribution of the features and found out that most of them were highly skewed. I used binning to normalize the distribution of the features. I also checked for multicollinearity and found that some features were highly correlated. 


# Modeling Approach
I used both Random Forest and Gradient Boosting models to predict bankruptcy. We chose these models because they are powerful machine-learning algorithms that can handle both categorical and continuous data. 


I split this project into three notebooks

* Working with JSON: This notebook shows the decompression and conversion process.
* Random Forest: This notebook shows the modeling and results with Random Forest.
* Gradient Boosting: This notebook shows the modeling and results with gradient boosting.