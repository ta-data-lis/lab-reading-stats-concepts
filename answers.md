## Challenge 1: What is the difference between expected value and mean?

Functionally, the two concepts are similar, as the expected value is calculated in the same way as the average: it is the probability-weighted average of the possible outcomes. The difference is in the context in which each concept is used.

Average is used in descriptive statistics to characterise a certain sample. On the other hand, the expected value is related to probabilities and it is the expected average of all possible samples of a population. In other words, given one experiment, we can calculate the average of its outcomes. The average will converge towards the expected value the more times an experiment is repeated.


## Challenge 2: What is the "problem" in science with p-values?

The "problem" with the use of p-values in science is related with the (human) tendency to present results as a dychotomy. When testing an hypothesis, we first study a null hypothesis that is incompatible with an alternative hypothesis that we want to demonstrate. We study the null hypothesis instead of going directly to the alternative hypothesis that is the real focus of our interest because the study of the p-value (given a certain threshold) allows us to dismiss an hypothesis as extremely unlikely to happen, but not demonstrate it.

The "problem in science" that the article talks about, then, is when studies attempt to use the p-value to positively demonstrate an hypothesis. They conclude that when the p-value is higher than the threshold they have set, then this not only means that the null hypothesis cannot be rejected, it's an actual demonstration of its truth. This is incorrect.

As the article explains, "all statistics, including p-values and confidence intervals, naturally vary from study to study, and often do so to a surprising degree." The image below intends to illustrate this assertion.

![alt text](https://github.com/mjvsilva/lab-reading-stats-concepts/blob/master/gauss.png "Normal distribution examples")

The three distributions in the image could represent the study of various samples from the same population. Their mean is the same but, because the standard deviation varies, in some cases the p-value might allow the rejection of some hypothesis and in other cases not. The results are the same but, because some tests were more or less accurate than others, the p-value also varies.


## Challenge 3: Applying testing to a specific case: A/B testing.

1) Characterise the original conditions: The original conditions are the A group/control group. In order to analyse it, the best suited metric needs to be determined. In the Netflix example, the first thing to do would be to determine the baseline probability that a film is viewed given its original cover image and then specify what percentage of an increase in views would justify the change to a new cover.

2) Test group: The next step in setting set up the experiment is to determine the size of the test group. Not knowing whether the cover change results in a negative or positive result, in order not to hurt the business, it is best to adopt a relatively small test group. However, the smaller the group, the longer it will take to collect the necessary data for the A/B test. It is also important to consider the minimum sample size needed for the experiment.

3) Compare data: The third step is to compare the data from the control group and the test group using hypothesis testing. The null hypothesis will be that the chosen metric (number of film views) did not change from the control group to the test group. The alternative hypothesis is that this metric increased (or decreased) in the test group.
