Desiging Machine Learning Systems by Chip Huyen

Checklist
Ch2
Understand the business objectives
Identify business metrics

Four characteristics ML systems:

- Reliability

- Scalability

- Maintainability

- Adaptability

ML Developement Cycle

1. Project Scoping
2. Data Enineering
3. ML model development
4. Deployment
5. Monitoring and continuoul learning
6. Business Analysis

1. Project Scoping
Is the problem you are trying to solve even a ML problem? Can it be framed as a ML problem?
Identify goals and objectives
Classification or regression?
Identify stakeholders
Estimate Resources

Ch3
2. Data Engineering
Understand the data
  check for skewed distribution
Pick the right data model for you needs. Realtional model, document model, graph database etc...
Decide on structured vs. unstructured data

Ch4
Decide on sampling method
Common choices
non-probabilty sampling - should not use unless you have to, high probability of selection bias
  convience sampling
  snowball sampling
  judgement sampling
  quota sampling

random sampling
  simple random sampling
  stratified random sampling
  weighted sampling
  reservoir sampling
  importance sampling

Labeling methods
  hand labels  
  natural labels
  lack of labels
    weak supervision
    semi-supervision
    transfer learning
    active learning

Class Imbalances
  data-distribution
    evaluate the ROC curve for the positive class
    evaluate the precision-recall curve for the negative class
  data level
    resampling - oversampling, undersampling
  algoritmic level
    tuning the loss function
      cost-sensitive learning
      class-balanced loss
      focal loss

data augmentation
  label-preserving transformations
  data synthesis

Ch5
Feature Engineering
  Handle missing values
  Identify the type of missing values
    missing completely at random MCAR
    missing at random MAR
    missing not at random MNAR
  Dealing with missing values
    remove the rows
    remove the columns
    impute the missing values
      use a default, ex. ""
      use mean, median, mode
  Feature Scaling
    check for skewed distribution
      apply log transformation
    verify did not introduce data leakage by scaling
  Encoding Categorical Features
    check whether categories have changed over time
    check whether categories are added
      if so use the "hashing trick"
  Feature Crossing combine features to create new features
  Data leakage
    check for the following:
      do you understand how the data was generated?
      if the data is time-correlated, was it split by time
      scaling before splitting
      remove duplicates before splitting
      group leakage
    detecting data leakage
      measure the predictive power of each feature against a label
      determine how many features are correlated with the label
        do an ablation study
      if new feature imroves the model then check that there is not data leakage
  Measure feature importance
    SHAP
  Feature Generalization
   Generally want to look at two things
      feature coverage
      distribution of feature values
        is it in both your training and test sets

3. ML model development

Ch6 Model Development and Offline Evaluation

Model Evaluation
  common models for text classification include naive Bayes, logistic regression, recurrent neural networks, and transformer-based models such as BERT, GPT, and their variants.
  fraudulent transactions are abnormalities that you want to detect—and common algorithms for this problem are many, including k-nearest neighbors, isolation forest, clustering, and neural networks.
 it’s important to consider not only the model’s performance, measured by metrics such as accuracy, F1 score, and log loss, but also its other properties, such as how much data, compute, and time it needs to train, what’s its inference latency, and interpretability.

6 tips for model selection

avoid the state-of-the-art trap
start with the simplest model
avoid human biases in selecting models
evaluate good performance now vs good performance later
  use learning curves to evaluate how your model might perform with more data
evaluate trade-offs
4. Deployment

5. Monitoring and continual learning

6. Busness Analysis
