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

The expected value is the average of the outcomes when repeatedly repeating the procedure. The expected value is functionally associated to distribution with a given parameter, a distribution that can further generate samples with different sample averages. Therefore I do not think they synonims, but they are related since the expected value takes a sample of the distribution that we know the mean of.

### Challenge 2: What is the "problem" in science with p-values?
We have told you that a lot of scientifical investigations are based on p-values. The last week, Nature magazine published [an article](http://nature.social/statistical4) regarding the problem. Start digging on it!

Firstly, in statistics we cannot conclude that some p value obtained within a confidence interval proves that we should accept or reject a certain null hypothesis with 100% accuracy, therefore we can't conclude that there is no difference based on this p value. If we compare two scientific studies that have different p values(one higher and one lower) they might not be in conflict with each other and people still assume that they are non signficant. There is a lot of articles that are misinterpreting in terms of their significance or effect. Furthermore, we should not use p values to decide weather a scientific hipothesis is true of false only based on this criteria. Instead, additional methods of analysis decision should be used. Yet people tend to categorize a singificant result and a non significant result. A good way to solve this problem is to rename confidence interval levels according to each study in a particular and embrace the fact that there will always be an uncertainty associated to any statistical result. 


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

So we call a designer and after a lot of work he shows us a new design for our application: we will add a button specific for that king of games inviting the users to click on it:

*Click here to discover cool games!*

We think it will work but can we be sure? So instead of implementing this new button for all users, we implement it for 10% and we compare the results with the users that didn't have it. Is there a significant difference? Is our botton working?

Read more about A/B testing with a couple of examples:

[Another example about Netflix here](http://select.video/artwork4)

[What happened to Basecamp](http://millions.social/tested7)

[An example with Python](http://math.social/tested3)

[A cool general explanation](http://arts.show/tested7)

So, take one single example in the articles you just read, which specific test/s would you apply? (We want you just to do a draft and think a little bit how to apply the tests you already know in this case)

I picked the first example fo Netflix which aims to give users a better experience based on what they've watched. The goal of the test done aims to identify artwork that enabled members to find a story they wanted to watch faster.

They have tried to address all of these limitations in the design for a new “title level explore test”. In this experiment, all members of the explore population are in a single cell and dynamically assigned an artwork variant for every (member, title) pair just before the title gets shown to the member. Therefore, an A/B test was perform for every title with a cell for each artwork. 

In order to perform an A/B test I would follow these steps: 

1. Pick a variable to test
2. Identify my goal
3. Split my samples in groups and choose sample size
4. Define how singificant the results have to be and appropriate confidence interval
5. Choose specific test to use. 
6. For this case, I would choose an ANOVA test and a t student independent test.

ANOVA (or ANalysis Of VAriance) is a technique meant to compare the means of three or more independent samples. An example of when we might use ANOVA is when conducting a test on an e-commerce website and trying out multiple UI designs at once to see if there is a change in sales. With the ANOVA, we compare the difference in variation between the groups and the difference in variation within the groups themselves. If the F statistic is sufficiently large, this means the p-value will be sufficiently small. This will lead us to reject the null hypothesis and conclude that there is significant variation between the groups and therefore at least one of the means is different.

The independent t-test, also called the two sample t-test, independent-samples t-test or student's t-test, is an inferential statistical test that determines whether there is a statistically significant difference between the means in two unrelated groups.

By analysing difference between means and variances I beleive we can have a more robust analysis and in this case draw the best and accurate conclusions.

## Deliverables
You need to submit a markdown file with the answers to the questions above. You can create a new `.md` file or directly edit the `README.md`.

## Submission
Upon completion, add your deliverables to git. Then commit git and push your branch to the remote.
