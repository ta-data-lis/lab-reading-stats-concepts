<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Lab | Reading About Statistic Concepts

## Challenges

### Challenge 1: What is the difference between expected value and mean?
_You know both concepts but, is there a difference?_
Yes, they are different, but they're also somehow the same. The expected value is a probability concept, while the mean is a value of statistical description.

The mean is an observed value. For instance, to know the mean of goals scored by a team in a football tournament, we must know the results of the matches already. If the team has scored 8 goals in 4 matches, we can say that the mean is 2 goals in each match. However, in the current match, a player from the opposing team has been sent off, so the expected value of goals in that game might increase.

The thing is that with the Law of Large Numbers, if we have enough data we can translate that into a model, and the expected value is actually the mean. 



### Challenge 2: What is the "problem" in science with p-values?
This seems a bit complex, but from what I gather the problem with the p-values is that the "statiscally significance" (or lack of thereof) is dismissing valid scientific research results. According to the Nature article, the problem is mostly in the interpretation of the p-value itself as a measure for validation or legitimacy of the results. A study may not reach a "statistically significant" p-value, but still display important correlations, for instance (they quote some examples).



_If you're into this, take a listen to a couple of episodes of the Hi-Phi Nation podcast, where Barry Lam explores some of the issues of statistical significance [regarding research in Parapsychology](https://hiphination.org/complete-season-one-episodes/episode-6-hackademics-mar-6-2017/) and [psychology](https://hiphination.org/complete-season-one-episodes/episode-7-hackademics-ii-the-hackers/)._


### Challenge 3: Applying testing to a specific case: A/B testing.

Our application has a lot of mini-games. We want people to reach the games that we think are the best but the behaviour is not the expected, they don't reach them.

So we call a designer and after a lot of work he shows us a new design for our application: we will add a button specific for that kind of games inviting the users to click on it:

*Click here to discover cool games!*

We think it will work but can we be sure? So instead of implementing this new button for all users, we implement it for 10% and we compare the results with the users that didn't have it. Is there a significant difference? Is our button working?

So, take one single example in the articles you just read, which specific test/s would you apply? (We want you just to do a draft and think a little bit how to apply the tests you already know in this case)


**The Answer**

Actually, since we're running tests, I'd test out maybe a few buttons instead of only one: playing around with different copytext and positioning can also play a role in the conversion rate (as per the netflix example).

While 10% may not sound like a lot, it may be a significant amount of users (for instance, 10% of the netflix users is nearly 17 million people!).  More than the percentage itself, it seems more important to ensure the samples are the same size and that we consider a certain period of time (maybe a couple of weeks could be enough to test the various buttons?). However, it is agreed that the larger the samples, the most likely it is to have converging results in terms of the relation of the sample with the universe.

(_I'm not gonna dive into the deep maths of this, cause I am still far from understanding everything._)

 I'd try to make sure that the samples across the various hypothesis are similar not only in size, but also in terms of demographics (_ask the data team!_), and aligned with the core target of the app. 

 In terms of actual math tests, we could use χ² test (as suggested by the article about Sephora), using Pearson's theorem (it is quite complex for me, though). And then the Z-test to test those results.

 Finally, we should take into account other factors that maay not be inferred by the data itself. Things like when you run your tests (are the kids mostly at home or at school?), for example.