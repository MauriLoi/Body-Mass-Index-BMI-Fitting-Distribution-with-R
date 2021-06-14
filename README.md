# Body-Mass-Index-BMI-fitting-Distribution-with-R

The data used for the study are taken from a marketing campaign dataset based on a case of a retailer company in computer accessories. The data set contains 1500 customer records. Each record consists of 19 variables, which includes socio-demographic and product ownership information. 
The work is developed following the below index, starting from the Data Understanding , untill the development of a logistic regression Model.


1. Body Mass Index (BMI) Data set

   1.1 Introduction 
    
   1.2 Selection of all the possible Distributions

   1.3 Distribution choice
    
   1.4 Output the Parameters
   
## Introduction to the Body Mass Index (BMI) data set 

The aim of this section of the report is to analyze the data set previous given of the Body Mass Index(BMI) from the Fourth Dutch Growth Study, Fredrisk et al.(2000a) and find a suitable probability distribution to fit at the data. The dataset reports 7482 observations and has as explanatory variable the age. The age range from 0.03 (3 days) to 21.70 (21 years and 7 months).The first step is to create a sub set of observations for a single year. I have decided to choose as a year of my subset data the age from 14 to 15.
Fitting a distribution is the process of finding a mathematical function that represent at the best a statistical variable in our case the BMI. In practice given the unknown distribution density (pdf) derivate from our observation sample that is an univariate continuous distribution with domain[0,+∞ ] we need to select an appropriate distribution that is able to approximate the behavior of the empirical data. I will use a two steps approach the fitting stage and the diagnostic one. I will fit different distribution and compare them using the generalized Akaike information criterion (GAIC) given the nature of not nested gamlss models. After I have compered the different result I will choose the one with the smallest GAIC(k) after the selection of the value k. Reminding the fact that GAIK(k)=GD + (k *df), where df is the effective degree of freedom used in the model and GD is the fitted Global deviance. The first approach is to explore the data with histograms and short descriptive stats, the frequency histogram with 60 bins of the values, the empirical density function and the empirical cumulative frequency distributions are reported below (see figure 1,3 and 4 for the BMI data set ). Descriptive statistic of the distribution as the mean, standard deviation, skewness, kurtosis this could be done using the descdist(). A skewness-kurtosis plot proposed by Cullen and Frey (1999) provided by the descdist() function is shown above (see Figure 2 for the BMI data set).




