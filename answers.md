## Challenge 1: What is the difference between expected value and mean?

Functionally, the two concepts are very similar, as the expected value is calculated in the same way as the average: it is the probability-weighted average of the possible outcomes. The difference lies in the context in which each concept is used.

Average is used in descriptive statistics to characterise a certain sample. On the other hand, the expected value is related to probabilities and it is the expected average of all possible samples of a population. In other words, given one experiment, we can calculate the average of its outcomes. The expected value is the average obtained when performing repeated experiments. The average will converge towards the expected value the more times the experiment is repeated.


## Challenge 2: What is the "problem" in science with p-values?

a statistically non-significant result does not ‘prove’ the null hypothesis (the hypothesis that there is no difference between groups or no effect of a treatment on some measured outcome)1. Nor do statistically significant results ‘prove’ some other hypothesis.

we should never conclude there is ‘no difference’ or ‘no association’ just because a P value is larger than a threshold

Neither should we conclude that two studies conflict because one had a statistically significant result and the other did not.




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
