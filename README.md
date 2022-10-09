# Cervical-Cancer-Prediction-Using-Logistic-Regression-Trees
<img src="https://github.com/Vaibhavnaudiyal92/Cervical-Cancer-Prediction-Using-Logistic-Regression-Trees/blob/main/cancer-cells-image.jpg?raw=true"
     alt="Markdown Monster icon"
     style="float: left; margin-right: 10px;" />
# Introduction
The cervical cancer dataset contains indicators and risk factors for predicting whether a woman will get cervical cancer. The features include demographic data (such as age), lifestyle, and medical history. The data can be downloaded from the UCI Machine Learning repository and is described by Fernandes, Cardoso, and Fernandes (2017)16.

Cervical cancer is a cancer arising from the cervix. It is due to the abnormal growth of cells that have the ability to invade or spread to other parts of the body. Early on, typically no symptoms are seen. Later symptoms may include abnormal vaginal bleeding, pelvic pain or pain during sexual intercourse. While bleeding after sex may not be serious, it may also indicate the presence of cervical cancer.

Human papillomavirus infection (HPV) causes more than 90% of cases; most people who have had HPV infections, however, do not develop cervical cancer. HPV 16 and 18 strains are responsible for nearly 50% of high grade cervical pre-cancers. Other risk factors include smoking, a weak immune system, birth control pills, starting sex at a young age, and having many sexual partners, but these are less important. Genetic factors also contribute to cervical cancer risk. Cervical cancer typically develops from precancerous changes over 10 to 20 years. About 90% of cervical cancer cases are squamous cell carcinomas, 10% are adenocarcinoma, and a small number are other types. Diagnosis is typically by cervical screening followed by a biopsy. Medical imaging is then done to determine whether or not the cancer has spread.(Source: Wikipedia). In our project, we are trying to develop a model which can effectively classify cases of cervical cancer.

# Subset of data features

The subset of data features used are:

1. Age in years
2. Number of sexual partners
3. First sexual intercourse (age in years)
4. Number of pregnancies
5. Smoking (yes or no)
6. Smoking (in years)
7. Hormonal contraceptives (yes or no)
8. Hormonal contraceptives (in years)
9. Intrauterine device yes or no (IUD)
10. Number of years with an intrauterine device (IUD)
11. Has patient ever had a sexually transmitted disease (STD) yes or no
12. Number of STD diagnoses
13. Time since first STD diagnosis
14. Time since last STD diagnosis
15. The biopsy results “Healthy” or “Cancer”. Target outcome.

The biopsy serves as the gold standard for diagnosing cervical cancer. For the examples in this book, the biopsy outcome was used as the target. Missing values for each column were imputed by the mode (most frequent value), which is probably a bad solution, since the true answer could be correlated with the probability that a value is missing. There is probably a bias because the questions are of a very private nature. But this is not a book about missing data imputation, so the mode imputation will have to suffice for the examples.

# Steps performed in this notebook are:
### Exploratory Data Analysis(EDA)
* Finding hidden patterns in the dataset
* Searching for missing values
* Visualising data using graphs 

### Data Pre-Processing
* Removing Outliers
* Filling missing values if found
* Checking for data imbalance and resolving the issue if found

### Model Building and Implementation
Built 3 machine learning models and evaluated their performances
1. Decision Tree CLassifier
2. HDTree Classifier for two atrribute node splitting
3. Logistic Regression Classifier for single node splitting using decision_function

# Conclusion

Successfully implemented the models and predicted whether a given case has positive biopsy result or not
