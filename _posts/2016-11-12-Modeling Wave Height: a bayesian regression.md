![Capstone Model1](/images/Unknown-9.png)

This model is intended to predict the likelihood that the tide is above 15 meters in order to ensure the viability of a surf shack next to the beach. The data is organized in a dataframe with time and tide height at one specific location as the two variables. I will build a bayesian regression and, thus, will have access to the exact probability of the tide (given the data being observed) being over 15 meters and can decide if that's a risk worth taking. 

To begin, a visualization of the data in the form of a scatterplot. The data seems to oscillate repetitively, so a sine or cosine wave could be used in the regression. 

![Capstone Model1](/images/Unknown-8.png)

Next, I create a function with one argument (a list of parameters for our model) that returns the natural log of the posterior, the log prior plus the log likelihood (likelihood * prior). When the function is called, the log likelihood is calculated with an iteration through the data. """"""""" Model takes shape of sinosoidal wave. equation

At this point I employed the emcee sampler (Monte Carlo-Markov Chain) to sample from my posterior distribution. This returns the values for a specified amount of samplers, the values of which represent a """""""""".

The Monte Carlo function then """"""""" and returns values for my hyperparameters.

I used the values of these hyperparameters to graph the regression line overlayed on the prior scatterplot to demonstrate the fit. 

![Capstone Model1](/images/Unknown-9.png)

This following graph shows the probability densities of the hyperparameters, calculated from the histogram of the values of each hyperparemeter from the samples data collected from the emcee sampler. 

![Capstone Model1](/images/Unknown-10.png)

And here is the corner plot, again for each of the hyperparameters. 

![Capstone Model1](/images/Unknown-12.png)



![Capstone Model1](/images/Unknown-11.png)