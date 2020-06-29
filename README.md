# Analysis-of-US-Census-Income-Dataset
## Comparison and Integration of Classification Models
<h2 align="left"><font size="3">Abstract</font></h2>

In this project we compare the performance(efficiency) of five classification techniques namely:
- K Nearest Neighbor(KNN)
- Decision Tree
- Support Vector Machine
- Logistic Regression

In predicting .............
whether a person makes over 50K or below 50K a year. We then investigate the performance(efficiency) of integrated models developed through using the algorithms listed above. This data set contains weighted census data extracted from the 1994 and 1995 current population surveys conducted by the .[U.S. Census Bureau](http://www.census.gov/)
The data contains 41 demographic and employment related variables. 

One instance per line with comma delimited fields. There are **299285** instances in total [datasets](https://archive.ics.uci.edu/ml/machine-learning-databases/census-income-mld/census.tar.gz) of which there are **199523** instances in the [data/train](https://archive.ics.uci.edu/ml/machine-learning-databases/census-income-mld/census-income.data.gz) file and **99762** in the [test file](https://archive.ics.uci.edu/ml/machine-learning-databases/census-income-mld/census-income.test.gz). 

The models are evaluated both in terms of their prediction accuracy, as well as with ROC analysis. The Jaccard index, log loss and F1-score for each algorithm was then calculated. Since the data set was very skew/ imbalanced we also performed Precision - recall curve analysis.

## Dataset

#### [Census-Income (KDD) Data Set](https://archive.ics.uci.edu/ml/datasets/Census-Income+%28KDD%29)

This data set contains weighted census data extracted from the 1994 and 1995 current population surveys conducted by the .[U.S. Census Bureau](http://www.census.gov/)
The data contains 41 demographic and employment related variables. 

One instance per line with comma delimited fields. There are **299285** instances in total [datasets](https://archive.ics.uci.edu/ml/machine-learning-databases/census-income-mld/census.tar.gz) of which there are **199523** instances in the [data/train](https://archive.ics.uci.edu/ml/machine-learning-databases/census-income-mld/census-income.data.gz) file and **99762** in the [test file](https://archive.ics.uci.edu/ml/machine-learning-databases/census-income-mld/census-income.test.gz). 

The data was split into train/test in approximately **2/3, 1/3** proportions using MineSet's MIndUtil mineset-to-mlc. 

It includes following fields:

| Field                                      | Description | Field                                      | Description |
|--------------------------------------------|-------------|--------------------------------------------|-------------|
|age						                 | AAGE        |detailed household and family stat	        | HHDFMX      |
|class of worker					         | ACLSWKR     |detailed household summary in household     | HHDREL      |
|industry code					             | ADTIND      |instance weight					            | MARSUPWT    |
|occupation code					         | ADTOCC      |migration code-change in msa			    | MIGMTR1     |
|adjusted gross income				         | AGI         |migration code-change in reg			    | MIGMTR3     |
|education					                 | AHGA        |migration code-move within reg			    | MIGMTR4     |
|wage per hour					             | AHRSPAY     |live in this house 1 year ago			    | MIGSAME     |
|enrolled in edu inst last wk		         | AHSCOL      |migration prev res in sunbelt			    | MIGSUN      |
|marital status					             | AMARITL     |num persons worked for employer		        | NOEMP       |
|major industry code				         | AMJIND      |family members under 18				        | PARENT      |
|major occupation code				         | AMJOCC      |total person earnings				        | PEARNVAL    |
|race						                 | ARACE       |country of birth father				        | PEFNTVTY    |
|hispanic Origin					         | AREORGN     |country of birth mother				        | PEMNTVTY    |
|sex						                 | ASEX        |country of birth self				        | PENATVTY    |
|member of a labor union			         | AUNMEM      |citizenship					                | PRCITSHP    |
|reason for unemployment			         | AUNTYPE     |reason for unemployment			            | AUNTYPE     |
|full or part time employment stat	         | AWKSTAT     |own business or self employed			    | SEOTR       |
|capital gains					             | CAPGAIN     |taxable income amount				        | TAXINC      |
|capital losses					             | CAPLOSS     |fill inc questionnaire for veteran's admin  | VETQVA      |
|divdends from stocks				         | DIVVAL      |veterans benefits				            |VETYN        |
|federal income tax liability		         | FEDTAX      |weeks worked in year				        |WKSWORK      |
|tax filer status				             | FILESTAT    |state of previous residence		            | GRINST      |
|region of previous residence		         | GRINREG     |


## Machine Learning Models Considered

- K Nearest Neighbor(KNN)
- Decision Tree
- Support Vector Machine
- Logistic Regression


<h1> Observations and To-Dos </h1>

- Because of the size of the data, perform the hyper-parameter tuning took forever to complete.
- We could also perform more classification analysis using integrated methods such as: 
    - Bagging algorithms:
        - Random Forest
    - Boosting algorithms:
        - AdaBoost
        - Gradient Boosting Machine (GBM)
        - XGBoost
        - Light GBM
    - Neural Networks Classifier
    - Naive Bayes Classifier
    
To further improve on the performance of the evaluation

# File Structure
README.md
 Data/
    adult.data
    adult.test
    adult.names
 Code/
    check the attached notebook
