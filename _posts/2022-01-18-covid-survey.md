---
layout: post
title: "Positly covid survey: long covid"
date: 2022-01-17 22:05:00 -0700
tags: covid advice
comments: true
image: https://photobucket.com/u/katjasgrace/p/ad7dcf12-e166-4214-a4fa-6e7ff1f4972a
summary: In a small survey, a quarter of covid-infected people seemed to have ongoing problems more than two months after recovery, most of which they say impact their lives a lot.    
---
Here are some more careful results from a [survey](https://worldspiritsockpuppet.com/2022/01/14/preliminary-long-covid-survey.html) I ran the other day on [Positly](https://app.positly.com/), to test whether it's trivial to find people who have had their lives seriously impacted by long covid, and to get a better sense of the distribution of what people mean by things like 'brain fog', in bigger, vaguer, research efforts.<!--ex-->

Respondents are from the US, aged 20-40, and decided to take the survey&mdash;entitled 'Lifestyle 2022' with a longer description mentioning the pandemic&mdash;when offered good compensation for doing so, a couple of days ago.

## Most basic results

- 228 responses
- 56 people thought they have had covid; seven or eight of them on multiple occasions
- 12 had ongoing health problems or symptoms after recovering from acute illness (21% of those infected)

This was the basic long covid question:

>Do you seem to have ongoing health problems or symptoms after recovering from acute covid illness?

In retrospect, it seems misinterpretable, but looking at other responses (see very bottom for all questions, or section 'How bad are these long covid cases' for more details on most of them), I don't think they misinterpreted it much.

## Long covid from cases over two months ago, by vaccination status

The most basic results are not so telling, because maybe all of those people with ongoing problems are among the masses recovering in recent weeks, and will recover from everything before long. So here we'll just look at people who were infected more than two months ago.

Also, let's divide up rates by vaccination status at the time of infection.
<!-- (It's nice to have results for people as close to one's own reference class as possible, so that one doesn't have to make a bunch of iffy adjustments to figure out what to expect.)  -->

Minor details:
- These results are about cases rather than people, i.e. people with two cases are registered twice below (I asked about the date, vaccination status and health consequences for each, so e.g. one person says they got long covid from the second case, so the first is counted under 'no LC').

- 'Vaccinated' = at least a full one or two shot course for two weeks

### Results:

||All	| Vac|	No vac|	(Vac N/A)|
|--|--|--|--|--|
All	| 39|	6|	31|	2|
LC|	9	|2|	7|	0
no LC|	30|	4	|24	|2
P(LC)| 0.23 | 0.33 | 0.23 |

In sum, in this (small) group:
- Around quarter of cases of covid >2 months ago were reported to precede some kind of ongoing health problems or symptoms
- Around a sixth of covid cases happened to people vaccinated at the time
- For vaccinated cases, the rate of long covid was about the same as for unvaccinated

Or to put it visually:

<a href="https://photobucket.com/u/katjasgrace/p/ad7dcf12-e166-4214-a4fa-6e7ff1f4972a" target="_blank"><img src="https://hosting.photobucket.com/images/i/katjasgrace/LCvac.png?width=1920&height=1080&fit=bounds" border="0" alt="LCvac"/></a>

## How bad are these long covid cases?
A thing I wanted to know was how bad these ongoing symptoms are for people. So I asked some more quantitative questions, as well as for open-ended descriptions.

There are only nine cases of long covid from more than two months ago, and I asked people a few different things about them, so it seems easier to tell you their answers than to try to summarize, especially because I think it's helpful to see all of a person's answers together:  

<a href="https://photobucket.com/u/katjasgrace/p/ec1a1890-1e39-4a2b-843d-c8a475232ddc" target="_blank"><img class="full-width" src="https://hosting.photobucket.com/images/i/katjasgrace/Screen_Shot_2022-01-17_at_10.25.31_PM.png?width=1920&height=1080&fit=bounds" border="0" alt="Screen_Shot_2022-01-17_at_10.25.31_PM"/></a>

<a href="https://photobucket.com/u/katjasgrace/p/6c0225a5-5cbf-4dfa-96d3-e352e8f0357c" target="_blank"><img class="full-width" src="https://hosting.photobucket.com/images/i/katjasgrace/Screen_Shot_2022-01-17_at_10.26.00_PM.png?width=1920&height=1080&fit=bounds" border="0" alt="Screen_Shot_2022-01-17_at_10.26.00_PM"/></a>

*(8th column heading ends: "...you were on average in 2019"; for the second column, other options that nobody in this group agreed to were 'I am unable to walk up stairs without resting afterward', and 'A doctor has diagnosed me with having specific organ damage'.)*


Taking answers at face value, about eight of these sound pretty bad to me, just on column Q grounds. However it seems likely that some amount of miscommunication is going on, so I trust more impressions coming from several questions. On that basis, maybe half sound like very likely a big deal to me, holistically (and most of the others plausibly so).


To be maybe continued later...

(Maybe coming up later: What's going on with all these people who don't want to be vaccinated? Are people still taking many precautions? Which ones? What fraction of people's covid-infected acquaintances seem to be severely ongoingly unwell from it? &mdash;I had a lot of prepaid survey-taking minutes from people who didn't have covid with which to satisfy some of my pandemic curiosities.)

---
## Full guidedtrack.com code for this survey

```
*randomize: 1
	*group
		*question: How productive were you this week, relative to your average in 2019?
			More than twice as productive
			About 1.5x as productive
			About as productive
			About three quarters as productive
			Less than half as productive
	*group
		*question: How productive were you this week, as a percentage of average for you in 2019?
			*type: slider
			*after: %
			*max: 200
			*before: For more than 200%, just put 200%
			*save: slidersave
	*group
		*question: Were you much less productive in 2021 than in 2019?
			Yes
			No

*question: Have you had covid?
	Yes
		*set: covid
	No
		*set: nocovid
	Unsure
		*set: unsurecovid

*if: covid
	*question: Have you had covid more than once?
		No
		Yes
			*set: multicovid
		Unsure

	*if: not multicovid
		*question: When did you get covid, roughly?
			*type: calendar

	*if: multicovid
		*question: When did you get covid each time, roughly?
			*type: paragraph

	*question: Were you vaccinated when you got covid?
		No
		Partially
		Yes, I'd had a full 1 or 2 shot course of vaccination for more than two weeks
		Yes, and boosted for more than two weeks
		I've had covid multiple times, and the answer is different for different times

	*question: Do you seem to have ongoing health problems or symptoms after recovering from acute covid illness?
		Yes
			*set: longcovid
		No
		Too soon to say
		*tip: If you have had covid more than once, answer yes if any bout of covid led to ongoing health problems


*if: not covid
	*question: How much are you taking precautions to avoid covid at the moment?
		Not at all
		A little
		Some
		A lot
		Very intensely
		*save: cautionlevelslider

	*question: Where do you think you fit among the population in taking precautions to avoid covid at the moment?
		Among the least cautious 20% of people
		Among the second least cautious 20% of people
		In the middle 20% of people
		Among the second most cautious 20% of people
		Among the most cautious 20%
		*save: cautionlevelslider

	*question: What precautions are you taking lately to avoid covid?
		*type: checkbox
		Avoiding indoor crowds
		Wearing masks indoors
		Wearing masks outdoors
		Reducing time indoors with friends
		Avoiding offices
		Caring for children to keep them from a high exposure setting
		Wearing high quality masks, such as N95, KN95 or P100 masks
		Washing or hand sanitizing extra
		Reducing travel
		Reducing time in stores
		Using rapid tests before spending time together
		Moving activities outdoors

	*question: How many people do you know who had covid at least two months ago and survived?
		*type: number
		*tip: A rough guess is fine.

	*question: How many of them are less than 40 years old?
		*type: number
		*tip: a rough guess is fine

	*question: How many of those people (under 40 years old, survived covid at least two months ago) seem to be having longer term health problems as a result, that probably reduce their productivity by more than 20%?
		*type: number
		*tip: For instance, if your friends Alice (37 years old), Bob (24 years old) and Mary (92 years old) all had covid in 2020, and Alice and Mary have both been too tired to do anything since their infections, then the answer would be '1' (Alice). A rough guess is fine.

	*question: Have you had a covid vaccination?
		Yes
		No
			*set: novax

	*if: novax
		*question: Why haven't you had a covid vaccination?
			*type: paragraph



*if: longcovid
	*question: Which of these things are true for you, as a result of having covid?
		*type: checkbox
		I feel substantially cognitively damaged
		I had no covid symptoms at all, and have had no ongoing covid-related health problems
		I am unable to read things I used to be able to read
		I am unable to walk up stairs without resting afterward
		My life is miserable
		I am markedly less able to think clearly, more than half of the hours of the day
		I had a really bad time for over a month
		I have lingering symptoms, but nothing that makes my life more than 10% worse
		My senses of taste and smell continue to be off
		A doctor has diagnosed me with having specific organ damage
		*tip: If you have had covid more than once, take into account the results of all bouts of covid you have had
	*question: How much do your ongoing health problems from covid reduce your capacity to do things you would have normally done in a day?
		*type: slider
		*after: %

	*if: multicovid
		*question: Which bout(s) of covid led to ongoing health problems for you?
			*type: paragraph
			*tip: e.g. "second", or "both"

	*question: Would you rather:
		A) be rid of ongoing covid related health issues and symptoms forever
			*set: prefcovone
		B) a 10% increase in your income this year
		C) Not applicable

	*if: prefcovone
		*question: Would you rather:
			A) be rid of ongoing covid related health issues and symptoms forever
				*set: prefcovtwo
			B) a 50% increase in your income this year

	*if: prefcovtwo
		*question: Would you rather:
			A) be rid of ongoing covid related health issues and symptoms forever
			B) a 200% increase in your income this year


*question: Are you currently working less as a result of the covid pandemic?
	*type: checkbox
	Yes, because I had covid and it left me with ongoing problems with physical or mental health
	Yes, because of reduced availability of work
	Yes, to avoid covid risks at work
	Yes, to care for others (e.g. children)
	Yes, because of other distractions, burdens or mental health issues stemming from the situation
	Yes, for other reasons
	No, I work as much as usual
	*save: work

*question: Roughly how many fewer hours do you think you are working per week than you were on average in 2019?
	*type: number
	*after: hours
	*tip: e.g. If you used to work about 40 hours per week, and recently work about 35 hours per week, put "5 hours"

*question: Do you have any chronic illness unrelated to covid?
	Yes
	No
	Prefer not to say

*if: covid
	*question: In words, please tell us about the biggest impacts that having covid has had on your life
		*type: paragraph
		*blank
		*tip: Numbers are especially helpful, e.g. 'I probably lose about ten minutes a day to coughing fits', or '20% reduction in my ability to work', or 'I used to run two miles a day, but now I can only manage one'.

*question: In words, please tell us about the biggest impacts that the pandemic has had on your life
	*type: paragraph
	*blank
	*tip: Numbers are especially helpful, e.g. 'I lose about twenty hours a week looking after my children because I can't send them to childcare', or '50% reduction in income, due to lack of available work', or 'I used to go to the gym twice a week, but it has mostly been closed'.


*question: Anything else you'd like to say?
	*type: paragraph
	*blank

Thank you!

*program: EndOfActivityButton
```
Bla
