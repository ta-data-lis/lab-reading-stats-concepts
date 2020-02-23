# Challenge 1: What is the difference between expected value and mean?
The Expected Value (EV) of a variable is the long-run average of repetitions of the experiment it represents. 

For instance: in a football match, the average probability of a penalty being scored is 72%. Since scoring (Goal) is worth 1 
and not scoring is woth 0, the EV of a penalty is: 

EV = (0.72 * 1) + ((1-0.72) * 0) => EV = 0.72 + (0.28 * 0) => EV = 0.72 + 0 => EV = 0.72.

In a basketball match, since the Average of scoring a 3 point (shooting the ball from behind the 3 points line and getting in), 
the EV of a 3-point  is:

EV = (1.94 * 3) + ((3 - 1.94) * 0) => EV = 5.82 + (1.06 * 0) => EV = 5.82 + 0 => EV = 5.82

In other words, the EV is:

EV = (Chance of desired outcome * result from the desired outcome) + (Chance of undesired outcome * result of the undesired 
outcome). 

Note that 1) you can't score .72 of a goal, nor get 5.82 points from a 3-point shoot (you'll either get a goal or not a goal,
and you'll either get 3 points or 0 points), but 2) if you take a big enough sample of penalties, in the long run, you're 
expected to get a return of 0.72 from a penalty and 5.82 from a 3-point, which is two say you'll score about 3 out of every
4 penalties you take, and make 2 out of 3 3-points shoots you take. #3) Note that while in the case of the penalty in football
the EV equals the average, in the case of a 3-pointer in basket, they do not carry the same value. 

So, the EV is a way to acertain how much you stand to win (or lose), on average, from chosing a particular action, while the 
average is the amount of times a particular outcome arrises from taking a particular action enough times.

Sources:
http://expected.news/value2
https://towardsdatascience.com/the-3-point-statistic-to-rule-them-all-12ac018a955a
Tippett, James: "The Expected Goals Philosophy", 1st Ed 2019, (pages 43-52).

# Challenge 2: What is the "problem" in science with p-values?
There isn't a "problem" in science with p-values. But there is a problem in the way how we, collectively (in science), 
understand them, use them and interpret them. P-values are tools, and as with any tool, you can use them well, wisely, 
appropriately. Or not.

In that sense, there are quite a few. I'll probably (no pun-intended) not mention all, but I'll try to be encompasing. Also, 
they are all somewhat related/built on one another.

First we need to understand (a little?) what P-values are and what are they are for. Then we can see how they can be missused,
or missinterpreted, and maybe even why.

To calculate a P-value we first *assume* that the null distribuition (the frequency distribuition associated to our null 
hypothesis) is the *True distribuition* our *sample* was taken from. Then we calculate how often we'd see a value that is 
*at least* as extreme has our observed value.

So P-values tell us how rare something is. But they do this in a context. They're the probability of getting a sample as or 
more extreme than ours *given* that the null hypothesis is true. 

P-values are then about the *sample* we get in relation to the *population* it was taken from and *assuming* something (that
something being the null hypothesis). They can be used to decide if our hyphotesis are reasonable and to reject or fail to 
reject an idea (more on that latter). And that's it.

The first problem that might arise is that they are not supposed to be interpreted in isolation, but in relation to another
value (alpha), that (hopefully!) has been predetermined as the cut-off point by which we reject or fail to reject the null 
hypothesis. Alpha (asside that it really really must be determined before the experiment/test takes place), is our way of 
saying what we consider to be sufficient evidence to reject or fail to reject the null hypothesis. Therefore someone might
look at an alpha we've chosen and decided if it is a strict enough criteria (or not) for them.

So the first problem is that since those cut off points (alphas) are somewhat arbitrary (for instance: some fields have 
defined a standard alpha of 0.05 while others have defined a standard alpha as only being good enough at 0.01), if you're only
looking only at the P-value, you're ony considering how rare it is that you'd get an extreme result given that sample data,
and not if that rarety is acceptable or not to reject or fail to reject the null hypothesis.

The second problem is that a P-Value only tells how extreme your data would be *if* you *assume* the null hypothesis is true.
But that's not actually what we want to know; we want to know *whether* the null hyphotesis is correct, or at least probably
correct. In other words, the probability of the null *given* that we've seen our data.

We *can't* use P-values (alone) to tell us about the probability of the null hypothesis being true or false. Because P-values
*don't* give us the probability that the null hypothesis is True. When we calculate the P-value we *already assumed* for a 
moment that our null hypothesis *is* true, and that any *sample* difference that we see is actually just due to random 
sampling variation. 

This being the case, using the P-value to express the probability of the null hypothesis being true or false would be like
saying: "Assuming it's raining, what's the probability that it raining?", which wouldn't make much sense.

P-values also cannot tell us the probability that we've made an error *given* that we've rejected the null hypothesis. This is
because P-values are not expressing the probability of the null hypothesis being true or false. 

Quoting Ronald Fish:
"In general, tests of significance are based on hypothetical probabilities calculated from their null hypothesis. They do not
generally lead to any to any probability statements about the real world, but to a rational and well-defined measure of 
reluctance to the acceptance of the hypothesis test."

In other words, they're are not about whether a hypothesis is true or not, but about the probability of getting a result by
random chance given our data (and model).

In yet another way of expressing this: A P-value doesn't give you the probability that the null hypothesis is true; it gives
you the probability of the *data*, *given* the null hypothesis.

As I was saying previously, the probability we want to know is the opposite conditional probability from what the P-value 
gives us. We want to know the probability of the null *given* that we've got this data.

To see this more clearly, think about this: the probability of being a child *given* that you're at a MacDonalds is not the 
same as the probability of being in a MacDonalds given that you're a child:

P(Child | @MacD) != P(@MacD | Child).

The third problem is that, if we're going at it correctly, by rejecting the null hypothesis we still don't have much 
information about the alternative hypothesis. When the data is very improbable under the *null distribuition*, we reject the
null hypothesis and accept the hypothesis that the data came from another distribuition that is not the *null distribuition*.
That's it. This is called the *alternative distribuition* and the hypothesis that goes with it, the alternative hypothesis.
But notice that what's been *accepted* was that the *data* came from a difference *distribuition* from the 
*null distribuition*. That's it. Nothing more. The problem is then that, sometimes, some people, claim more.

For instance: If we reject the *null hypothesis* that I'll submit *all* the labs on time this following week, then the 
alternative hypothesis is that I won't submit all the labs on time this week. But this tells us nothing about if it is one 
lab, two labs, all the labs not to be delivered on time this week. And if the possibility of submiting the labs in advance 
existed (and considered that in advance as being different of being submitted on time), then rejecting the null (all the labs
on time), wouldn't say if was rejected because one or more where late or if it was reject because one or more where early.

So, when the P-value is lower then the alpha, we're *allowed* to reject the *null hypothesis*. Nothing more.

The forth and final problem I'll describe is how to interpret non-significant P-values if our P-value *isn't* lower than our
predetermined cut-off (alpha). In this case we will *fail* to reject the null hypothesis. But *failing to reject the null 
hypothesis doesn't mean accepting the null hypothesis*. They're two different things. It doesn't even mean that the null is 
true; it only means that *we failed to provide evidence that it is false*. That's it.

If, for instance, I failed to provide evidence that a basketball player scored a 3-point, 1) it doesn't mean he didn't, 2) even
if he indeed didn't, it doesn't mean that he didn't score (might a scored a 2-point for instance). All I did was fail to 
provide evidence that he did.

Another way of saying this: I can't go to the sea, fill a bucket of water from it, and in the absence of fish inside the 
bucket conclude that there are no fish in the sea. I can only conclude that there is no fish in the bucket (sample), not in 
the sea (population). "Absence of evidence is not the same as evidence of absence" (I do not know the origin of this quote).

*Failing to reject* the null hypothesis doesn't mean that there isn't an effect or relationship; it just means that we didn't
get enough evidence to say definetly that there is one. That's all. 

The problem arrises when by rejecting the null, one claims more than what one can.

P-values (and alphas) give us insights on how to make (and how we make) decisions about data. If they are used like that, for
that, with their limitations in mind, then they become quite powerful tools in our statistical inferance arsenal. As long as
we don't over-value them and we don't missunderstand what they're able or not to tell us, we'll be alright.

A few quotes from David Spiegelhalter book that can be interesting:

"a 95% confidence interval does not mean there is a 95% probability that this particular interval contains the true value" 
(p. 241)

"a confidence interval is the range of population parameters for which our observed statistic is a plausible consequence"
(p. 241)

p. 257 -> figments of imagination

"(...) a null hypothesis (...) is the simplified form of statistical model that we are going to work with untill we have 
sufficient evidence against it." (p. 258)

"The null hypothesis is what we are willing to assume is the case untill proven otherwise. It is relentlessly negative, denying
all progress and change. But this does not mean that we actually believe the null hyphotesis is literally true (...). So we can
never claim that the null hyphothesis has been actually proved: in the words of (...) Ronald Fisher, 'the null hypothesis is
never proved or established, but it is possibly disproved (...). Every experiment may be said to exist only to give the facts a
chance of disproving the null hypothesis'." (p. 258)

"A P-value is the probability of getting a result at least as extreme as we did, if the null hypothesis (and all other 
modelling assumptions) were really true." (p. 264)

"The idea of statistical significance is straightforward: if a P-value is small enough, then we say the results are 
statistically significant." (p. 265)

"To summarize, I have describe the following steps:

1. Set up a question in terms of a null hyphotesis that we want to check. This is generally given the notation H0.
2. Choose a test statistic that estimates something that, if it turned out to be extreme enough, would lead us to doubt the
null hypothesis (often larger values of the statistic indicate incompatability with the null hypothesis).
3. Generate the sampling distribuition of this test statistic, were the null hyphotesis true.
4. Check whether our observed statistic lies in the tails of this distribuition and summarize this by the P-value: the 
probability, were the null hypothesis true, of observing such an extreme statistic. The P-value is therefore a particular 
tail-area.
5. 'Extreme' has to be defined carefully - if say both large positive and large negative values of the test statistic would 
have been considered incompatible with the null hypothesis, then the P-value has to take this into account.
6. Declare the results satistically significant if the P-value is below some critical threshold." (p. 266-267)

"(...) it is important to emphasize that the exact P-value is conditional not only on the truth of the null hypothesis, but 
also on all other assumptions underlying the statistical model, such as lack of systematic bias, independent observations, and
so on." (p. 267)

The danger of carrying out many significant tests (or the problem of multiple testing), which can be addressed with the 
Bonferroni correction (p. 278-282)

"If a small P-value is observed, then either something very surprising has happened, or the null hypothesis is untrue: the 
smaller the P-value, the more evidence that the null hypothesis might be an inappropriate assumption." (p. 283)

Sources:
https://www.nature.com/articles/d41586-019-00857-9
https://www.youtube.com/watch?v=PPD8lER8ju4
Spiegelhalter, David: "The Art of Statistics", 1st Ed, 2019.

# Challenge 3: Applying testing to a specific case: A/B testing.
—> I don't understand these sentences: "We want people to reach the games that we think are the best but the behaviour is not 
the expected, they don't reach them." (reach the games?)
->  Button, not: "botton".

-> I'm not understanding what is it that is intended for us to do; To say if we'd use the multi-cell explore-exploit test or
a longitudinal test (for instance)?
