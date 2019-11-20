## Challenge 1: What is the difference between expected value and mean?

Functionally, the two concepts are very similar, as the expected value is calculated in the same way as the average: it is the probability-weighted average of the possible outcomes. The difference lies in the context in which each concept is used.

Average is used in descriptive statistics to characterise a certain sample. On the other hand, the expected value is related to probabilities and it is the expected average of all possible samples of a population. In other words, given one experiment, we can calculate the average of its outcomes. The expected value is the average obtained when performing repeated experiments. The average will converge towards the expected value the more times the experiment is repeated.


## Challenge 2: What is the "problem" in science with p-values?

The "problem" with the use of P-values in science is related with the (human) tendency to present results as a dychotomy. When testing an hypothesis, we first study a null hypothesis that is incompatible with an alternative hypothesis that we want to demonstrate. We study the null hypothesis instead of going directly to the alternative hypothesis that is the real focus of our interest because the study of the P-value (given a certain threshold) allows us to dismiss an hypothesis as extremely unlikely to happen, but not demonstrate it.

The "problem in science" that the article talks about, then, is when studies attempt to use the P-value to positively demonstrate an hypothesis. They conclude that when the P-value is higher than the threshold they have set, then this not only means that the null hypothesis cannot be rejected, it's an actual demonstration of its truth. This is incorrect.

As the article explains, "all statistics, including P-values and confidence intervals, naturally vary from study to study, and often do so to a surprising degree." The image below intends to illustrate this assertion.

![alt text](https://github.com/mjvsilva/lab-reading-stats-concepts/blob/master/gauss.png "Normal distribution examples")

The three distributions in the image could represent the study of various samples from the same population. Their mean is the same, but because the standard deviation varies, in some cases the P-value might allow the rejection of some hypothesis and in other cases not. Just because the 95% (or whatever accepted range in the field) falls on a certain range of values, this does not mean that the values inside the 95% region are


## Challenge 3: Applying testing to a specific case: A/B testing.
A/B testing is a widely used tool to understand differences between two samples. It is a way to measure the impact of something we did:

A marketing campaign.
A new feature in our application.
A new design in our application.
A different flow in the User Experience flow.
To do this, is very important first to design our experiment.

We need to know how we are measuring the impact. If people has the behaviour we want with this new implementation.
We choose a control group (people who doesn't have/see the new change) and the group which will see the new change.
We think about how much data do we need.
We measure the difference between them.
One example: Our application has a lot of mini-games. We want people to reach the games that we think are the best but the behaviour is not the expected, they don't reach them.

So we call a designer and after a lot of work he shows us a new design for our application: we will add a botton specific for that kinf of games inviting the users to click on it:

Click here to discover cool games!

We think it will work but can we be sure? So instead of implementing this new botton for all users, we implement it for 10% and we compare the results with the users that didn't have it. Is there a significant difference? Is our botton working?

Read more about A/B testing with a couple of examples:

Another example about Netflix here

What happened to Basecamp

An example with Python

A cool general explanation

So, take one single example in the articles you just read, which specific test/s would you apply? (We want you just to do a draft and think a little bit how to apply the tests you already know in this case)
