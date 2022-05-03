# Credit_Risk_Analysis

## Deliverable 4: 

### Overview of the loan prediction risk analysis: 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes. We are going to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

### Results: 

- Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)

#### Oversampling

Compare two oversampling algorithms to determine which algorithm results in the best performance.

##### Naive Random Oversampling: 
- Balanced accuracy is 65% 
<img width="967" alt="Screen Shot 2022-05-03 at 12 45 09 AM" src="https://user-images.githubusercontent.com/93845867/166414126-9638f90d-d3a3-41d2-ad8a-c63e3925c957.png">

##### SMOTE Oversampling
- Balanced accuracy is 66% 
<img width="962" alt="Screen Shot 2022-05-03 at 12 45 28 AM" src="https://user-images.githubusercontent.com/93845867/166414135-dc39f5b5-a2b2-4d3c-ac7a-1988db8115d1.png">

#### Undersampling
- Balanced accuracy is 66% 
<img width="966" alt="Screen Shot 2022-05-03 at 12 45 58 AM" src="https://user-images.githubusercontent.com/93845867/166414139-bb1f9686-e599-4b23-a890-232a4d794c11.png">

#### Combination (Over and Under) Sampling 
- Balanced accuracy is 54% 
<img width="962" alt="Screen Shot 2022-05-03 at 12 46 18 AM" src="https://user-images.githubusercontent.com/93845867/166414144-2ea0d154-aaff-4735-8424-94689729662c.png">

### Ensemble Learners

Compare two ensemble algorithms to determine which algorithm results in the best performance. 

#### Balanced Random Forest Classifier
- Balanced accuracy is 77% 
<img width="963" alt="Screen Shot 2022-05-03 at 12 43 40 AM" src="https://user-images.githubusercontent.com/93845867/166414085-cc8c79a7-d161-4c4f-a5a3-923e99b5e591.png">

#### Easy Ensemble AdaBoost Classifier
- Balanced accuracy is 92% 
<img width="963" alt="Screen Shot 2022-05-03 at 12 44 14 AM" src="https://user-images.githubusercontent.com/93845867/166414110-65612f48-121f-4764-b85f-c935727b8238.png">

### Summary: 

Out of all 6 models, Easy Ensemble AdaBoost Classifier had the best balance of accuracy, precision and recall. I would recommend using it over the other models. 
