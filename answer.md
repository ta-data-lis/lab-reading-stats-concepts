## Challenges

### Challenge 1 What is the difference between expected value and mean

 The mean or average is the sum of the observations divided by the number of observations. The expected value is the average value expected to be obtained from an experiment.

 The first is a statistic out a sample and the second is a characteristic of a distribution.

 If you are 100% sure that you know the actual distributiondata generation process, then these would be the same.


### Challenge 2 What is the problem in science with p-values

  A p-value is the probability of obtaining an effect at least as extreme as the one in your sample data, assuming the truth of the null hypothesis (parameter = 0 usually).

  P-Values (or confidence metrics generally) are not that simple to interpret. They are more sample dependent than theoritical distribution dependent (they actually impose and assumption on the latter), which is obvious since we don't have the th distribution, but people often forget that. In particular, a low P-value indicates that your data are unlikely to be assuming a true null hypothesis (nullh0), but doesn't help you know if the null is true but the sample is biased or if the null is false. Further to that P-Value is alternative hypothesis(h1) dependent and it might be hard at times to know which h1 is more plausible.
 
  Another minor matter, but that is relevant in scientific publishing is that the p-Value statistical significance threshold (in science) is totally random, why 0.050.010.005  Meaning, the value of the p-value matters.
 

### Challenge 3 Applying testing to a specific case AB testing.

 Netflix article is interesting, controling for basic characteristics of the people would be nice such as gender, locations, langauge etc.
 They can go further and even use the variables they already have to know if people are into or not the different genres and see if that would have an impact given the image.
 People that like psychology might like one picture more and chess nerds might like another picture more and both like the Queen's Gambit show. I am pretty sure they could do that. Maybe they can't identify the chess nerds, but they can identify the drama lovers, the psyche lovers, the thriller ones... etc.