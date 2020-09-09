# Questions 1 (What is the difference between expected value and mean?):

-Expected value is the average value of a random variable over a large number of experiments.
 We can calculate the expected value for a discrete random variable (one in which the number of potential outcomes is countable) by taking a sim in which each term is a possible value of the random variable multiplied by the probability of that outcome.
 
-The mean is the average of a set of numbers. To find the mean of a data set, add up all of the numbers in the set, and then divide that total by the number of numbers in the set.

-A practical approach results in a frequency distribution and a mean value, a theoretical approach results in a probability distribution and an expected value.
 If the sample space is infinitely large, the mean value should approach the expected value every time.



# Question 2 (What is the "problem" in science with p-values?):

-The "Problem" in science with p-values is that every scietis and researcher have been warned that a statustically non-significant result does not 'prove' the null hypothesis (the hypothesis that there is no difference between groups or no effect of a treatment on some measured outcome), nor do statistically significant results 'prove' some other hypothesis.

-Like this article states: We should never conclude there is 'no difference' or 'no association' just because a P value is larger than a threshold such as 0.05 or, equivalently, because a confidence interval includes zero.
 Neither should we conclude that two studies conflict because one had a statistically significant result and the other did not.
 
-The problem in science is that bucketing results into 'statistically significant' and 'statistically non-significant' makes people think that the items assigned in that way are categorically difference, which it *can or cannot be the case*.
 


# Question 3 (Applying testing to a specific case: A/B testing) :

-For this question I'll be using Netflix as an example, so:
 Netflix knows that if you don't capture a member's attention within 90 seconds, that member will likely lose interest and move onto another activity.
 Through various studies, they found that the members look at the artwork first and then decide whether to look at addicional details, and they wanted to capitalize on this.
 Broadly, Netflix's A/B testing philosophy is about building incrementally, using data to drive decisions, and failing fast.
 
-They experimented using a movie as a Poc, 'The Short Game' measured the engagement with the title for each variant (click through rate, aggregate play duration, fraction of plays with short duration, fraction of content viewed (how far did you get through a mive or series), changing the image from user to user(A/B testing).

-Then, they decided to expand to a two way multi-cell explore-exploit test, where they measured the engagement of each user artwork for a set of titles, 'Explore'.
 Finallly they went to 'Exploit', wich means that the test served the most engaging artwork (from 'explore' test) for future users and see if we can improve aggregated streaming hours.
 
-It is my opinion that A/B testing is one of the most usefull testing methods, because it can be braodly applied to almost everything.
 This is highly important because it can help making decisions based on real data.