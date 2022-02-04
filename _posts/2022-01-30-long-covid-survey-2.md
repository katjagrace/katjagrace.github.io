---
layout: post
title: "Positly covid survey 2: controlled productivity data"
date: 2022-02-03 23:20:00 -0700
tags: covid survey
comments: true
image: https://photobucket.com/u/katjasgrace/p/ad7dcf12-e166-4214-a4fa-6e7ff1f4972a
summary:
---
*(This continues data from the survey I did the other day on Positly (some other bits [here](https://worldspiritsockpuppet.com/2022/01/14/preliminary-long-covid-survey.html) and [here](https://worldspiritsockpuppet.com/2022/01/18/covid-survey.html).)*

Before asking everyone whether they had had covid, or have ongoing problems from it, or anything else, I asked them about their recent productivity relative to 2019. I was hoping to minimize the influence of their narratives about their covid situation and how it should affect their productivity on their productivity estimates.

The clearest takeaway, I think: people who would later report ongoing post-covid symptoms also reported being way less productive on average than people who didn't report any covid.

 <!-- tell from this data whether people who had covid were overall less productive - this data alone seems consistent with covid-infected people having a similar range of outcomes, but reporting long covid when the outcomes are bad, or covid somehow improving people's productivity. -->

<!--ex-->

<!-- The first question of the survey was about how productive people were lately relative to their 2019 productivity.  -->
Perhaps stupidly, I asked people about their productivity in one of three randomly selected ways, to better tell if results were sensitive to misunderstandings, wording or other vagaries of survey taking. While I stand by this for higher commitment surveys, here it meant trying to aggregate a bunch of slightly mismatched claims about how unproductive a year people are having, when I could have just been averaging a column of numbers. And people did give different-looking distributions of answers for different questions, and different numbers of people with covid got randomized into different kinds of questions, so combining them is messy.

The different questions were these:
1. How productive were you this week, relative to your average in 2019?
    - More than twice as productive
    - About 1.5x as productive
    - About as productive
    - About three quarters as productive
    - Less than half as productive


2. How productive were you this week, as a percentage of average for you in 2019?

    (slider: 0-200%; instruction: For more than 200%, just put 200%)


3. Were you much less productive in 2021 than in 2019?
    - Yes
    - No


Below are the answers, divided up by question type. Note that the numbers of respondents involved are tiny and things are noisy. For example, the category question only got two long covid sufferers, and one of them was the nurse apparently working 200% as much as in 2019 but fatigued to the point of crashing her car. (In general, productivity varying because of demand as well as supply is an obvious-in-retrospect theme, according to my reading of the long answers to later questions.)

|  |  0-200% slider (average %) | Not 'much less' productive (fraction of people) | Category choice (average 1st-5th option, higher more productive) |
|--|--|--|--|
|**Productivity of demographic** | | | |
|All respondents	|106% |48% | 3.15 |
|No covid	| 108% | 54% |3.09 |
|Covid	|100% | 31% | 3.28 |
|Covid & not long covid	| 109% | 29% | 3.26 |
|Long covid	| 70% | 33% | 3.50 |
| **n in demographic** |  |  |  |
| Total n |  85 | 54 | 89 |
| Covid n |  18 | 13 |25 |
| Long covid n |  4 | 6 | 2 |

(Probably I should have given you the 'people who had covid more than two months ago' numbers, but I didn't and I'm short on time for this, sorry! All the data is available at the end.)
<!-- |if no LC	|115 | 108 |50 | -->

It would be nice to combine all these answers. A natural way to do it might be to assign plausible seeming numerical values to all the answers to 1 and 3 , then average all these values.


<!-- Maybe that explains why for the category choice question, having covid makes you substantially more productive than not having covid, and why only one of the three questions returned the answer that if you have covid, it's worse to also have long covid? Not sure.  -->


For instance, let's use the following conversion:

Question 1
- More than twice as productive: 200%
- About 1.5x as productive: 150%
- About as productive: 100%
- About three quarters as productive: 75%
- Less than half as productive: 50%

Question 3
- Yes (i.e. much less productive): 80%
- No: 100%

<!-- I expect this could be done better, but I am already spending too long on it. I didn't mess around with these to get more desirable answers. The only thing I fiddled with was changing 'No' to question 3 from 120% to 100%, because after a little more thought it seemed more reasonable as a guess for how productive a person is if they say they aren't way less productive. -->

With these we get:

|Respondents | Average productivity relative to 2019* | n |
|--|--|--|
|All |	106%| 228 |
|Covid |	106%| 56 |
|Long covid|	89%| 12 |
|Covid & not LC |	110%| 44 |
|No covid|	106%| 172 |
||**According to above described questionable quantification procedure (for those of you skipping to the table)*||

<!-- We can possibly make this slightly better by supposing that the different groups should have had the same average, and dividing everything by the average productivity for that question:

|Respondents | Productivity relative to 2019* | n |
|--|--|--|
|All |	106%| 228 |
|Covid |	106%| 56 |
|Long covid|	89%| 12 |
|Covid & not LC |	110%| 44 |
|No covid|	106%| 172 | -->

A different thing to do is call everything below 80% 'much less productive' then convert everything into fraction of people avoiding that fate:

|Demographic | P(not much less productive) | n |
|--|--|--|
|All |	68% | 228 |
|Covid |	64%| 56 |
|Long covid|	25%| 12 |
|Covid & not LC |	75%| 44 |
|No covid|	69%| 172 |

The 'covid & not LC' category is notably more productive than the 'no covid' category in both combinings, which seems interesting. Some things that might be going on:
- Covid is overall negligibly bad for productivity, and the quarter of people whose lives would have gotten worse lately anyway classify it as 'long covid', leaving the other covid sufferers unusually productive. (This being the main thing going on seems inconsistent with other evidence to me, but maybe there's some of that, or maybe my understanding of the other evidence is mistaken.)
- People who get long covid are disproportionately those whose productivities were on a less uphill trajectory.
- People who get covid and not long covid have a relatively productive time because they are freed from avoiding covid, whereas people without covid are often paying costs that are a large fraction of the cost of having covid to avoid it.
- Maybe people's sense of their own productivity is higher when they had reason that it might be low.
- Maybe people with covid but no ongoing problems are disproportionately in households with other people who have some kind of problem from covid (including for instance having died, or having lost income from a brief illness), and capable of helping, and so are being more productive by necessity.
- This data is so meagre and messy that reading anything into it that's not about a huge effect is a mistake, and this is already too much thought on the topic.

I tend to think it's the latter, but if anyone wants to actually do statistics, or anything else with this data:

[Data](https://docs.google.com/spreadsheets/d/1RcGe3ZiizCkSnCPtLE7UiYQr7TdNTxF1kdJpoWM8j-A/edit?usp=sharing)

<!-- , but I'm just saying the data here seems to suggest it. Though not that strongly I think, because all of this is so noisy that even if that was the story I wouldn't expect it to line up that nicely.) -->

<!-- It's interesting that covid and no covid come out the same here, in spite of huge variation in general, and covid being comprised one quarter by long covid sufferers who are 15% less productive. In particular, it isn't just that the 'covid' category is full of people who don't have long covid, bringing it up to normal. The people who don't report long covid are actually claiming to be more productive than people without covid at all, and what's more, exactly enough more to make up for how unproductive the long covid sufferers are.

xxx[but this isn't even right, because the covid should be >2mo old, which makes covid even better, so no more the coincidence]

These two things&mdash;that the non-LC folks are more productive, and that they are exactly the balancing amount more productive&mdash;point at a story where covid is negligibly bad for people, and the quarter of people whose lives would have gotten worse lately anyway classify it as 'long covid'. (This sounds fairly implausible to me for other reasons, but I'm just saying the data here seems to suggest it. Though not that strongly I think, because all of this is so noisy that even if that was the story I wouldn't expect it to line up that nicely.)

Is that what's going on? Some other things that might be going on:
- The bizarro question where the more covid you have the better has disproportionately many covid-havers randomized into it, and disproportionately few long-covid-havers. It also has substantially higher average numbers. Supposing the higher numbers for that question are an artifact of the question somehow, this increases the apparent productivity of people who had covid but not long covid. xxx

Maybe looking at the data separately first will help.



However this seems like a coincidence of the numbers I chose, which doesn't show up otherwise (xxx check). We can tell these numbers are bad, because they lead to very different average productivities based on which category you are randomized into. (Though possibly there is no way to rectify this.)

Note that two of the kinds of questions find that no covid is better than covid. Though only one of the three finds that no long covid is better than long covid. The category choice column is pretty weird, getting both of these counterintuitive answers. It also has an unusually high rate of covid cases and low rate of long covid cases, and generally very high productivity numbers. So probably this is just making people with covid and no long covid look extra productive.

On second thought, I think combining them may be too hard to do well.

but my first attempt to quickly correct for this error still has the pattern, so that's interesting.

<!-- A different thing to do:

|Situation per later answers | P(not much less productive) | n |
|--|--|--|
|All |	68% | 228 |
|Covid |	64%| 56 |
|Long covid|	25%| 12 |
|Covid & not LC |	75%| 44 |
|No covid|	69%| 172 | -->

<!-- This thing where people who had covid and didn't have long covid are more productive than people without covid seems at least a bit consistent, and is interesting. One hypothesis it suggests is that some amount of badness that would happen anyway is being counted as long covid.




(Note that I didn't remove the nurse who was at 200% productivity and attributed crashing her car to fatigue, though that seems like an example that shouldn't really be bringing the average expected outcome of long covid up a lot.)

Note that productivity is a weird thing to measure, and that the data seems to include various people whose productivity is being impacted by the need for productivity rather than the ease of it: the twice-infected nurse who says she has long covid but also that she is twice as productive as in 2019 (though does attribute a recent car crash to fatigue). People become sole supporters of families when their partners get sick or lose jobs, workplaces become short staffed, people need to look after children on top of whatever of their usual responsibilities can be salvaged. Glancing through the longer answers for people with covid who are more productive, I don't know what's going on. xxx[true?] Glancing through the longer answers for people with long covid who are less productive, it's also not always super clear what's going on, but a fair bit seems to have the straightforward narrative you might expect.  -->
