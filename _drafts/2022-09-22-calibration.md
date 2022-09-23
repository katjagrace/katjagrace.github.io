---
layout: post
title: "Calibration of a thousand predictions"
date: 2022-09-22 01:30:00 -0700
tags: CATEGORY-1 CATEGORY-2
comments: true
image:
summary:
---
I've been making predictions in a spreadsheet for the last four years, and I just got to a thousand resolved predictions. Some observations:

1. I'm shockingly well calibrated for things that mostly aren't my own behavior[^1]. Calibration curve for 630 resolved predictions in that class:

	<p style="text-align:center;"><img src="https://hosting.photobucket.com/images/i/katjasgrace/Calibration_for_no-special-context_forecasts_(mostly_excluding_much_own-behavior_prediction)(1).png" alt="calibration no context predictions" width="500"/></p>

	The 80% category is abberantly bad&mdash;off by about 12%&mdash;but the average miscalibration of the 11 categories is <3%.

	At definite risk of bragging, this seems wild to me. My experience of making these predictions is fairly well described as 'pulling a number out of thin air'. But if you take all these conjured numbers, and look at the 45 of them that fell in the vicinity of 40%, then I implicitly predicted that 17.28 of those events would happen. And in fact 18 of them happened. WTF? Why wasn't it eight of them or thirty-five of them? And that was the fifth most accurate bucket. For predictions in the vicinity of 70%, I was off by 0.15%&mdash;I said 54.88 of those 80 things would happen, and in fact 55 of them happened.

	Possibly people overall are just better calibrated than I thought. I had some remembered view that people's asserted 90% confidence intervals were really 50% confidence intervals or something, but I can't immediately find such evidence now, and I can find various graphs of [groups](https://predictionbook.com/predictions) of [people](https://www.researchgate.net/figure/Color-online-Calibration-Curves-Conditional-on-When-in-the-Questions-Life-the_fig1_320911494) [being](https://goodjudgment.com/wp-content/uploads/2021/10/Superforecasters-A-Decade-of-Stochastic-Dominance.pdf) on average fairly calibrated. And the [handful](https://predictionbook.com/users/Baeboo) [of PredictionBook](https://predictionbook.com/users/Tapetum-Lucidum) [users](https://predictionbook.com/users/gwern) [I could](https://predictionbook.com/users/JoshuaZ) [find](https://predictionbook.com/users/brunoparga) with more than a thousand predictions are not hugely worse.


Except maybe more like art&mdash;do you know that feeling where you look at the sketch, and tilt your head from side to side, and say 'no, a little bit more... just there....mmm...yes...'? It's like that: '27%...no, a little more, 29%? No, 33%. 33%, yes.' Except honestly it's more ridiculous than that, because my brain often seems to have views about which particular digits should be involved. So it's like, '23%...no, but mmm 3...33%, yes.' I am generally in favor of question decomposition and outside views and all that, but that's not what I'm doing here. I might have been sometimes, but these are usually fast intuitive judgments iirc. So imagine if you just sort of artistically made up numbers like that for years, with no introspective assurance that they were particularly good, and then they actually matched what happened! WTF? What magic is this? Also, aren't humans basically guaranteed to give 90% confidence intervals that should have been 50% confidence intervals or something? Did you accidentally sell your soul to the devil for this on some occasion that you have conveniently forgotten about?

Or more precisely: say 45 of those made up numbers fall between 35% and 45%, and those ones average 38.41%. Which is to say, I predicted that 17.28 of events in that bucket would happen, and then in fact 18 (40%) of them happened. And this example isn't even the closest. 




One might object to this being interesting by noting that calibration isn't hard in principle. For instance, if you want to be well calibrated, you can always make predictions about dice rolls, or otherwise strategize to coax predictably distributed randomness into right sized boxes (e.g. assign your statements randomly to P or -P and always predict 50% on P to be calibrated at 50%, and only make 75% predictions on statements of the form 'P or Q', etc). I don't think that's relevant here, because I didn't do anything like that. For instance, I didn't (that I recall) choose a proposition to predict on the basis that it would be easier to be calibrated on it. The closest things I do are try to adjust for my known miscalibration (e.g. if I want to say 80% on a thing, maybe I should say 70% if that is empirically what it has meant when I've said 80% before) and considering the opposites of statements (e.g. if I want to say 50% on A, check whether I really think 50% on not-A also). These seem like above-board ways to improve one's calibration, because they can be applied across the board in making predictions about other things, and so represent genuine better calibration. 

Here are some typical predictions, arbitrarily pulled from my spreadsheet and lightly edited:

- I will be invited to play ONUW today: 0.45 (true)
- The trial bank transfers come through to my IBKR account by the end of Monday: 0.34 (false)
- [Friend] will want to leave here for the day before I do: 0.05 (false)
- [Friend] will seem notably sad in demeanor when I talk to [them]: 0.6 (false)
- I will be paid by end Jan 27: 0.85 (true)
- If I go inside shortly I see [friend]: 0.08 (false)
- We have the [organization] party here: 0.55 (true)
- I go to math party today: 0.88 (true)
- I will get my period on Tuesday: 0.10 (true)
- We will be invited to work at [office] for at least a week: 0.75 (false)
- On Feb 5 we (including [friend], me, [friend]) are renting a new place: 0.73 (true)
- We will run the arts and crafts room auction today (i.e. by midnight we will have as much info from the auction as we will get re which room is whos, ignoring processing of info we have): 0.40 (true)
- [Person] is leading a new EAish org or CEO or COO of an existing EAish org by May 30 2023, where EAish includes orgs not culturally EA but doing things that are considered so by a decent fraction of EAs: 0.62 (TBD)
- I will get to the office in time for lunch: 0.95 (true)
- I see [housemate] tonight before midnight: 0.88 (true)
- If I ask [attendee] 'what did you think of [event I ran]?', [they] will be strongly positive: 0.8 (false)
- I see [friend]'s dad tonight before midnight: 0.95 (forgot to notice)
- If I offer [person] a trial [they] will take it: 0.65 (true)
- If I look at [friend]'s most recent Tweet, it is linking to [their] blog: 0.8 (false)
- My weight is under [number] again before it is over [number] again: 0.75 (false)
- I do all of my Complice goals tomorrow: 0.3 (false)
- I will go to the office on Friday: 0.6 (true)
- I will read the relevant chapter of Yuval book by the end of 2nd: 0.1 (false)
- I weigh less than [weight] the first time I weigh myself tomorrow: 0.65 (true)
- Lunch includes no kind of fish meat: 0.43 (true)


<!--ex-->

3. I'm off by about xxx% on average for the entire 1000 predictions. I haven't constructed the graph of just my own behavior, but it seems like I must be pretty bad at predicting it. Maybe I have free will? The kind of free will that manifests as consistently being about 20% less likely to do anything you think you're going to do than expected seems disappointing, but the menu of possible free will options was always a little disappointing.

Here are some examples of own-behavior marked predictions:
- Work goal as stated will be completed by end of day: start a document of feedback policies: 0.90 (true)
- I ok [person]'s post before the meeting: 0.68 (false)
- Work goal as stated, will be completed by Sunday 28th October: Respond to [person]: 0.80 (true)
- Work goal as stated will be completed by midnight Sunday 30 September 2018: read [person]'s research: 0.4 (false)
- Work goal as stated, will be completed by Sunday 4th November: Arrange to talk to [other researcher] about [employee] project (0.25): 0.3 (false)
- Work goal as stated will be completed by midnight Sunday 30 September 2018: Think for 1h about Anthony Aguirre thing: 0.5 (true)
- I have fewer than 1k emails in inbox at some point on Feb 10th: 0.87 (true)
- I have written to [brother] by Feb 10th: 0.82 (true)
- I will be home by 9pm: 0.97 (true)




3.

And I think calibration measured on more arbitrary events (i.e. not those chosen to make calibration easy) is important: it is genuinely useful to know if when Alice says a thing is 90% likely, how often 90% of the time.

(Not represented in the above list: I recently got into predicting history that I don't know or remember then looking it up on Wikipedia. This is a pretty fun combination of predicting things and reading Wikipedia IMO.)


[^1]: I have a column where I write context on some predictions, which is usually that they are my own work goal, or otherwise a prediction about how I will behave. This graph excludes those, but keeps in some own-behavior prediction which I didn't flag for whatever reason.)

---
To probably cut: 

I realize bragging is heuristically bad, but it seems important on topics like this, where otherwise people might make dangerous mistakes on who they listen to. My physical voice is fairly quiet, and I'm a friendly and conflic-avoidant woman, so the thought that people should listen to me often seems to be counter-intuitive. But for the record, I am very unusually good at being correct.

Or perhaps this is a normal level of calibration? I had the cached understanding that people are generally terribly calibrated, and if you ask them for a 90% confidence interval, it should have been a 40% confidence interval or something. But looking into this now, i don't immediately find much, and the 