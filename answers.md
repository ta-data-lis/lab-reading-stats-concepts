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

So, take one single example in the articles you just read, which specific test/s would you apply? (We want you just to do a draft and think a little bit how to apply the tests you already know in this case)

