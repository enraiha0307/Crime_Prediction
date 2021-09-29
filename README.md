

<!--
*** Thanks for checking out this README Template. If you have a suggestion that would
*** make this better, please fork the repo and create a pull request or simply open
*** an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
***
***
***
*** To avoid retyping too much info. Do a search and replace for the following:
*** github_username, repo_name, twitter_handle, email
-->









<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/github_username/repo_name">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Crime Pediction and Analysis</h3>

  <p align="center">
   This analyses crime often occurring in a particular area and also predict the likelihood of occurrence of a crime in a particular area.
    <br />
    <!-- <a href="https://github.com/github_username/repo_name"><strong>Explore the docs »</strong></a>
    <br /> -->
    <br />
    <a href="https://github.com/enraiha0307/Crime_Prediction/issues">Report Bug</a>
    ·
    <a href="https://github.com/enraiha0307/Crime_Prediction/issues">Request Feature</a>
  </p>
</p>

## Problem Statement
Crime is increasing considerably day by day. Crime is among the main issues which is growing continuously in intensity and complexity. Crime patterns are changing constantly because of which it is difficult to explain behaviours in crime patterns.

So it becomes a difficult challenge for crime analysts to analyse such voluminous crime data without any computational support. A powerful system for predicting crimes is required in place of traditional crime analysis because traditional methods cannot be applied when crime data is high dimensional and complex queries are to be processed. Therefore a crime prediction and analysis tool were needed for identifying crime patterns effectively.
## Actions
To develop an efficient machine learning algorithm which could classify and predict the type of crime which might occur at a place at a given time and location in San Francisco City.
## Goals
- Predicting the type of crime before it happens which will not only provide extra edge to law enforcement agencies but will also help in detecting the crime hotspot in a particular region.
- Understanding and analysis of crime pattern which could help in decreasing the crime rate.
## Methodology
We used Predictive modeling for making predictions since it has the method which is able to build a model and has the capability to make predictions. This method consists of different algorithms of ML that can study properties from the data used for training which is used for producing predictions.

## Classification Algorithms Used
- Support Vector Machine
-K-nearest Neighbour
-Decision trees
-Extra Tree Classifier
-Artificial Neural Network

## Training and Testing
After validating the assumptions of the algorithm that we have chosen. Model is trained on the basis of given training Sample. After training, the performance of the model is checked on the basis of error and accuracy. At last, the trained model is tested with some unseen data and the model performance is checked on the basis of various performance parameters depending on the problem.

## Data Collection
We have used the crime data set of San Francisco city which is taken from kaggle.com in csv format and was derived from incidents present in SFPD Crime Incident Reporting system. The attributes of the data set are Date, category of crime, description, DayofWeek, Police Department District, Address, Latitude and longitude and contained 884k data points. This dataset provides nearly 12 years of crime reports from across all San Francisco’s neighbourhood. It is a multi-class classification problem, given time and location, the goal is to predict the category of crime that occurred.

## Data Analysis and Visualisation
Before processing data we tried to analyse the data first which was avail- able. So that we can find out which factors are affecting which type of crime and how is the crime distributed in different parts of the country. This information can then be used by the law enforcement agencies to analyse the crime more efficiently. From the figures 1.1 and 1.2 we observed that the most crimes are in the location of longitude from -122.44 to -122.40 and latitude from 37.76 to 37.80. This information can be used by the law enforcement agency to see which are the crime prone areas and increase the security in those areas accordingly. 
 <div class="images">
<img src="./images for crime prediction report/da2.PNG" alt="Fig 1.1"> 
  <br/>
<figcaption> Figure 1.1</figcaption>
  <br/>
<img src="./images for crime prediction report/da3.PNG" alt="Fig 1.2">
  <br/>
<figcaption> Figure 1.2</figcaption>
</div>

Figure below shows the distribution of assualt and Drug Narcotics across the city. From these figures we observed that there exist some crimes that is focused on certain locations, for example prostitution is focused mostly in (37.79N, -122.41W) and (37.76N, -122.41W). Other crimes are spread into the map like Assault and Drug narcotics.
 <div class="images">
<img src="./images for crime prediction report/da4.PNG" alt="Fig 1.3"> 
  <br/>
<figcaption> Figure 1.3</figcaption>
  <br/>
<img src="./images for crime prediction report/da5.PNG" alt="Fig 1.4">
  <br/>
<figcaption> Figure 1.4</figcaption>
  <br/>
<img src="./images for crime prediction report/da6.PNG" alt="Fig 1.5">
  <br/>
<figcaption> Figure 1.5</figcaption>
</div>

## Training Models
For training the data splitted in the ratio of 80% for training and 20% for testing using sklearn library.
As a result we train size of around 114000 data points and test size of around 28000 data points. After trying different combinations of
the parameters for each classification algorithm used, the optimal value of accuracy and Fscore was obtained the parameters chosen for each
model is as shown below. Here basically five models as mentioned in the methodology were used for traning purpose. After trying different 
combinations of parameters for each of the models different models were trained and their fscore, accuracy etc were calculated. 
For KNN the parameters used were n jobs and >weights and their values were set to minus one and balanced respectively.

Similarly for Decision tree the parameter used was class weight and whose value was set to balance and similarly the parameter tuning was done for other models to get best output from each case possible. For MLP after trying different parameter tuning it was found that it worked best for 100 hidden layers and adam solver. Here as evident from the graph that SVC is taking lot of training time hence this cannot be considered. Where as if we look for KNN it has good value of fscore along with better accuracy and optimal training time as compared to others. So, it is best to use neural network for this purpose.

## Results
As seen from figures, SVC is taking huge amount of time in training than other models so it is not a good model. Similarly for Artificial Neural network its accuracy is least, so it is not a good option for classification. Now we are left with KNN, decision trees and Extra tree classifier.Here we can see from table that Decision tree and Extra tree classifier are working best with optimal training and good accuracy. Moreover the testing accuracy of ANN, SVM, KNN, Decision tree and Extra tree classifier are 12%, 67%, 73%, 74% and 74% percent respectively. From here also it is evident that Decision tree and Extra tree classifier are performing better than other.


### Built With

* Python
* pandas
* numpy
* IPython
* libgeos
* matplotlib
* pyproj
* collections
* math
* sklearn







<!-- CONTACT -->
## Contact

Akanksha Gahalot - [@AkankshaGahalot](https://twitter.com/AkankshaGahalot) 

Project Link: [https://github.com/enraiha0307/Crime_Prediction](https://github.com/enraiha0307/Crime_Prediction)





<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/github_username/repo.svg?style=flat-square
[contributors-url]: https://github.com/github_username/repo/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/github_username/repo.svg?style=flat-square
 [forks-url]: https://github.com/github_username/repo/network/members
 [stars-shield]: https://img.shields.io/github/stars/github_username/repo.svg?style=flat-square
 [stars-url]: https://github.com/github_username/repo/stargazers
 [issues-shield]: https://img.shields.io/github/issues/github_username/repo.svg?style=flat-square
 [issues-url]: https://github.com/github_username/repo/issues
 [license-shield]: https://img.shields.io/github/license/github_username/repo.svg?style=flat-square
[license-url]: https://github.com/github_username/repo/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/github_username
 [product-screenshot]: images/screenshot.png
