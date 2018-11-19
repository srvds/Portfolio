# Data Science Portfolio


In this repository, I have put some of the Data science projects, I have worked on or currently working. 
All the projects will mostly focus on utilizing Machine Learning and Deep Learning Techniques to design data science or statistical models, that either solves a problem or discovers important information about the data.

## NOTE:
* I am in the process of Documenting the projects like how to reproduce results and more.
* Most of it can also be found in the respective Jupyter notebooks even if the README files are not yet updated

Click on the projects to see the documentation and code.
(Project Repository README are being build,meanwhile check the ipython notebooks, they are sufficiently documented)

## Projects:

###  [Human Activity Recognition](https://github.com/srvds/Human-Activity-Recognition)
* Predicted Activity based on Accelerometer and Gyroscope readings from smart phone
| 1. Walking | 2. WalkingUpstairs | 3. WalkingDownstairs | 4. Standing | 5. Sitting | 6. Lying
* Fitted Logistic Regression|Linear SVC |rbf SVM classifier|DecisionTree |Random Forest |GradientBoosting DT on featured data
* LSTM model trained on Raw data
* **t-sne Visualization**
<img src="https://github.com/srvds/Human-Activity-Recognition/blob/master/t-sne_perp_50_iter_1000.png" width="700">

---

###  [Amazon Fashion Prediction System](https://github.com/srvds/Amazon-Fashion-Prediction-Engine)
* Predict similar apparel and recommend those apparell based on which apparel(query product) the user is watching.
* Data acquired in policy compliant manner using Amazon API.
* Text based product recommendation, i.e using product title, brand, description, color and price.
* Results with Text Featurized using BOW,TF-IDF, IDF,average word2vec,IDF weighted word2vec are subjectively compared.
* Product Image based model using **VGG-16 CNN** also trained.
* Final model build as a weighted Nearest neighbor model using Image,Title,Brand and Color
* final model uses title:Idf-Word2vec, brand:one hot encoding, colour:one hot encoding, image: VGG-16 CNN
* **Query product**     
 <img src="https://github.com/srvds/Amazon-Fashion-Prediction-Engine/blob/master/plots/plot1.PNG" width="400">
 
* **Suggested product**
 <img src="https://github.com/srvds/Amazon-Fashion-Prediction-Engine/blob/master/plots/plot2.PNG" width="400">

---

###  [Taxi Demand Prediction](https://github.com/srvds/Taxi-Demand_Prediction)
* Predicted number of pickups, given location cordinates(latitude and longitude) and time of the day.
* Time-series forecasting and Regression.
* New York citymap is divided into several regions based on region radius and density of passenger.
* **K-means clustering** used for geometric division of the city map
* Time series data is divided into 10 minutes interval.
* Frequency domain features are also used along with time domain data to improve the model.
* Linear Regression, Random Forest and Gradient Boosted Decision trees(GBDT) models were trained and tested.
* GBDT model performed better than other models
<p float="left">
 <img src="https://github.com/srvds/Taxi-Demand_Prediction/blob/master/plot/plot1.PNG" width="400">
 <img src="https://github.com/srvds/Taxi-Demand_Prediction/blob/master/plot/plot2.png" width="450" height="450">
</p>

---

###  [Quora question similarity](https://github.com/srvds/Quora-question-similarity)
* Identify which questions asked on Quora are duplicates of questions that have already been asked.
* Modelled as classification problem with class as duplicate and not duplicate.
* 15 features are extracted, some of them are:
 * word_common: Number of common unique words in question1 and question2.
 * word_total: toal number of words in qs1 + total number of words in qs2.
 * word_share: (word_common) / (word_total)
 * common_word_count / min( len(q1 word), len(q2 word))
* along with the above extracted features question text is featured using tf-idf.
* Fitted Logistic Regression, Linear SVM and XGboost gradient boosted decision trees.
* Question appearance count.
 <img src="https://github.com/srvds/Quora-question-similarity/blob/master/plots/plot3.png">
* Word Cloud for Duplicate Question pairs.<br>

 <img src="https://github.com/srvds/Quora-question-similarity/blob/master/plots/plot1.png">

* Word Cloud for Duplicate Question pairs.<br>
 <img src="https://github.com/srvds/Quora-question-similarity/blob/master/plots/plot2.png">

---

###  [Netflix Movie Recommendation System](https://github.com/srvds/Netflix-Movie-Recommendation)
* Predicted the rating that a user would give to a movie that they have not yet rated.
* Minimized the difference between predicted and actual rating (RMSE and MAPE).
* Generated user-user and movie-movie similarity matrix.
* Featurized the data further into 13 features.
* Models trained: Surprise-baseline, Surprise-knn-baseline, Surprise-SVD++, XGboost
<img src="https://github.com/srvds/Netflix-Movie-Recommendation/blob/master/plots/plot1.png">

---

###  [Personalized Cancer Diagnosis](https://github.com/srvds/Personalized-Cancer-Diagnosis)
* Classified the given genetic variations/mutations based on evidence from text-based clinical literature into 9 classes.
* dataset 3 important attributes 'Gene' 'Variation' and 'Clinical text'.
* Dataset is imbalanced, modeled with and with out balancing to compare results.
* Clinical text featurized using tf-idf. Gene and variation are featured using both One-hot encoding and response coding.
* Dimensionality reduction of text vector using truncated SVD.
* fitted and compared various models including Logisting Regression, Linear SVC , Naive Bayes and Random forest
* experimented with stacking the models and also to use max-voting on the results of the models.
* Interpretability of results is important here so a calibrated classifier is stacked with the models 
* ploted Confusion,precision and recall matrices to have more Interpretability.
<img src="https://github.com/srvds/Personalized-Cancer-Diagnosis/blob/master/plots/rf-responsecode-pricision.png">

