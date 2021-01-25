---
layout: post
title: "Tentative covid surface risk estimates"
date: 2021-01-25 01:25:00 -0700
tags: covid botec
comments: true
image:
summary:
---
My household previously made some highly uncertain estimates of the covid risk from bringing random objects that other people have recently been touching into our home, for instance salads and groceries an endless stream of Amazon packages. The official guidance is very vague, e.g. ["...not thought to be the main way the virus spreads"](https://www.cdc.gov/coronavirus/2019-ncov/faq.html). Our bad estimates were fairly low, so we decided to basically ignore it in our covid risk accounting, except for habitually taking some reasonable precautions.

Then the covid rates here increased by a factor of ten, so we decided it would be good to look at it again.

So today I tried to estimate this from [this paper](https://www.medrxiv.org/content/medrxiv/early/2020/11/01/2020.10.27.20220905.full.pdf) (HT Ben Weinstein-Raun and Catherine Olsson) in which a group of researchers swabbed various door handles and trash cans and crosswalk buttons and the like in a small Massachusetts city and measured the covid RNA detectable on them. They also used the amounts they measured to estimate the infectiousness if someone else were to touch the surface and then touch their face.

[Here](https://www.getguesstimate.com/models/17305) I offer you a draft of an elaborate Guesstimate spreadsheet on the topic, in case you are interested in such things. Hopefully someone is, and will tell me ways that it is wrong, then later I might offer you something reliable. At present, it is probably pretty unreliable, and should only be used insofar as you would otherwise use something even more unreliable. Some non-exhaustive evidence of its unreliableness:
- I haven't actually read much of the paper
- The answers in the spreadsheet have changed substantially while I have felt about as confident in them as I do now
- There are numerous places where it seems dubious to me, or where I made up numbers
- I try not to be the sort of person who only shares things if they are of high quality, even if the stakes are high
- This calculation is ignoring the efforts everyone is making to be safe, so you might underestimate the risks if surfaces look low risk in this study because supermarket employees are actually constantly wiping them down, for instance. So it should probably be interpreted more like 'if you take levels of caution similar to those taken with the study surfaces...'.

Interesting tentative conclusions so far, rely upon at own risk:
- a person with covid touching something then you touching it then touching your face is worth extremely roughly 13 [microcovids](https://www.microcovid.org/?distance=sixFt&duration=136&interaction=oneTime&personCount=20&riskProfile=average&setting=plane&subLocation=US_06075&theirMask=basic&topLocation=US_06&voice=silent&yourMask=n95) (uCov) (with 90% confidence of 0.7 to 110 according to my estimate, but I wouldn't trust that)
- thus such a touch-touch-face sequence with a random person in San Francisco (where I live) at the moment is ~0.7 uCov (give or take an order of magnitude)
- adding further wild guesses about how many touches are involved in acquiring groceries, I get that a 30 item San Francisco grocery trip is worth about 5 uCov (give or take an order of magnitude)
- that would mean about two cases from groceries in San Francisco per week, (give or take an order of magnitude) which doesn't sound crazy to me. (You might think it does sound crazy, because surely we would notice that by now, but I'm pretty uncertain about our collective ability to observe and infer things.)

The basic reasoning is this:
- If an infected person touches a surface, it looks like it has about a 13% chance of becoming detectably infectious by this method (based on 36 samples from grocery store surfaces which are estimated by me to receive very roughly 2 covid-infected touches per day yielding 4 positive samples, along with some complication with distributions that make the arithmetic strange.)
- Average risk from touching one of these positive-testing surfaces is very roughly 100 microcovids (taking an estimate half way between the average grocery surface infectiousness and the average surface infectiousness, according to the paper)
- So if a person with covid touches a surface, then you touch it and then touch your face, this gives us about 13% of 100 microcovids = 13 microcovids (.0013% chance of covid)

I welcome all kinds of comments, e.g. even 'I want to know why this cell says 27, but I can't be bothered reading all these things'.
