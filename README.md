# Machine Learning Homework - Exoplanet Exploration

![exoplanets.jpg](Images/exoplanets.jpg)

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, you will create machine learning models capable of classifying candidate exoplanets from the raw dataset.

- - -

## Instructions

### Preprocess the Data

* Preprocess the dataset prior to fitting the model.
* Perform feature selection and remove unnecessary features.
* Use `MinMaxScaler` to scale the numerical data.
* Separate the data into training and testing data.

### Tune Model Parameters

* Use `GridSearch` to tune model parameters.
* Tune and compare different classifiers.

- - -


# Conclusion

### After comparing all the models, it looks like Random Forest Classifier gives the best Accuracy Score.

### SVM without Gridsearch

* Accuracy = 0.6922196796338673
* Training Data Score: 0.8081251192065612
* Testing Data Score: 0.8117848970251716

                 precision    recall  f1-score   support

     CANDIDATE       0.87      0.45      0.60       818
     CONFIRMED       0.00      0.00      0.00         0
    FALSE POSITIVE   0.96      0.90      0.93       930

      accuracy                           0.69      1748
     macro avg       0.61      0.45      0.51      1748
    weighted avg     0.92      0.69      0.77      1748


### SVM with Gridsearch

* Accuracy = 0.41418764302059496
* Training Data Score: 0.8165172611100515
* Testing Data Score: 0.8232265446224256

                precision    recall  f1-score   support

     CANDIDATE       0.26      0.25      0.26       444
     CONFIRMED       0.00      0.00      0.00         0
    FALSE POSITIVE   0.70      0.47      0.56      1304

      accuracy                           0.41      1748
     macro avg       0.32      0.24      0.27      1748
     weighted avg    0.59      0.41      0.48      1748


### Decision Tree 

* Accuracy = 0.8678489702517163
* Training Data Score: 0.751096700362388
* Testing Data Score: 0.7522883295194508

                precision    recall  f1-score   support

     CANDIDATE       0.74      0.75      0.74       417
     CONFIRMED       0.77      0.75      0.76       462
    FALSE POSITIVE   0.98      0.99      0.98       869

      accuracy                           0.87      1748
     macro avg       0.83      0.83      0.83      1748
    weighted avg     0.87      0.87      0.87      1748


### Random Forest without Gridsearch

* Accuracy = 0.9084668192219679
* Training Data Score: 0.737745565515926
* Testing Data Score: 0.7408466819221968

                precision    recall  f1-score   support

     CANDIDATE       0.79      0.85      0.82       393
     CONFIRMED       0.85      0.82      0.83       466
    FALSE POSITIVE   1.00      0.98      0.99       889

      accuracy                           0.91      1748
     macro avg       0.88      0.88      0.88      1748
    weighted avg     0.91      0.91      0.91      1748
  
  
### Random Forest with Gridsearch

* Accuracy = 0.5051487414187643
* Training Data Score: 1.0
* Testing Data Score: 0.9073226544622426

                precision    recall  f1-score   support

     CANDIDATE       0.02      0.30      0.03        23
     CONFIRMED       0.00      0.00      0.00         0
    FALSE POSITIVE   1.00      0.51      0.67      1725

      accuracy                           0.51      1748
     macro avg       0.34      0.27      0.24      1748
    weighted avg     0.99      0.51      0.67      1748
  
  
### KNN Score without Gridsearch

* Accuracy = 0.5011441647597255
* Training Data Score: 0.8571428571428571
* Testing Data Score: 0.7889016018306636

                precision    recall  f1-score   support

     CANDIDATE       0.00      0.00      0.00         0
     CONFIRMED       0.00      0.00      0.00         0
    FALSE POSITIVE   1.00      0.50      0.67      1748

      accuracy                           0.50      1748
     macro avg       0.33      0.17      0.22      1748
    weighted avg     1.00      0.50      0.67      1748
  

### KNN Score with Gridsearch

* Accuracy = 0.790045766590389
* Training Data Score: 0.6286477207705512
* Testing Data Score: 0.6464530892448512

                precision    recall  f1-score   support

     CANDIDATE       0.44      0.61      0.51       305
     CONFIRMED       0.71      0.58      0.64       556
    FALSE POSITIVE   1.00      0.99      0.99       887

      accuracy                           0.79      1748
     macro avg       0.72      0.72      0.71      1748
    weighted avg     0.81      0.79      0.80      1748


## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

- - -



































