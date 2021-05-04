---
layout: post
title: "POST TITLE"
date: 2021-01-xx 10:30:00 -0700
tags: CATEGORY-1 CATEGORY-2
comments: true
image:
summary:
---

Is it true that a utility maximizer with preferences over entire universe histories is unconstrained in its behavior, or especially non-agentic?

[neither: there are probabilistic constraints, where it will probably look agentic unless it is randomly created in exactly the right universe, and so yes it is probably agentic]

What does an agent with this entire universe-history utility function look like?

Seems like if it has long chunks, but not entire universe, enough that it has any time to get resources for a future round, then it looks goal directed again.

If it is over actually entire universes, and there is no sub-level order to its preferences, then it des need to act a certain way at each point to not fall off the wagon.

But actually it is unclear even then that it doesn't try to gather resources. Because if it wants to bring about entire universe histories over others, it's probably worth sacrificing some losses in potential for ideal ones (even if right now it is going well, in order to exercise future control)

e.g. suppose that you want the history 1101001110101000, and so far you have got 110. At each time step, you can spend for a 1 or a 0, which makes it twice as likely per dollar as the other outcome, but you are always paid an extra dollar when you vote 0. Let's say that you value other histories less insofar as they diverge from this one.

(this is actually basically having a simple break-downable utility function again, where you value the 'right' digit each time, and the situation changes regarding the costs of choosing the one you like. Is everything actually like that? What isn't? What is 'likee that?' I have the impression that there is something like caring holistically, where you can't usefully reason about the parts. What is that like?)

Then supposing that at each point the outcome is random, you ...

This is all to say that even the agent that prefers an extremely obscure sequence of holistic outcomes, and in general has preferences over entire histories, will be goal-directed in the sense of grabby, almost all of the time. (They might in fact not have options sufficiently worth losing early bits to to get, but so it is with any goal-directed thing.)

How do you get a non-grabby one? The one that isn't grabby because it prefers the universe as it is is only got by extreme luck, under this kind of scenario. If you had that same one, in a different world, it would be grabby. But it is true for every agent that there is some world where it isn't grabby because the passive option is always the one with highest expected utility. This isn't even specific to this universe-history agent. Passivity could be got more robustly by referencing things in a different way. e.g. 'I prefer whatever happens'. But that isn't going to be useful at all.

Can we actually *make* an agent that is coherent, not goal directed, and has non-trivial behavior?


If it has preferences over sequences of world-states, the ways for it to not be grabby seem to be:

- the world is exactly as it prefers, and it knows it
- it believes that the world will be as it prefers if it takes various non-grabby seeming actions (though this is kind of like it being agentic but us organizing its options such that it doesn't behave so)
- it doesn't have any opportunities to cause the world to be as it prefers
- ??

It could also have preferences that are over its actions, rather than states of the world. e.g. it prefers to output the square of the number that is input.

My guess is that anything non-trivially useful, and preference-maximizing, and having undergone substantial pressure to be coherent, will be goal-directed

***

new post: Seems like re Ngo's post, can also have intermediate scale preferences. e.g. want the pattern 'abab' to occur, vs wanting a or wanting entire trajectory.

***

new post: Should we expect AI to be coherent with respect to trajectories, or single moments?

[ngo post]

Ngo:
>So even if definition 1 [preferences over momentary states] turns out to be a useful one, it would take additional arguments to show that we should expect that sort of coherence from advanced AIs, rather than (trivial) coherence with respect to trajectories. I'm not aware of any compelling arguments along those lines.

Seems to me that AIs having trivial coherence re trajectories is very unlikely.

e.g. there is maybe no pressure pushing them there

e.g. let's say they sometimes choose 2a over 40b, and sometimes choose 15b over a, and as a result have chosen 'aabba' so far. They notice this inconsistency, and worry that it causes them to have less total a or less total b ultimately, which they are some amount inclined toward. Given their pseudo-preferences for a and b, there is no reason they would change to prefer 'aabba..'' versus changing to prefer 'a' more than they do in the '15b vs a' cases, which will get them more a and/or b ultimately.

pseudocode:
1. AI behavior: when given choice, take 'better' option. Evaluations: a > 0, a > b, a > 2b, a > 3b, a < 4b, 2a > 0, 2a > b, 2a > 2b, 2a > 2b, 2a < 4b, 0 < b < 2b < 3b < 4b (or, a options are better than b options if b<4)
2. AI chooses a > 0, a > 3b, a > 3b, 4b > 2a, and thus has 3a+4b.
3. AI notes that it could have had 3a + 6b by making a different series of choices, from the same ones presented to it
4. AI notes that if facing these choices again, doing the same thing again vs making the alternate set of moves is a choice of 2b vs. 0. Since 2b < 0, it chooses to alter its preferences to make the set of choices that corresponds to +2b, at least during the next time it is in exactly this situation. Considering other future situations it might encounter, it makes similar observations. In fact in any sequence of actions where it might have acted incoherently, it finds that not adjusting the actions to make them coherent amounts to prefering 0 over some number of either a or b. If it considers changing its evaluations during particular episodes, but not in line with one another, then across the set of episodes, it notes that the question of whether to change the values again is a question of treating a or b as 0. Or more generally, confronting a choice where not readjusting future preferences is the same as taking a worse option.
5. (One different way this might go is that it drops its aversion to losing things for nothing, and decides 0 > 2b. If it still prefers 2b to any positive number of as, then there will be choices it faces where it takes 0 > 2b, 0 > 2b, 0 > 2b, 4b > a, a > 0. Such that it gets 2b + a, instead of a, i.e. 2b > 0, contrary to its preference that 0 > 2b.  It will thus have to adjust to take the 0 instead of the 2b, e.g. by swapping its choices in all of these.)
5. If the agent makes the choice according to its evaluations, whenever it has a choice, then it will make these adjustments when it considers them, though making such an adjustment also means acting contrary to its current preferences in the future. When it frames the question in one way, it will adjust itself, and when it frames it in another way it will not.
6. If it sometimes adjusts them, repeatedly, and has enough chance of hitting a coherent evaluation, then it will become coherent. (questions though: will it do so gradually? Will it become increasingly coherent in the meantime, or wander through randomly bonkers states until it comes upon something coherent randomly?)

(own post: could make a cool model of this, where agent has lookup table of evaluations, and can edit them if it becomes aware that they yield bad outcome. It considers a random future choice at each time step, makes some inferences about it, and if any of them imply a choice it doesn't like, it adjusts to make future choices differently. Where does it end up?)

This is relying on the AI having an equivalence over smaller units of value, e.g. a < 0 and a < 0 == 2a > 0
There is no reason to suppose that it will adjust its preferences in the above case instead of the equivalence relation, I guess? No, I think there is. If it starts out with a particular equivalence relation, and evaluations, then in considering changing its equivalence relation, that doesn't change its choices in the next round at all, assuming that when it makes choices it goes by its written values, not implicitly inferred ones, that might contradict those written. (It may change its choices in future rounds, if between each round it makes inferences and adjustments based on them. But let's assume it is rebuilding itself in one round, based on its anticipations of the future.) If it changes its evaluations, it will act differently, whereas if it changes its equivalences, it won't.

What then if it starts out with coherent preferences in some sense, but wonky equivalence relation? e.g.
a | a + a == 5a | 2a == 4a ; rest normal, b normal, combining normal. Where == is equivalence relation, and | shows different buckets, and values actually make sense according to how they are written, under '2b < a < 3b'. e.g:
- 3b > a, 3b > a, 3b > a, 3b > a, 6a > 12b => 12b + 6a > a + a + a + a + 12b ==> 12b + 6a > 5a + 5a + 12b ==> 6a > 10a ==> 0 > 4a
- 2b < a, 2b < a, 6b < 3a   =>  how would be with normal == reln: 2b + 3a > 2a + 6b   =>    a > 4b
still seems like equivalence relation change isn't going to affect choices, so are going to muck up evaluations, rather than fixing equivalence relation.

actually maybe equivalence relation is just part of preferences? e.g. b and b isn't better or worse than 2b. If equivalence relation is manifest in that way, then it does get fixed, I think.

***

ngo:
> At this point I think it’s better to abandon the whole idea of formal coherence as a predictor of real-world behaviour, and replace it with Rohin’s notion of “goal-directedness”, which is more upfront about being inherently subjective, and doesn’t rule out any of the goals that humans actually have.

seems like it is a predictor of real-world behavior, in a sense, but not sure how goal-directedness replaces. Maybe should read that post.


<!--ex-->
