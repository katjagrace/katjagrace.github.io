---
layout: post
title: "Calibration of a thousand predictions"
date: 2022-10-12 01:38:00 -0700
tags: experiment prediction
comments: true
image: https://hosting.photobucket.com/images/i/katjasgrace/Calibration_for_no-special-context_forecasts_(mostly_excluding_much_own-behavior_prediction)(1).png
summary: I'm great at predicting things that aren't me, but remain an enigma to myself
---
I've been making predictions in a spreadsheet for the last four years, and I recently got to a thousand resolved predictions. Some observations:

1. I'm surprisingly well calibrated for things that mostly aren't my own behavior[^1]. Here's the calibration curve for 630 resolved predictions in that class:

	<p style="text-align:center;"><img src="https://hosting.photobucket.com/images/i/katjasgrace/Calibration_for_no-special-context_forecasts_(mostly_excluding_much_own-behavior_prediction)(1).png" alt="calibration no context predictions" width="500"/></p>
	
	<!--ex-->

	I don't know what's up with the 80% category, but the average miscalibration of the eleven categories is <3%.

	At risk of bragging, this seems wild to me. My experience of making these predictions is fairly well described as 'pulling a number out of thin air'[^2]. But apparently if you take all these conjured numbers, and look at the 45 of them that fell in the vicinity of 40%, then I implicitly guessed that 17.28 of those events would happen. And in fact 18 of them happened. WTF? Why wasn't it eight of them or thirty-five of them? And that was only the fifth most accurate of the eleven buckets shown above! For predictions in the vicinity of 70%, I was off by 0.15%&mdash;I said 54.88 of those 80 things would happen, and in fact 55 of them happened.

	Possibly people overall are just better calibrated than I thought. I had some remembered view that people's asserted 90% confidence intervals were really 50% confidence intervals or something, but I can't immediately find such evidence now, and I can find various graphs of [groups](https://predictionbook.com/predictions) of [people](https://www.researchgate.net/figure/Color-online-Calibration-Curves-Conditional-on-When-in-the-Questions-Life-the_fig1_320911494) [being](https://goodjudgment.com/wp-content/uploads/2021/10/Superforecasters-A-Decade-of-Stochastic-Dominance.pdf) on average fairly calibrated. And the [handful](https://predictionbook.com/users/Baeboo) [of PredictionBook](https://predictionbook.com/users/Tapetum-Lucidum) [users](https://predictionbook.com/users/gwern) [I could](https://predictionbook.com/users/JoshuaZ) [find](https://predictionbook.com/users/brunoparga) with more than a thousand predictions are not hugely worse.
	
	If you are curious about what I predicted, I put examples at the end of this post.


2. For the entire thousand predictions&mdash;the above plus 370 about my own behavior&mdash; I'm off by 6.25% on average (up from 2.95%) over the same eleven buckets. 


	<p style="text-align:center;"><img src="https://hosting.photobucket.com/images/i/katjasgrace/Calibration_for_all_predictions.png" alt="calibration first 1000 resolved predictions" width="500"/></p>


3. As you may infer, I'm pretty bad overall at predicting my own behavior!

	<p style="text-align:center;"><img src="https://hosting.photobucket.com/images/i/katjasgrace/Calibration_for_forecasts_with_context_(mostly_own-behavior)(1).png" alt="calibration first 1000 resolved predictions" width="500"/></p>
	
	This is more what I expected of a calibration curve&mdash;broadly overconfident. And perhaps its general worseness is explained by the appeal of optimism in predicting oneself. But it's a pretty weird shape, which seems less explicable. If I think there's a 40% chance that I'll do something, apparently it's not happening. If you want it to happen, you should hope I change my mind and put 5% on it! 
		
	I'm not sure what is up with this particular strange shape. But note that making predictions about one's own behavior has particular complication, if one likes to be right. If you put a number below 50% on taking an action, then you have a disincentive to doing it. So you should then put a lower probability on it than you would have, which would make you even more wrong if you took the action, so you have a further disincentive to doing it, etc. I do generally look for a fixed point where given that I put probability *p* on something (and the incentive consequences of that), I do think it will happen with probability *p*. But this is a different process than the usual predicting process, and I could imagine it going wrong in strange ways. For instance, if I'm more motivated by being right than I thought, then 40% predictions which might have been 50% predictions originally should really be 5% predictions. This theory doesn't really work though, because then shouldn't the lower categories also be especially overconfident? Whereas in fact they are okay.

	(Maybe I just have free will? The kind of free will that manifests as being about 15% less likely to do anything than one might have expected seems disappointing, but the menu of possible free will options was never that inspiring.)

## Example predictions

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
	
And some examples of own-behavior marked predictions:

- Work goal as stated will be completed by end of day: start a document of feedback policies: 0.90 (true)
- I ok [person]'s post before the meeting: 0.68 (false)
- Work goal as stated, will be completed by Sunday 28th October: Respond to [person]: 0.80 (true)
- Work goal as stated will be completed by midnight Sunday 30 September 2018: read [person]'s research: 0.4 (false)
- Work goal as stated, will be completed by Sunday 4th November: Arrange to talk to [other researcher] about [employee] project [...]: 0.3 (false)
- Work goal as stated will be completed by midnight Sunday 30 September 2018: Think for 1h about [colleague] thing: 0.5 (true)
- I have fewer than 1k emails in inbox at some point on Feb 10th: 0.87 (true)
- I have written to [brother] by Feb 10th: 0.82 (true)
- I will be home by 9pm: 0.97 (true)

Categories missing from these randomishly selected lists but notable in being particularly fun:
1. Predictions of history that I don't know or remember, followed by looking it up on Wikipedia. A pretty fun combination of predicting things and reading Wikipedia.
2. Predictions of relationship persistence in successive episodes of *Married at First Sight*.

<br>
<br>
---
## Notes

[^1]: I have a column where I write context on some predictions, which is usually that they are my own work goal, or otherwise a prediction about how I will behave. This graph excludes those, but keeps in some own-behavior prediction which I didn't flag for whatever reason.)

[^2]: Except maybe more like art&mdash;do you know that feeling where you look at the sketch, and tilt your head from side to side, and say 'no, a little bit more... just there....mmm...yes...'? It's like that: '27%...no, a little more, 29%? No, 33%. 33%, yes.' Except honestly it's more ridiculous than that, because my brain often seems to have views about which particular digits should be involved. So it's like, '23%...no, but mmm 3...33%, yes.' I am generally in favor of question decomposition and outside views and all that, but to be clear, that's not what I'm doing here. I might have been sometimes, but these are usually fast intuitive judgments. 

