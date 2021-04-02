# 2338-Machine-Learning-Final-Project-
Predicting Pancreatic Cancer Using Urinary Biomarkers

Problem: 
Pancreatic ductal adenocarcinoma (PDAC) is predicted to be one of the leading causes of cancer mortality in the United States, with a lower than 5% 5-year survival rate. Therefore, using non-invasive screening to predict PDAC in its early stage is urgently needed for improving the survival rate. In this project, we will seek to predict PDAC with four urine biomarkers (creatinine, LYVE1, REG1B and TFF1), and further explore the variation of these biomarkers and their performance in determining which biomarkers show promise in detecting PDAC. 

Data description:
The current study will use the open-access data from a study published in December 2020 [1]. The data collected and organized by the study contained 590 urine specimen samples obtained from multiple centers in different countries. Among the 590 individuals, 183 were in the control group, who had no known history of any pancreatic conditions or renal diseases, 208 were in the benign group, with benign hepatobiliary disease (of which 119 were chronic pancreatitis), and 199 were in the PDAC group (102 in stage I–II of PDAC and 97 in stage III–IV). 50.7% of the whole sample were female individuals. 

Proposed approach and methods:
For statistical analyses, this study will conduct univariate analysis for a general understanding of data distribution. We will build prediction models by using Logistic Regression, Linear Discriminant Analysis (LDA) and Quadratic Discriminant Analysis (QDA), and determine which one is the best fit for this study. The datasets included 590 participants and the biomarkers panels were evaluated in each participant’s urine specimen [1]. We will randomly split data by sample-id and make 80% as a training set and 20% as a testing set. The performance is characterized by the area under the ROC curves(AUC). 

Evaluation plan:
The diagnosis of PAAD has three categories: No pancreatic disease, benign hepatobiliary disease and PDAC. The main predictors are four urine biomarkers, sex and age. We will make two combinations of the diagnosis: No pancreatic disease versus pancreatic cancer and benign hepatobiliary disease versus pancreatic cancer. Both no disease and benign disease will compare with pancreatic cancer I-IV stages. Each case has a binary outcome. We will compare the AUC with 95% CI between each category of the outcome in these two groups.  

