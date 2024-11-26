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
Feature engineerung

3. ML model development
feature engineering
model selection
model training
model evaluation

4. Deployment

5. Monitoring and continual learning

6. Busness Analysis
