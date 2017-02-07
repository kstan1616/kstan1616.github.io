![PairPlot](/images/Unknown-16.png)

Here I have built a model to predict whether a loan will default or not using data from Lending Club, an innovative peer-to-peer lending company. The dataset contains information on several thousands of loans, mostly basic financial and personal details. The model employs a logistic regression. 

The data was imported from a csv file that Lending Club had released publically. Here is some intial EDA:

![PairPlot](/images/Unknown-15.png)

![PairPlot](/images/Unknown-14.png)

![PairPlot](/images/Unknown-13.png)

With the values for my parameters I continued on to predict the outcome of several lines of data, of which I had the information of the loan status, and thus could verify if the model worked well or not. I found that my model does give higher probability to customers paying when they do (true positives) than customers defaulting, but the probability estimate is greater than 50% (the amount of defaults in the dataset) so there would be many false positives. 

I think I could better my model by simplifying it and building up from there, one by one, assuming that it was correctly done this time. Overall, I learned a lot in this project about RLS (although that wasn't the point of the exercise), cleaning data, using pandas dataframes, and improving my grasp on the statistical methods that we have been using. 


