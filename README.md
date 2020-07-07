# Exoplanet Exploration

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

### * After comparing the following models, it looks like Random Forest Classifier Model gives the best Accuracy Score for the data. 
### * Although it was better after the model is tuned, it is not a good idea to use KNN model for this data. 

### SVM without Gridsearch

* Accuracy = 0.7871853546910755
* Training Data Score: 0.7808506580202175
* Testing Data Score: 0.7871853546910755

                    precision    recall  f1-score   support

         CANDIDATE       0.16      0.88      0.28        78
         CONFIRMED       0.96      0.55      0.70       783
      FALSE POSITIVE     1.00      0.99      0.99       887

          accuracy                           0.79      1748
         macro avg       0.71      0.81      0.66      1748
      weighted avg       0.94      0.79      0.83      1748


### SVM with Gridsearch

* Accuracy = 0.7894736842105263
* Training Data Score: 0.7840930764829296
* Testing Data Score: 0.7894736842105263

                    precision    recall  f1-score   support

         CANDIDATE       0.18      0.85      0.30        92
         CONFIRMED       0.95      0.56      0.70       769
      FALSE POSITIVE     1.00      0.99      0.99       887

          accuracy                           0.79      1748
         macro avg       0.71      0.80      0.67      1748
      weighted avg       0.93      0.79      0.83      1748

### Decision Tree 

* Accuracy = 0.8569794050343249
* Training Data Score: 1.0
* Testing Data Score: 0.8569794050343249

                        precision    recall  f1-score   support

             CANDIDATE       0.99      0.49      0.65       858
             CONFIRMED       0.01      0.02      0.02       266
        FALSE POSITIVE       0.70      0.99      0.82       624

              accuracy                           0.60      1748
             macro avg       0.57      0.50      0.50      1748
          weighted avg       0.74      0.60      0.62      1748


### Random Forest without Gridsearch

* Accuracy = 0.9016018306636155
* Training Data Score: 1.0
* Testing Data Score: 0.9016018306636155

                        precision    recall  f1-score   support

             CANDIDATE       0.78      0.83      0.80       396
             CONFIRMED       0.83      0.80      0.82       465
        FALSE POSITIVE       1.00      0.99      0.99       887

              accuracy                           0.90      1748
             macro avg       0.87      0.87      0.87      1748
          weighted avg       0.90      0.90      0.90      1748

### Random Forest with Gridsearch

* Accuracy = 0.9033180778032036
* Training Data Score: 1.0
* Testing Data Score: 0.9033180778032036

                        precision    recall  f1-score   support

             CANDIDATE       0.77      0.84      0.80       389
             CONFIRMED       0.84      0.80      0.82       472
        FALSE POSITIVE       1.00      0.99      0.99       887

              accuracy                           0.90      1748
             macro avg       0.87      0.88      0.87      1748
          weighted avg       0.91      0.90      0.90      1748

  
### KNN Score without Gridsearch

* Accuracy = 0.7877574370709383
* Training Data Score: 0.8586687011253099
* Testing Data Score: 0.7877574370709383


                     precision    recall  f1-score   support

         CANDIDATE       0.48      0.59      0.53       343
         CONFIRMED       0.67      0.58      0.62       520
      FALSE POSITIVE     1.00      0.99      0.99       885

          accuracy                           0.79      1748
         macro avg       0.72      0.72      0.71      1748
      weighted avg       0.80      0.79      0.79      1748
  

### KNN Score with Gridsearch

* Accuracy = 0.7820366132723112
* Training Data Score: 0.8176616440968911
* Testing Data Score: 0.7820366132723112

                    precision    recall  f1-score   support

         CANDIDATE       0.00      0.00      0.00       668
         CONFIRMED       0.98      0.50      0.66       886
      FALSE POSITIVE     0.22      1.00      0.36       194

          accuracy                           0.36      1748
         macro avg       0.40      0.50      0.34      1748
      weighted avg       0.52      0.36      0.38      1748


## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

- - -



































