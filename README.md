# Disease Prediction from Symptoms
![logo](images/dpfs.jpg)
This project concerns the prediction of disease based on symptoms using machine learning. Machine learning algorithms wil be employed on the provided dataset to predict diseases. Its implementation is done through the python programming language. The accuracy of the algorithm is determined by its performance on the given dataset.


## Dataset
The dataset for this problem is downloaded from [here](https://impact.dbmi.columbia.edu/~friedma/Projects/DiseaseSymptomKB/index.html).             
The first column shows the disease, the second column shows the number of discharge summaries that are positive and currently mention the disease, and the associated symptoms.

## Approach
- Data preprocessing` : The data preprocessing tasks performed were as follows:
  * Misspelled names of diseases and symptoms or their codes were corrected.
  * Codes given to diseases or symptoms were removed as they were irrelevant to our task.
  * A cumulative list of all symptoms was created.
  * Each symptom was assigned a boolean value of 0 or 1 for each disease, depending on whether the symptom occurs with that disease or not.
- Model Building` : Two machine learning models were used to train the dataset: *Multinomial Naive Bayes Classifier* and *Decision Tree*.
a problem: when the data is split into the train and test, We have never seen the disease in the test set, so we cannot function on data we have not seen. Also, there is only one score for each disease, so we do not have this score. Therefore, the model must be fully trained.
