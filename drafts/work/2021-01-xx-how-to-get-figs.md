---
layout: post
title: "POST TITLE"
date: 2021-01-xx 10:30:00 -0700
tags: CATEGORY-1 CATEGORY-2
comments: true
image:
summary:
---
How do you buy figs from the store?

(How do you go to the supermarket and get figs, as a superintelligent entity? Must you have a utility function? If not, what do you have? How do you not destroy the universe maximizing something?)

- seems related to abstractions that point at the same thing from different places, and abstractions that somehow point at the actual world rather than something in the map
- seems interesting that we can make such things now, but not describe what they are in the terms we want, or something

maybe some kind of satisficing function? where pragmatically, instead of searching over options for the best one, you search for the first one that reaches a certain minimum value.

I guess there are just a lot of action functions, that select actions repeatedly.

being coherent is better than not being coherent, but it's not obviously the only consideration, e.g. it is impossibly hard. But also maybe if you weren't coherent in particular ways, you would be safer in ways for others, and would't especially want to become coherent. (i.e. the value wouldn't be coming from not being coherent, it would be coming from having a different criteria for selection.)

Seems related to question of what to do with magic infinite computation boxes

Plan A: yer basic utility function optimization
- Assume you have large set of possible states of the world, in each consisting of a physics model that can be run forward to answer any question about it probabilistically, and these include versions where you take any action available to you immediately.
- Consider each possible first action, and do the one which has the highest chance of bringing about your buying figs at the store within half an hour and spending less than $20

(what is supposed to happen here? it does some galaxy brained scheme to take over the world so it can be more sure that it buys the figs? Doesn't sound like a more reliable way to get figs. It might do some crazy thing like phone up everyone around and threaten them if they don't bring figs to the store for it to buy, since that materially raises the chance of there being figs to buy, and doesn't take long. You can probably stop that one by also asking that it remain within the law, or remain in good standing, or be approved of. Seems very unlikely that it is worth having an intelligence explosion to better think of ways of maximizing chance of getting figs, but I guess can't rule it out? Is this the actual problem?)

What if you just ask it to do stuff, such that its every move is what current you would approve of after much thought? How does this go badly? Is it just hard to train?

what if you just don't want it to try to do crazy shit at all though? You just want it to go to the store like a simple hoe?

Plan B:
- Assume you have large set of possible states of the world...
- Consider each possible first action, and do the one which is most like what a human would do/choose for you to do if they were trying 'to go to the store and get some figs', and they could see the full consequences that you can see

Plan C:
- ...do the one which gets the figs with more than X% chance and is most likely to be what a human would choose

Plan D:
- ...do one randomly that gets the figs within the constraints with more than X% chance, assuming your future moves are also random like this

This prevents highly contingent plans, e.g. phone Bob and threaten him if he doesn't bring figs to the store, because at each moment, you don't know if you will continue to carry out the weird plan, or move toward another weird plan. Is this different for walking to the store though? Seems like you might be able to distinguish them in that every step you take toward the store does make it easier in the next moment to carry out the objective according to many plans, whereas starting to call Bob in the absence of walking to the store only helps with a small number of plans?
Problem: you can just do crazy shit if you have a bit of spare time. Though you could have a lot of empty actions that you would tend to fall in if you had slack, or tiny steps so that if you have slack you do a random walk.

Plan E:
- ...do one randomly that increases the chance of you getting the figs within the constraints by more than x%, assuming that your future moves are also random like this

this stops you doing crazy shit with your slack, because you don't have any. Your first move should be a thing that is relatively helpful in expectation. Actually not sure, seems like at first maybe nothing scores highly, because you are very likely to succeed anyway if you start later. So maybe you just sit there for a bit. Then at the time it becomes important for your success that you leave, moving toward the store has to happen. So there's a question of whether you can get more added chance earlier via harebrained schemes. ?? Hope is for this to work like the above, but better.

(can we make an unbounded-utility-haver trap? if you think things naturally become coherent, maybe we could trap them with a nice game of st petersburg paradox? I guess they won't go for it if they can just take the universe with high probability.)

Plan F:
- ...make a simplified model of the world that has at least a 50% chance of being right (i.e. abstract away uncertain features). e.g. it says there is a store two blocks North, which is open, and sells figs, and there is sidewalk between you and it, and it is safe...?.
- Select a sequence of actions that gets you the figs in this abstract world [unclear what this means - the abstract world is non-specific]

this seems tricky because how do you make this model, and how do you know if it has the figs in it...

Plan G:
- ... select all strategies (tree-shaped sequences of moves and information reception) that attain figs from store within constraints with at least x% chance
- do one that is most human-like/fastest-and-cheapest(?)/random(not safe now because taking whole path so can do whacky things)/least-affecting-of-things

(but there is uncertainty that is gradually revealed as you go)

what happens if you use criteria A to select from pool to a certain degree of specificity, then criteria B to select among those things? As far as selecting for something you don't want goes?
e.g. if you take all things that make at least one paperclip in expectation, and do the cheapest one?

Seems like these satisficing strategies have no reason to become maximizers.

Seems like if you wanted a certain level of performance, you could choose a higher bar, and still if it was too high, the thing would just not move. But I guess if you just keep doing this, you can find a level where it does the extremal thing it would have done.

Plan H:
- compute current expected cost of
- locate any situation from which getting figs from store would be cheaper

this seems promising, but not fleshed out

Plan I:
- some kind of combination over different utility functions that share 'get figs from store' in common

Plan J:
- some kind of randomly changing utility function at every step, that maintains 'get figs from store' being above average good, and knows that future will be randomized

Plan K:
- find any course of action that does the thing

is there something about the world being so fuzzy that that somehow interacts with utility functions and requires them not to be extremely precise? Just a hazy thought.

Plan L:
- there is a cost on compute, and on time, and on $
- maximize for e.g. 10xfigs - $ spent - time passing in minutes

what is an 'objective'
