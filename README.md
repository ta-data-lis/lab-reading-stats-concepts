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

##### my answer
mean is the simple average of numbers, f.e. when you throw a fair six-sided dice 3 times, you take the average of the thre numbers.

expected value is not about the throwed numbers, its 1/6 * the numbers on the side --> taking into account the probability

law of large numbers: the average gets to the expected values when you repeat throwing the dice a lot (=large number)



### Challenge 2: What is the "problem" in science with p-values?
We have told you that a lot of scientifical investigations are based on p-values. The last week, Nature magazine published [an article](http://nature.social/statistical4) regarding the problem. Start digging on it!

Don't hesitate to use more articles if you want to :)

##### my answer
Upon until now a lot of scientist have taken the p-value of 0.05 (5%) as a strict value to decide wheter a result is significant or not: 
- if the p-value was above 5% they declared their results as not significant
- if the p- value was smaller than 5 % they claimed her results to not beeing significant, and sometimes they said, that their is even no relationship.s

A movement of statisticians assess this as too much of black and white thinking. It leads to the risk of deciding wrong or interpreting results of different studies as contradictory,, just because in one study the p-value was above 5% and in the other bellow. In fact, the p-value depends also on the setting of a study (f.e. amount of observation). 

The movement of statistician make four suggestions to improve the discussion about the significancy of results.
  - don't only look at the p-value of 5%, but also at other p-values. 
  - not only indicate significancy with stars (f.e. 3 stars for a p-value bellow 5 %), but add the p-value to a table. 
  - not only discuss about the point estimation you get from a regression, but also about the confidence-intevall: f.e. you can say, that all the values between x and y are compatible.
  - describe and discuss the method, so that others can think about the method and decide, if the setting and the study is compatible for them.
  
My opinion: I like this new trend because at university i saw students / teacher just change their regressions and ideas untlil they got a significant results (at 5%). With that all the "non-significant" results was never discussed or published, although it could have been valuable and important.s




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

So we call a designer and after a lot of work he shows us a new design for our application: we will add a botton specific for that kind of games inviting the users to click on it:

*Click here to discover cool games!*

We think it will work but can we be sure? So instead of implementing this new botton for all users, we implement it for 10% and we compare the results with the users that didn't have it. Is there a significant difference? Is our botton working?

Read more about A/B testing with a couple of examples:

[Another example about Netflix here](http://select.video/artwork4)

[What happened to Basecamp](http://millions.social/tested7)

[An example with Python](http://math.social/tested3)

[A cool general explanation](http://arts.show/tested7)

So, take one single example in the articles you just read, which specific test/s would you apply? (We want you just to do a draft and think a little bit how to apply the tests you already know in this case)


#### my answer
example: my company sells one type of chocolate bars. The boss asked the design department to design a package for this bar, in order to improve the sales number. Befor changing the package, he asked me to test, if customers buy more of the chocloate with the new package. Therefore i will select some stores that sell the bar in the new package. Than i will compare the sale numbers with the previous sale numbers.

H0: sales dont change
H1: sales do change

Sample size:
depends on the number of chocolate bars the stores sold before. 
and the increase in salsenumber we expect / the boss wants to change the package
alpha: 0.5%
statistical power: 80&



## Deliverables
You need to submit a markdown file with the answers to the questions above. You can create a new `.md` file or directly edit the `README.md`.

## Submission
Upon completion, add your deliverables to git. Then commit git and push your branch to the remote.
