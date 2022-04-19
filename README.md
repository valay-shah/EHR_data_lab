# Machine Learning Models applied to find the drug effectiveness in patients having Rheumatoid Arthritis
There is a vast majority of EHR (Electronic Health Record) data being collected and there is very little use of EHR Data which can be used for finding out patterns
in the data. So even before showing the symtoms, the EHR data can be used to find patterns and provide timely treatment. Autoimmune diseases are one such part where the
data is collected in the form of EHR. In order to bridge the gap between the data and treatment this study applies various Machine Learning (ML) models in order to find
out how patients would react to a particular drug called TNF Inhibitor which is the most important drug used for treating patients having Rheumatoid Arthritis.

### Data
Data is gathered from NYU Langone. The EHR data consists of 296 patients having 101 features. 

### Libraries required
- sklearn == 1.0
- xgboost == 1.4.2
- numpy == 1.22.3
- pandas == 1.3.5
- matplotlib == 3.3.2
- imblearn == 0.8.0
- impyute == 0.0.8

### Code File Description
- Initial_preprocessing.ipynb: This file contains initial preprocessing for the EHR data (removing some unused columns, removing duplicate values etc)
- method-1_classification.ipynb: This file deals with the unknown values by removing the datapoints which has "Unknown" label in the target variable.
- method-2_classification.ipyng: This file deals with the "Unknown" label in the target variable by keeping them as the 4th category.
- method-3_classification.ipynb: This file deals with the "Unknown" label in the target variable by imputing them with the training set while not polluting the test set.
- models_classification.ipynb: This file contains various models for classification task.
- models_for_hyperparameters.ipynb: This file contains different models that I tried in order to find the best hyperparameters for the models. 
