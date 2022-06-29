## Decision Tree and Random Forest

### Problem 1: (`model_prob1.ipynb`) ###
We use the attached dataset called `annualrainfall.mat`. It contains a single matrix called XR that is 357x118. Each row refers to a 
location in India and each column refers to a year. We carry out the following steps:
- For each year, we calculate the total rainfall over all the locations. We calculate the mean (m) and 
standard deviation (s) of this quantity over all the years (columns).
- We ssign labels to each year according to the rule: if the total rainfall in any year is more than 
m+s, the label is +1, if the total rainfall in any year is below m-s, the label is
-1, else the label is 0.
- For each year, we try to predict the label of each year from the rainfall values at the different 
locations, using a Decision Tree of depth 10. We note down which locations are chosen. We use se the first 100 years 
for training using 5-fold cross validation, and the remaining 18 years for testing. Finally we lot both training and 
testing errors. [4 marks]
- We repeat the same analysis using a Random Forest and compare the results.
- Now, for each location, we define the mean and standard deviation of annual rainfall. We attach a 
label +1/0/-1 to each location, for each year, according to the rule previously used.
- We use a Decision Tree of depth 10 to predict the label at each location on any given year, using the 
labels at the remaining locations in the same year. For each location, we identify the top 10 predictor 
regions. Once again, we use the first 100 years for training with 5-fold cross-validation, and the remaining 
years for testing.
- We repeat the previous step with random forest. 

### Problem 2: (`model_prob2.ipynb`) ###
We download the MNIST dataset of handwritten digits 0-9. In each image we try to predict the label (0-9) 
using the pixel values. We train a decision tree of depth 20 and a random forest for this purpose.
We will increase the depth till 50 until we find a satisfactory accuracy. For each image class, we use 75% images for training 
and the rest for testing. Further we use 10-fold cross validation.
