# Model Selection: Data Prep

## Process

1. Split the data into training and test set.
2. Train vectorizers on training set and use that to transform test set.
3. It beste random forest model and best gradient boosting model on training set and predict on test set. 
4. Thoroughly evaluate results of these two models to select best model. 


## Two final points
- Further evaluation
  - Solice test set
  - Examine text messages the model is getting wrong
 
- Results trade-off- consider business context 
    - Is predict time of 0.213 vs. 0.135 goinng to create a bottleneck?
    - Precision (False positives) / recall (False negatives). For instance, for spam flilter - optimize for precision, but for antivirus software - optimize for recall
