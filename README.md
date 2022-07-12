# Healthcare Research

## Introduction 

In this research we first use a mixture of gaussian models to describe the duration between the two highest peaks in the signal of one footstep. We recorded this value from the patient through time and notice that it follows the distribution dictated by a mixture of two gaussians. The signal recorded is therefore assumed to come from two gaussians  (one gaussian corresponds to the fatigued state and the second to the non-fatigued state). We use the Expectation Maximization algorithm to learn the parameters of the two gaussians. This step allows us to personalized the algorithm to the patient. Even though most of the patients have mostly identical fatigued and non-fatigued models (10 for mu and 1 and .1 for resp the fatigued and non-fatigued models) we thought that personalizing the algorithm to learn the parameters from the subject would make the prediction even more effective. 
Once we have learn the parameters from the data we can make prediction using the forward-backward algorithm. For the assignment we simply cluster by taking the class with the highest probability. 

## Learning the parameters of the mixture of Gaussian

