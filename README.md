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
- seaborn == 0.11.0

### Code File Description
- Initial_preprocessing_class.ipynb: This file contains initial preprocessing for the classification task of EHR data (removing some unused columns, removing duplicate values etc)
- method_1_classification.ipynb: This file deals with the unknown values by removing the datapoints which has "Unknown" label in the target variable.
- method_2_classification.ipyng: This file deals with the "Unknown" label in the target variable by keeping them as the 4th category.
- method_3_classification.ipynb: This file deals with the "Unknown" label in the target variable by imputing them with the training set while not polluting the test set.
- models_class.ipynb: This file contains all the models for classification task.
- Initial_preprocessing_reg.ipynb: This file contains initial preprocessing for the regression task of EHR data (removing some unused columns, removing duplicate values etc)
- method_1_reg.ipynb: This file deals with the unknown values by removing the datapoints which has "Unknown" label in the target variable.
- method_2_reg.ipynb: This file deals with the null values in the target variable by imputing them with the training set while not polluting the test set.
- models_reg.ipynb: This file contains all the models for regression task.
- autogluon_class.ipynb: This file contains the results of the classification based models produced by the Autogluon library.
- autogluon_reg.ipynb: This file contains the results of the regression based models produced by the Autogluon library.
- models_for_hyperparameters.ipynb: This file contains different models that I tried in order to find the best hyperparameters for the models. 
- two_step_regression.ipynb: This file contains all the preprocessing steps until the regression model prediction and then converting the regression values to classification based labels.
