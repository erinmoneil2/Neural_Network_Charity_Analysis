# Neural_Network_Charity_Analysis

## Overview
The purpose of this project is to use our knowledge of machine learning and neural networks to create a binary classifer that is capable of predicting whether applicants who were funded by Alphabet Soup were successful with their investment. 

## Results
### Data Processing 

The target in this model is whether the investment/project was successful or not, defined by the column "IS_SUCCESSFUL". 

For the variables, I put all the other columns.  

In the first Deliverable, we remvoed the EIN and the NAME of the project/funded organization because it does not add any additional categorical data to the dataset. For our Optimization deliverable, I also removed the SPECIAL_CONSIDERATIONS" column. 

![Screen Shot 2022-03-05 at 9 33 00 AM](https://user-images.githubusercontent.com/92831268/156894250-9715945e-b3e6-437f-b93e-1582c54e9ae6.png)

In addition, I changed the binning of the APPLICATION_TYPE to have one less bin. 
![Screen Shot 2022-03-05 at 9 33 11 AM](https://user-images.githubusercontent.com/92831268/156894290-ec83e714-0c48-4442-aaf2-78584bda5aab.png)

### Compiling, Training, and Evaluating the Model 
FOr my optimization, I utilized 4 hidden layers. I had originially tried two, and then 3, and then 4. Each time increased the accuracy score by a very small amount. I left the neurons somewhere between 80-30 as we did in the originaly model, but used a number in between, decreasing by each layer. I also used the sigmoid activiation within the hidden layers because we are trying to find a binary classifier (successful or not successful). 

![Screen Shot 2022-03-05 at 9 33 31 AM](https://user-images.githubusercontent.com/92831268/156894392-2651626e-fb56-4027-94fd-0dede4f2412f.png)

Lastly I changed the epochs to 50. It seemed as if the more epochs I used, the smaller the accuracy score got. 

![Screen Shot 2022-03-05 at 9 33 46 AM](https://user-images.githubusercontent.com/92831268/156894452-3633d126-422f-4a8d-8ee1-afcc3dee2088.png)

In order to achieve an increased performance, I changed the binning for application types, I dropped special_considerations from our variables, I added two additional layers, and lowered the epochs. I was unable to acheive the performance of 75% or higher accuracy score. My accuracy score only increased by 0.002%, however, this was the closest accuracy score through trial and error that I was able to acheive. All other attempts resulted in a lower accuracy score. 

![Screen Shot 2022-03-05 at 9 33 52 AM](https://user-images.githubusercontent.com/92831268/156894543-ef59d23c-cfe5-4197-88bf-0d6241218d0b.png)

## Summary
Overall, I was able to reach an accuracy score of 72.6%, which was only .2-3% higher than the accuracy score acheived in the first model (Deliverable 1). My recommendation would be to potentially bin by amounts instead of by application type. We only have 17 application types, but over 8,000 different ammounts. It might be more accurate to see if the amount of what was asked for was more successful than by what type of application we are submitting. 
