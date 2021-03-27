---
layout: post
title: "Coherence arguments imply a force for goal-directed behavior"
date: 2021-03-26 21:20:00 -0700
tags: ai airisk
comments: true
image:
summary:
---
<!--ex-->

<em><em>Crossposted from <a href="https://aiimpacts.org/">AI Impacts</a></em></em>



<em>[Epistemic status: my current view, but I haven’t read all the stuff on this topic even in the LessWrong community, let alone more broadly.]</em>



There is a line of thought that says that advanced AI will tend to be ‘goal-directed’—that is, consistently doing whatever makes certain favored outcomes more likely—and that this is to do with the ‘coherence arguments’. <a href="https://www.lesswrong.com/posts/NxF5G6CJiof6cemTw/coherence-arguments-do-not-imply-goal-directed-behavior">Rohin Shah</a>, and probably others[^1] , have argued against this. I want to argue against them.


<!-- wp:heading -->
<h2>The old argument for coherence implying (worrisome) goal-directedness</h2>
<!-- /wp:heading -->


I’d reconstruct the original argument that Rohin is arguing against as something like this (making no claim about my own beliefs here):



- **‘Whatever things you care about, you are best off assigning consistent numerical values to them and maximizing the expected sum of those values’** <br> 'Coherence arguments’[^2] mean that if you don’t maximize ‘expected utility’ (EU)—that is, if you don’t make every choice in accordance with what gets the highest average score, given consistent preferability scores that you assign to all outcomes—then you will make strictly worse choices by your own lights than if you followed some alternate EU-maximizing strategy (at least in some situations, though they may not arise). For instance, you’ll be vulnerable to ‘<a href="https://www.oxfordreference.com/view/10.1093/oi/authority.20110803100205601">money-pumping</a>’—being predictably parted from your money for nothing.[^3]
- **‘Advanced AI will tend to do better things instead of worse things, by its own lights’** <br>Advanced AI will tend to avoid options that are predictably strictly worse by its own lights, due to being highly optimized for making good choices (by some combination of external processes that produced it, its own efforts, and the selection pressure acting on its existence).
- **‘Therefore advanced AI will maximize EU, roughly’** <br>Advanced AI will tend to be fairly coherent, at least to a level of approximation where becoming more coherent isn’t worth the cost.[^5] Which will probably be fairly coherent (e.g. close enough to coherent that <a href="https://arbital.com/p/optimized_agent_appears_coherent/">humans can’t anticipate the inconsistencies</a>).
- **‘Maximizing EU is pretty much the same as being goal-directed’**<br>To maximize expected utility is to pursue the goal of that which you have assigned higher utility to.[^6]



And since the point of all this is to argue that advanced AI might be hard to deal with, note that we can get to that conclusion with:


<!-- wp:list {"ordered":true,"start":5} -->
<ol start="5"><li><strong>‘Highly intelligent goal-directed agents are dangerous’</strong><strong><br></strong>If AI systems exist that very competently pursue goals, they will likely be better than us at attaining their goals, and therefore to the extent there is a risk of mismatch between their goals and ours, we face a serious risk.</li></ol>
<!-- /wp:list -->

<!-- wp:heading -->
<h2>Rohin’s counterargument</h2>
<!-- /wp:heading -->


Rohin’s counterargument begins with an observation made by others before: any behavior is consistent with maximizing expected utility, given <em>some</em> utility function. For instance, a creature just twitching around on the ground may have the utility function that returns 1 if the agent does whatever it in fact does in each situation (where ‘situation’ means, ‘entire history of the world so far’), and 0 otherwise. This is a creature that just wants to make the right twitch in each detailed, history-indexed situation, with no regard for further consequences. Alternately the twitching agent might care about outcomes, but just happen to want the particular holistic unfolding of the universe that is occurring, including this particular series of twitches. Or it could be indifferent between all outcomes.



The basic point is that rationality doesn’t say what ‘things’ you can want. And in particular, it doesn’t say that you have to care about particular atomic units that larger situations can be broken down into. If I try to call you out for first spending money to get to Paris, then spending money to get back from Paris, there is nothing to say you can’t just have wanted to go to Paris for a bit and then to come home. In fact, this is a common human situation. ‘Aha, I money pumped you!’ says the airline, but you aren’t worried. The twitching agent might always be like this—a creature of more refined tastes, who cares about whole delicate histories and relationships, rather than just summing up modular momentarily-defined successes. And given this freedom, any behavior might conceivably be what a creature wants.&nbsp;



Then I would put the full argument, as I understand it, like this:


<!-- wp:list {"ordered":true} -->
<ol><li>Any observable sequence of behavior is consistent with the entity doing EU maximization (see observation above)</li><li>Doing EU maximization doesn’t imply anything about what behavior we might observe (from 1)</li><li>In particular, knowing that a creature is an EU maximizer doesn’t imply that it will behave in a ‘goal-directed’ way, assuming that <em>that</em> concept doesn’t apply to all behavior. (from 2)</li></ol>
<!-- /wp:list -->


Is this just some disagreement about the meaning of the word ‘goal-directed’? No, because we can get back to a major difference in physical expectations by adding:


<!-- wp:list {"ordered":true,"start":4} -->
<ol start="4"><li>&nbsp;Not all behavior in a creature implicates dire risk to humanity, so any concept of goal-directedness that is consistent with any behavior—and so might be implied by the coherence arguments—cannot imply AI risk.</li></ol>
<!-- /wp:list -->


So where the original argument says that the coherence arguments plus some other assumptions imply danger from AI, this counterargument says that they do not.&nbsp;



(There is also at least some variety in the meaning of ‘goal-directed’. I’ll use goal-directed<sub>Rohin</sub> to refer to what I think is Rohin’s <a href="https://www.lesswrong.com/s/4dHMdK5TLN6xcqtyc/p/DfcywmqRSkBaCB6Ma">preferred</a> usage: roughly, that which seems intuitively goal directed to us, e.g. behaving similarly across situations, and accruing resources, and not flopping around in possible pursuit of some exact history of personal floppage, or peaceably preferring to always take the option labeled ‘A’.[^7])


<!-- wp:heading -->
<h2>My counter-counterarguments</h2>
<!-- /wp:heading -->


What’s wrong with Rohin’s counterargument? It sounded tight.&nbsp;



In brief, I see two problems:

>A. The whole argument is in terms of logical implication. But what seems to matter is changes in probability. Coherence doesn’t need to rule out any behavior to matter, it just has to change the probabilities of behaviors. Understood in terms of probability, argument 2 is a false inference: just because any sequence of behavior is consistent with EU maximization doesn’t mean that EU maximization says nothing about what behavior we will see, probabilistically. All it says is that the probability of a behavioral sequence is never reduced to zero by considerations of coherence alone, which is hardly saying anything.


You might then think that a probabilistic version still applies: since every entity appears to be in good standing with the coherence arguments, the arguments don’t exert any force, probabilistically, on what entities we might see. But:

>B. An outside observer being able to rationalize a sequence of observed behavior as coherent doesn't mean that the behavior is actually coherent. Coherence arguments constrain combinations of external behavior and internal features—‘preferences’[^8] and beliefs. So whether an actor is coherent depends on what preferences and beliefs it actually has. And if it isn’t coherent in light of these, then coherence pressures will apply, whether or not its behavior <em>looks</em> coherent. And in many cases, revision of preferences due to coherence pressures will end up affecting external behavior. So 2) is not only not a sound inference from 1), but actually a wrong conclusion: if a system moves toward EU maximization, that does imply things about the behavior that we will observe (probabilistically).



Perhaps Rohin only meant to argue about whether it is <em>logically possible</em> to be coherent and not goal-directed-seeming, for the purpose of arguing that humanity can construct creatures in that perhaps-unlikely-in-nature corner of mindspace, if we try hard. In which case, I agree that it is logically possible. But I think his argument is often taken to be relevant more broadly, to questions of whether advanced AI will tend to be goal-directed, or to be goal-directed in places where they were not intended to be.



I take A) to be fairly clear. I’ll lay out B) in more detail.


<!-- wp:heading -->
<h2>My counter-counterarguments in more detail</h2>
<!-- /wp:heading -->

<!-- wp:heading {"level":3} -->
<h3><strong>How might coherence arguments affect creatures?</strong></h3>
<!-- /wp:heading -->


Let us step back.



How would coherence arguments affect an AI system—or anyone—anyway? They’re not going to fly in from the platonic realm and reshape irrational creatures.



The main routes, as I see it, are via implying:


<!-- wp:list {"ordered":true} -->
<ol><li>incentives for the agent itself to reform incoherent preferences</li><li>incentives for the processes giving rise to the agent (explicit design, or selection procedures directed at success) to make them more coherent</li><li>some advantage for coherent agents in competition with incoherent agents</li></ol>
<!-- /wp:list -->


To be clear, the agent, the makers, or the world are not necessarily thinking about the arguments here—the arguments correspond to incentives in the world, which these parties are responding to. So I’ll often talk about ‘incentives for coherence’ or ‘forces for coherence’ rather than ‘coherence arguments’.



I'll talk more about 1 for simplicity, expecting 2 and 3 to be similar, though I haven’t thought them through.


<!-- wp:heading {"level":3} -->
<h3><strong><em>Looking</em></strong><strong> coherent isn’t enough: if you aren’t coherent inside, coherence forces apply</strong></h3>
<!-- /wp:heading -->


If self-adjustment is the mechanism for the coherence, this doesn't depend on what a sequence of actions looks like from the outside, but from what it looks like from the inside.



Consider the aforementioned creature just twitching sporadically on the ground. Let’s call it Alex.



As noted earlier, there is a utility function under which Alex is maximizing expected utility: the one that assigns utility 1 to however Alex in fact acts in every specific history, and utility 0 to anything else.



But from the inside, this creature you excuse as 'maybe just wanting that series of twitches’ has—let us suppose—actual preferences and beliefs. And if its preferences do not in fact prioritize this elaborate sequence of twitching in an unconflicted way, and it has the self-awareness and means to make corrections, then it will make corrections[^9]. And having done so, its behavior will change. 



Thus excusable-as-coherent Alex is still moved by coherence arguments, even while the arguments have no complaints about its behavior <em>per se</em>.



For a more realistic example: suppose Assistant-Bot is observed making this sequence of actions:&nbsp;


<!-- wp:list -->
<ul><li>Offers to buy gym membership for $5/week&nbsp;</li><li>Consents to upgrade to gym-pro membership for $7/week, which is like gym membership but with added morning classes</li><li>Takes discounted ‘off-time’ deal, saving $1 per week for only using gym in evenings</li></ul>
<!-- /wp:list -->


This is consistent with coherence: Assistant-Bot might prefer that exact sequence of actions over all others, or might prefer incurring gym costs with a larger sum of prime factors, or might prefer talking to Gym-sales-bot over ending the conversation, or prefer agreeing to things.



But suppose that <em>in fact</em>, in terms of the structure of the internal motivations producing this behavior, Assistant-Bot just prefers you to have a gym membership, and prefers you to have a better membership, and prefers you to have money, but is treating these preferences with inconsistent levels of strength in the different comparisons. Then there appears to be a coherence-related force for Assistant-Bot to change. One way that that could look is that since Assistant-Bot’s overall behavioral policy currently entails giving away money for nothing, and also Assistant-Bot prefers money over nothing, that preference gives Assistant-Bot reason to alter its current overall policy, to avert the ongoing exchange of money for nothing.[^10] And if its behavioral policy is arising from something like preferences, then the natural way to alter it is via altering those preferences, and in particular, altering them in the direction of coherence.



One issue with this line of thought is that it’s not obvious in what sense there is anything inside a creature that corresponds to ‘preferences’. Often when people posit preferences, the preferences are defined in terms of behavior. Does it make sense to discuss different possible ‘internal’ preferences, distinct from behavior? I find it helpful to consider the behavior and ‘preferences’ of groups:



Suppose two cars are parked in driveways, each containing a couple. One couple are just enjoying hanging out in the car. The other couple are dealing with a conflict: one wants to climb a mountain together, and the other wants to swim in the sea together, and they aren’t moving because neither is willing to let the outing proceed as the other wants. ‘Behaviorally’, both cars are the same: stopped. But their internal parts (the partners) are importantly different. And in the long run, we expect different behavior: the car with the unconflicted couple will probably stay where it is, and the conflicted car will (hopefully) eventually resolve the conflict and drive off.



I think here it makes sense to talk about internal parts, separate from behavior, and real. And similarly in the single agent case: there are physical mechanisms producing the behavior, which can have different characteristics, and which in particular can be ‘in conflict’—in a way that motivates change—or not. I think it is also worth observing that humans find their preferences ‘in conflict’ and try to resolve them, which is suggests that they at least are better understood in terms of both behavior and underlying preferences that are separate from it.&nbsp;



So we have: even if you can excuse any seizuring as consistent with coherence, coherence incentives still exert a force on creatures that are<em> in fact</em> incoherent, given their real internal state (or would be incoherent if created). At least if they or their creator have machinery for noticing their incoherence, caring about it, and making changes.



Or put another way, coherence doesn’t exclude overt behaviors alone, but does exclude combinations of preferences, and preferences beget behaviors. This changes how specific creatures behave, even if it doesn’t entirely rule out any behavior ever being correct for some creature, somewhere.&nbsp;



That is, the coherence theorems may change what behavior is <em>likely</em> to appear amongst creatures with preferences.&nbsp;


<!-- wp:heading {"level":3} -->
<h3><strong>Reform for coherence probably makes a thing more goal-directed</strong><strong><sub>Rohin</sub></strong></h3>
<!-- /wp:heading -->


Ok, but moving toward coherence might sound totally innocuous, since, per Rohin’s argument, coherence includes all sorts of things, such as absolutely any sequence of behavior.&nbsp;



But the relevant question is again whether a coherence-increasing reform process is likely to result in some kinds of behavior over others, probabilistically.



This is partly a practical question—what kind of reform process is it? Where a creature ends up depends not just on what it incoherently ‘prefers’, but on what kinds of things its so-called ‘preferences’ are at all[^11], and what mechanisms detect problems, and how problems are resolved.



My guess is that there are also things we can say in general. It’s is too big a topic to investigate properly here, but some initially plausible hypotheses about a wide range of coherence-reform processes:


<!-- wp:list {"ordered":true} -->
<ol><li><strong>Coherence-reformed entities will tend to end up looking similar to their starting point but less conflicted<br></strong>For instance, if a creature starts out being indifferent to buying red balls when they cost between ten and fifteen blue balls, it is more likely to end up treating red balls as exactly 12x the value of blue balls than it is to end up very much wanting the sequence where it takes the blue ball option, then the red ball option, then blue, red, red, blue, red. Or wanting red squares. Or wanting to ride a dolphin.<br><br>(I agree that if a creature starts out valuing Tuesday-red balls at fifteen blue balls and yet all other red balls at ten blue balls, then it faces no obvious pressure from within to become ‘coherent’, since it is not incoherent.)<br></li><li><strong>More coherent strategies are systematically less wasteful, and waste inhibits goal-direction<sub>Rohin</sub>, which means more coherent strategies are more forcefully goal-directed<sub>Rohin</sub> on average</strong><br>In general, if you are sometimes a force for A and sometimes a force against A, then you are not moving the world with respect to A as forcefully as you would be if you picked one or the other. Two people intermittently changing who is in the driving seat, who want to go to different places, will not cover distance in any direction as effectively as either one of them. A company that cycles through three CEOs with different evaluations of everything will—even if they don’t actively scheme to thwart one another—tend to waste a lot of effort bringing in and out different policies and efforts (e.g. one week trying to expand into textiles, the next week trying to cut everything not involved in the central business).</li></ol>
<!-- /wp:list -->

<!-- wp:list {"ordered":true,"start":3} -->
<ol start="3"><li><strong>Combining points 1 and 2 above, as entities become more coherent, they generally become more goal-directed</strong><strong><sub>Rohin</sub></strong><strong>. </strong>As opposed to, for instance, becoming more goal-directed<sub>Rohin</sub> <em>on average,</em> but individual agents being about as likely to become worse as better as they are reformed. Consider: a creature that values red balls at 12x blue balls is very similar to one that values them inconsistently, except a little less wasteful. So it is probably similar but more goal-directed<sub>Rohin</sub>. Whereas it’s fairly unclear how goal-directed<sub>Rohin </sub>a creature that wants to ride a dolphin is compared to one that wanted red balls inconsistently much. In a world with lots of balls and no possible access to dolphins, it might be much less goal-directed<sub>Rohin</sub>, in spite of its greater coherence.&nbsp;</li></ol>
<!-- /wp:list -->

<!-- wp:list {"ordered":true,"start":4} -->
<ol start="4"><li><strong>Coherence-increasing processes rarely lead to non-goal-directed</strong><strong><sub>Rohin</sub></strong><strong> agents—like the one that twitches on the ground</strong><strong><br></strong>In the abstract, few starting points and coherence-motivated reform processes will lead to an agent with the goal of carrying out a specific convoluted moment-indexed policy without regard for consequence, like Rohin’s twitching agent, or to valuing the sequence of history-action pairs that will happen anyway, or to being indifferent to everything. And these outcomes will be even less likely in practice, where AI systems with anything like preferences probably start out caring about much more normal things, such as money and points and clicks, so will probably land at a more consistent and shrewd version of that, if 1 is true. (Which is not to say that you couldn’t intentionally create such a creature.)<br></li></ol>
<!-- /wp:list -->


These hypotheses suggest to me that the changes in behavior brought about by coherence forces favor moving toward goal-directedness<sub>Rohin</sub>, and therefore at least weakly toward risk.


<!-- wp:heading -->
<h2>Does this mean advanced AI will be goal-directed<sub>Rohin</sub>?</h2>
<!-- /wp:heading -->


Together, this does not imply that advanced AI will tend to be goal-directed<sub>Rohin</sub>. We don’t know how strong such forces are. Evidently not so strong that humans[^12], or our other artifacts, are whipped into coherence in mere hundreds of thousands of years[^13]. If a creature doesn’t have anything like preferences (beyond a tendency to behave certain ways), then coherence arguments don’t obviously even apply to it (though discrepancies between the creature’s behavior and its makers’ preferences probably produce an analogous force[^14] and competitive pressures probably produce a similar force for coherence in valuing resources instrumental to survival). Coherence arguments mark out an aspect of the incentive landscape, but to say that there is an incentive for something, all things equal, is not to say that it will happen.


<!-- wp:heading -->
<h2>In sum</h2>
<!-- /wp:heading -->


1) Even though any behavior could be coherent in principle, if it is not coherent in combination with an entity’s internal state, then coherence arguments point to a real force for different (more coherent) behavior.



2) My guess is that this force for coherent behavior is also a force for goal-directed behavior. This isn't clear, but seems likely, and also isn't undermined by Rohin's argument, as seems commonly believed.


<br>
<br>

<figure class="wp-block-image size-large is-resized"><a href="http://aiimpacts.org/wp-content/uploads/2021/03/Two_dogs_attached_to_the_same_leash_are_pulling_in_different_Wellcome_V0021880-scaled.jpeg"><img src="http://aiimpacts.org/wp-content/uploads/2021/03/Two_dogs_attached_to_the_same_leash_are_pulling_in_different_Wellcome_V0021880-1024x804.jpeg" alt="" class="wp-image-2877" width="768" height="603"/></a><figcaption><em>Two dogs attached to the same leash are pulling in different directions</em>. <a href="https://commons.wikimedia.org/wiki/File:Two_dogs_attached_to_the_same_leash_are_pulling_in_different_Wellcome_V0021880.jpg">Etching by J. Fyt</a>, <a href="https://catalogue.wellcomelibrary.org/record=b1199389">1642</a></figcaption></figure>


<br>

<!-- wp:separator -->
<hr/>
<!-- /wp:separator -->

<br>

[^1]: For instance, Richard Ngo agrees <a href="https://www.lesswrong.com/posts/vphFJzK3mWA4PJKAg/coherent-behaviour-in-the-real-world-is-an-incoherent">here</a>, and Eric Drexler makes a related argument <a href="https://www.fhi.ox.ac.uk/wp-content/uploads/Reframing_Superintelligence_FHI-TR-2019-1.1-1.pdf">here</a>, section 6.4.
[^2]: Something something <a href="https://arbital.com/p/expected_utility_formalism/?l=7hh">This</a> has more on these arguments.
[^3]: I haven’t read all of this, and don’t yet see watertight versions of these arguments, but this is not the time I’m going to get into that.
[^5]: Assuming being ‘more coherent’ is meaningful and better than being ‘less coherent’, granting that one is not coherent, which sounds plausible, but which I haven’t got into. One argument against is that if you are incoherent at all, then it looks to me like you can logically evaluate any bundle of things at any price. Which would seem to make all incoherences identical—much like how all logical contradictions equivalently lead to every belief. However this seems unlikely to predict well how creatures behave in practice if they have an incoherent preferences.
[^6]: This isn’t quite right, since ‘goal’ suggests one outcome that is being pursued ahead of all others, whereas EU-maximizing implies that all possible outcomes have an ordering, and you care about getting higher ones in general, not just the top one above all others, but this doesn’t seem like a particularly relevant distinction here.
[^7]: I am not sold on this usage myself for ‘goal-directed’—there is an appeal to using that phrase for ‘pursues goals’ in its most basic sense, but I am also tentatively in favor of having as many concepts as possible.
[^8]: It seems perhaps misleading to call these ‘preferences’, if they are incoherent, and so do not together implicate orderings of outcomes being better than one another. If a creature is not coherent, what are even the objects of its decision calculus? I am inclined to think in terms of ‘decision criteria’, e.g. ‘given X and Y, choose X’, and ‘given Y and Z, choose Y’, which don’t necessarily imply anything about ‘given Z and X, choose …’, but I haven’t thought about this much, and it seems like a technical detail of the creature in question. Whatever they are though, if the creature has behavior, then there are internal dynamics that produce it. When exactly an aspect of these should be considered a ‘preference’ for the sake of this argument isn’t entirely clear to me, but would seem to depend on something like whether it tends to produce actions favoring certain outcomes over other outcomes across a range of circumstances (similar to the unclear definition of ‘agent’).
[^9]: The ‘right’ way to correct your own incoherent preferences seems complicated and not obviously well defined or existent, and perhaps there is not much more to say than that what you do will depend on your design. It’s also not clear to me that a genuinely incoherent creature should necessarily want to reform, by its own lights, but that is a question for another time—here I’m assuming that the coherence arguments do have this implication that seems commonly attributed to them. My guess is that in practice, such creatures often do want to reform, and exactly how they do it doesn’t matter for my argument here.
[^10]: I’m describing the force potentially felt by Assistant-Bot itself, but to the extent that its makers, or users also have preferences for money over nothing, and wish to use Assistant-Bot, and can alter it, they would seem to have similar incentives to mitigate its self-defeating behavior.
[^11]: The creature’s ‘preferences’ can’t be in terms of consistent numerical values assigned to everything, because those would be consistent. So what are they? For instance, one might imagine that they are pairwise comparisons between some kind of things (which can include ‘A > B’ and ‘B > C’ and ‘C > A’), or that they are a set of ‘situation—>action’ mappings, or they are a noisy ‘options—>feelings’ mapping combined with a set of deontological constraints over actions and feelings (‘choose things you feel better about, except don’t choose things out of selfishness, except when you feel more than 50% scared...’, etc.
[^12]: For instance, humans are insistently incoherent on the <a href="https://en.wikipedia.org/wiki/Allais_paradox">Allais paradox</a>.
[^13]: That seems pretty interesting—but note that well-designed computers have been known to do things that took humans participating in biological and cultural evolution hundreds of thousands of years before, so inference here not straightforward, and the forces of coherence depend on the costs of reform, which depend on the machinery for it. Also, we don’t know what other forces were in play—there might even have been forces for apparent incoherence, e.g. insofar as hypocrisy can benefit social animals, and dishonesty is complicated (<a href="https://www.amazon.com/Elephant-Brain-Hidden-Motives-Everyday/dp/0190495995">The Elephant in the Brain</a> discusses such ideas).
[^14]: For instance, the coherent creature that evaluates red balls differently on Tuesday and Wednesday might be in conflict with its creators, if they have a more consistent red ball evaluation, giving them reason to reform it. You might class this under the question, ‘what kinds of advanced AI will people want?’, but the reason for it is very similar to the reasons for internal pressure for coherence. If you refuse to pay $13 for a red ball, and your AI then goes out and buys you one for $15 because it is Tuesday, then the pair of you together could have done better.
