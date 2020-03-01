<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Lab | Reading About Statistic Concepts

## Introduction

In the future, you will need to understand deep statistical concepts by reading technical articles. As a training for that, it is interesting to start from here. Also, as we have limited time, this is a way to have some self guided learning to understand everything better and have a wider knowledge.

This week you will find some questions here that you will need to answer by documentating yourself. So you will do a different PR for each question (you are meant to answer the questions in different days). Don't hesitate to write as many text as you need and push images if you need them.

Remember for this lab: there is a right answer. But there is no perfect way to explain it (except for in a mathematical way, but this is another story).

## Challenges

### Challenge 1: What is the difference between expected value and mean?
You know both concepts but, is there a difference? Are they synonims? Start investigating. 

As a good reference (once you have looked for some information) you have   [this](http://expected.news/value2) article.


#Answer: 

A random variable maps numeric values to each possible outcome in an experiment. 
We can calculate expected value for a discrete random variable — one in which the number of potential outcomes is countable — 
by taking a sum in which each term is a possible value of the random variable multiplied by the probability of that outcome. 

For example, I come up to you and offer you to play coins, if it’s heads, I get a dollar, if it’s tails, you get three dollars. 
Easy bet right? The mean is (3+(−1))/2=+1. The mean outcome is +1 for you. But, what I don’t tell you is that the coin flips heads with probability of .8 and tails with probability of .2. 
The expected value is not +1 for you, but instead (0.8∗−1)+(0.2∗3)=−0.2. 
The expected value is the weighted mean for a random event like described above. 
The mean is the expected value but for samples, instead of random variables.

However, if you treat your sample as a distribution, then the mean and the expected value are the same thing. For instance, 
if X is a random variable then we can usually define the expected value of X to be either the sum of X*p(X),where p(X) is the probability density or probability mass function. 
This is frequently called the mean of X and in this context the terms may be used interchangeably. 
However, if you have a list of N numbers a1,a2,…,aN, then the mean of that list of numbers is 1/N*(a1+a2+⋯+aN). 
This definition has nothing inherently to do with probability, and we wouldn't call this the "expected value" of the list. They are 
closely related however: if you have a list of numbers drawn from some probability distribution, then taking the mean of that list is 
usually a very good way to estimate the expected value of the probability distribution.

### Challenge 2: What is the "problem" in science with p-values?
We have told you that a lot of scientifical investigations are based on p-values. The last week, Nature magazine published [an article](http://nature.social/statistical4) regarding the problem. Start digging on it!

#Answer:

Academics in the scientific community should never conclude there is ‘no difference’ or ‘no association’ just because a P value is larger 
than a threshold such as 0.05 or, equivalently, because a confidence interval includes zero. Neither should we conclude that two studies conflict 
because one had a statistically significant result and the other did not. These errors waste research efforts and misinform policy decisions.

One reason to avoid such ‘dichotomania’ is that all statistics, including P values and confidence intervals, naturally vary from study to study, 
and often do so to a surprising degree. In fact, random variation alone can easily lead to large disparities in P values, far beyond falling just to 
either side of the 0.05 threshold. For example, even if researchers could conduct two perfect replication studies of some genuine effect, each with 80% 
power (chance) of achieving P < 0.05, it would not be very surprising for one to obtain P < 0.01 and the other P > 0.30. Whether a P value is small or 
large, caution is warranted.


Don't hesitate to use more articles if you want to :)


### Challenge 3: Applying testing to a specific case: A/B testing.
A/B testing is a widely used tool to understand differences between two samples. It is a way to measure the impact of something we did: 
* A marketing campaign.
* A new feature in our application. 
* A new design in our application.
* A different flow in the User Experience flow.

To do this, is very important first to design our experiment. 
* We need to know how we are measuring the impact. If people has the behaviour we want with this new implementation.
* We choose a control group (people who doesn't have/see the new change) and the group which will see the new change. 
* We think about how much data do we need.
* We measure the difference between them.

One example:
Our application has a lot of mini-games. We want people to reach the games that we think are the best but the behaviour is not the expected, they don't reach them.

So we call a designer and after a lot of work he shows us a new design for our application: we will add a botton specific for that kinf of games inviting the users to click on it:

*Click here to discover cool games!*

We think it will work but can we be sure? So instead of implementing this new botton for all users, we implement it for 10% and we compare the results with the users that didn't have it. Is there a significant difference? Is our botton working?

Read more about A/B testing with a couple of examples:

[Another example about Netflix here](http://select.video/artwork4)

[What happened to Basecamp](http://millions.social/tested7)

[An example with Python](http://math.social/tested3)

[A cool general explanation](http://arts.show/tested7)

So, take one single example in the articles you just read, which specific test/s would you apply? (We want you just to do a draft and think a little bit how to apply the tests you already know in this case)

#Answer

To A/B test the Basecamp Website, I would create another/others, alternative web page that with some new projected features. 
The existing design -- or the "control" -- is Version A. Version B is the "challenger". 
Then, I would test these two versions by showing each of them to a predetermined percentage of site visitors. 

I would evaluate the following variables: 

-Conversion Rate: control the number of people that would fill out the form;
-Bounce Rate: analyse how many visitors would come to the website and bounce out after at most 10 seconds;

Looking at the BaseCamp homepage, I would propose the following changes:

-Change main message to "Manage projects the right way";
-Reduce titles size;
-Reduce explanations to one sentence only.
-Change color for "Give Basecamp a Try" button, and title to "Try Basecamp for free";
-Put the review from NASA as first;
-Reduce number of reviews to 3;
-Put bottom graph right after reviews;
-Insert a link to pricing webpage;
-CREATE A DEMO BUTTON, that would let the user experiment navigation on the software;

For version A and B, with all the changes mentioned above, I would test conversion rate and bounce rate.

## Deliverables
You need to submit a markdown file with the answers to the questions above. You can create a new `.md` file or directly edit the `README.md`.

## Submission
Upon completion, add your deliverables to git. Then commit git and push your branch to the remote.
