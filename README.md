# A Statistical Analysis of Descriptions to Determine Severity of the Vulnerabilities

For a thoroughly research paper on this analyis please visit the "Cybersecurity Analysis: A Statistical Analysis of Descriptions to Determine Severity of the Vulnerabilities.pdf" paper in this repository.


# Overview

This repository contains the code and findings from my dissertation on cybersecurity vulnerability analysis. The study utilizes data from the National Vulnerabilities Database (NVD) to analyze cybersecurity threats, trends, and risk factors using machine learning and statistical methods.

# Data

- The dataset consists of JSON files downloaded from the National Vulnerabilities Database (NVD).
- These files contain structured data on cybersecurity vulnerabilities and contains variables like *"CVE-ID", "CVE-Problemtype", "DatePublished", "Date-
Modified"*, etc, but for the purpose of this analysis I only used the variables *"CVE-ID", "Description", "Base_Severity_V3" and "Published_Date"*.

# Objective

The primary objective of this research is the predict the severity of a vulnerability based on the description. This can be achieved using machine learning and deep learning techniques along with natural language processing techniques. Additionally, using deep deep learning techniques along with natural language processing techniques will also allow the generation of keyword for the predicted severity, thus highlighting the nature of the vulnerability.

# Methodology 

- **Data Preprocessing**: Cleaning and structuring JSON data into a machine-readable format.
- **Exploratory Data Analysis (EDA)**: Identifying patterns and trends in vulnerability occurrences.
- **Machine Learning Models**: Classification models, namely Multinomial Logistic Regression (Lasso Regression, Ridge Regression and Elastic Net), Decision Tree, Random Forest and Support Vector Machines along with Long Short-Term Memory a type of Recurrent Neural Network, are used predict vulnerability severity.
- **Natural Language Processing (NLP) Techniques**: Topic Modelling technique Latent Dirichlet Allocation (LDA) is to analyze textual descriptions of vulnerabilities and generate keywords for predicted severities.

# Limitations

- This study was limited by the available computational power, which has an impact on the optimization of hyperparameters and the overall performance of the models. Due to this restraint, an extensive search for the hyperparameters was not feasible which affects the general predictive power of the models.
- While LDA adds a layer of interpretability, models like LSTM and Random Forest and Support Vector Machines, are generally considered “black box” models. This poses a challenge to the interpretability of the results.
- A significant limitation of the study was the imbalance of the classes present in the database used for training and testing. This imbalance introduced bias in the model, making it more sensitive to the majority class and less sensitive to the other classes.


# Key Findings

This project explores various machine learning models for cybersecurity vulnerability classification. While the models effectively predict vulnerability severity and generate relevant keywords, their overall accuracy remains limited due to several constraints. Despite hyperparameter tuning and different approaches, the models do not achieve high accuracy. However, they still provide valuable insights by identifying key terms associated with different severity levels, which can help in understanding vulnerability patterns.

# Future Work

To improve model performance, future iterations of this project would focus on optimizing the models with better hardware, allowing for more extensive hyperparameter tuning and deeper architectures. Additionally, incorporating a larger dataset spanning more than four years could enhance predictive capabilities and provide a more comprehensive view of cybersecurity trends.

This project is for academic and research purposes. Please cite appropriately if used in your work.






