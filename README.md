# Wine-Quality-Classification-using-ML
his project applies Machine Learning techniques to classify wine quality based on 10 chemical and physical attributes such as alcohol content, acidity, and pH levels.

## File structure 
* `wine_quality.ipynb` -> File classifies the wine in a quality from 1 to 10
* `wine_quality_binary_classification.ipynb` -> File classifies the wine  as good or bad
* `winequality-red.csv` -> File containing red wine data
* `winequality-white.csv` -> File containing white wine data 
* `data_set_info.txt` 
* `old_version.ipynb` -> an old version of the project

## Clasification of wine quality 

For the file `wine_quality.ipynb`
* I have processed the data using pandas and have tried getting upsampled, undersampled , original and SMOTE processed data. 
* Next I have used this data to train XGBoost and Random Forest classifier models
* **due to the unbalanced nature of the data the result was not satisfactory**

So I had to move to binary classification in `wine_quality_binary_classification.ipynb`
* In the file I had to balance the data set using undersampling techniques before it could be processed
* After this ANN , XGBoost and Random forest classifiers were trained on the data
* Confusion matrix and Cross Vaildation was run to get the following best result
* **Achieved 79% accuracy and 0.78 F1-score using XGBoost**