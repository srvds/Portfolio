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

###  [Amazon Fashion Prediction System](https://github.com/srvds/Amazon-Fashion-Prediction-Engine)
* Predict similar apparel and recommend those apparell based on which apparel(query product) the user is watching.
* Data acquired in policy compliant manner using Amazon API.
* Text based product recommendation, i.e using product title, brand, description, color and price.
* Results with Text Featurized using BOW,TF-IDF, IDF,average word2vec,IDF weighted word2vec are subjectively compared.
* Product Image based model using **VGG-16 CNN** also trained.
* Final model build as a weighted Nearest neighbor model using Image,Title,Brand and Color
* final model uses title:Idf-Word2vec, brand:one hot encoding, colour:one hot encoding, image: VGG-16 CNN
* **Query product and a suggestion**
<p float="left">
 <img src="https://github.com/srvds/Amazon-Fashion-Prediction-Engine/blob/master/plots/plot1.PNG" width="400">
 <img src="https://github.com/srvds/Amazon-Fashion-Prediction-Engine/blob/master/plots/plot2.PNG" width="450" height="450">
</p>
 
###  [Taxi Demand Prediction](https://github.com/srvds/Taxi-Demand_Prediction)
* Predicted number of pickups, given location cordinates(latitude and longitude) and time.
* Time-series forecasting and Regression.
* New York citymap is divided into several regions based on region radius and density of passenger.
<p float="left">
 <img src="https://github.com/srvds/Taxi-Demand_Prediction/blob/master/plot/plot1.PNG" width="400">
 <img src="https://github.com/srvds/Taxi-Demand_Prediction/blob/master/plot/plot2.png" width="450" height="450">
</p>
 
