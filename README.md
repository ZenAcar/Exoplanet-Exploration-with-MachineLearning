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

* Accuracy = 0.7488558352402745
* Training Data Score: 0.7808506580202175
* Testing Data Score: 0.7871853546910755

                        precision    recall  f1-score   support

             CANDIDATE       0.95      0.51      0.67       786
             CONFIRMED       0.13      0.57      0.21       104
         FALSE POSITIVE      0.97      0.99      0.98       858

              accuracy                           0.75      1748
             macro avg       0.68      0.69      0.62      1748
          weighted avg       0.91      0.75      0.79      1748


### SVM with Gridsearch

* Accuracy = 0.8054919908466819
* Training Data Score: 0.7840930764829296
* Testing Data Score: 0.7894736842105263

                precision    recall  f1-score   support

         CANDIDATE       0.89      0.57      0.69       661
         CONFIRMED       0.36      0.82      0.50       198
       FALSE POSITIVE    0.99      0.98      0.99       889

          accuracy                           0.81      1748
         macro avg       0.75      0.79      0.73      1748
      weighted avg       0.88      0.81      0.82      1748

### Decision Tree 

* Accuracy = 0.8735697940503433
* Training Data Score: 0.737745565515926
* Testing Data Score: 0.7408466819221968

                    precision    recall  f1-score   support

         CANDIDATE       0.75      0.77      0.76       408
         CONFIRMED       0.79      0.76      0.77       469
        FALSE POSITIVE   0.98      0.98      0.98       871

          accuracy                           0.87      1748
         macro avg       0.84      0.84      0.84      1748
      weighted avg       0.87      0.87      0.87      1748


### Random Forest without Gridsearch

* Accuracy = 0.9021739130434783
* Training Data Score: 0.737745565515926
* Testing Data Score: 0.7408466819221968

                    precision    recall  f1-score   support

         CANDIDATE       0.78      0.83      0.80       396
         CONFIRMED       0.83      0.80      0.82       466
        FALSE POSITIVE   1.00      0.99      0.99       886

          accuracy                           0.90      1748
         macro avg       0.87      0.87      0.87      1748
      weighted avg       0.90      0.90      0.90      1748
  
  
### Random Forest with Gridsearch

* Accuracy = 0.7408466819221968
* Training Data Score: 1.0
* Testing Data Score: 0.9050343249427918

                    precision    recall  f1-score   support

         CANDIDATE       1.00      0.49      0.65       861
         CONFIRMED       0.00      0.00      0.00         0
        FALSE POSITIVE   1.00      0.99      0.99       887

          accuracy                           0.74      1748
         macro avg       0.66      0.49      0.55      1748
      weighted avg       1.00      0.74      0.83      1748
  
  
### KNN Score without Gridsearch

* Accuracy = 0.5371853546910755
* Training Data Score: 0.8586687011253099
* Testing Data Score: 0.7877574370709383

                    precision    recall  f1-score   support

         CANDIDATE       0.74      0.47      0.58       666
         CONFIRMED       0.00      0.00      0.00         0
        FALSE POSITIVE   0.71      0.58      0.64      1082

          accuracy                           0.54      1748
         macro avg       0.49      0.35      0.40      1748
      weighted avg       0.72      0.54      0.62      1748
  

### KNN Score with Gridsearch

* Accuracy = 0.566933638443936
* Training Data Score: 0.8176616440968911
* Testing Data Score: 0.7820366132723112

                    precision    recall  f1-score   support

         CANDIDATE       0.44      0.59      0.50       315
         CONFIRMED       0.69      0.57      0.63       546
        FALSE POSITIVE   1.00      0.99      0.99       887

          accuracy                           0.79      1748
         macro avg       0.71      0.72      0.71      1748
      weighted avg       0.80      0.79      0.79      1748


## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

- - -



































