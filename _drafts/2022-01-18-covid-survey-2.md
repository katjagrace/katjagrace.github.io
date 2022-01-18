---
layout: post
title: "Tiny covid survey: long covid Part I"
date: 2022-01-17 22:05:00 -0700
tags: CATEGORY-1 CATEGORY-2
comments: true
image:
summary:
---
Here are some more careful results from a survey I ran the other day on Positly, to test whether it's trivial to find people who have had their lives seriously impacted by long covid, and to get a better sense of the distribution of what people mean by things like 'fatigue'.

Respondents are from the US, aged 20-40, and decided to take the survey&mdash;entitled 'Lifestyle 2022' with a longer description mentioning the pandemic&mdash;when offered I think relatively high compensation for doing so, a couple of days ago.



## Loss of productivity, by covid, no covid, long covid


Does long covid show up in the less productivity (which I asked before I brought the topic to covid)

Does the 'working less due to covid' match lower productivity?

How much less productive are long-covid sufferers
How much less worky?

How much less productive are covid sufferers
How much less worky?

How much less productive are non-covid sufferers
How much less worky?

How many people say they work less due to long covid?

Frequency of checkable statements

Readthrough of 'bad cases' to check stories

How much do your ongoing health problems from covid reduce your capacity to do things you would have normally done in a day? Average

Associations with:
- age
- chronic illness


How much are non-vac people isolating?

<!--ex-->

Full guidedtrack.com code for the survey:

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
