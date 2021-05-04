---
layout: post
title: "An exploration of fragility of value"
date: 2021-01-xx 10:30:00 -0700
tags: CATEGORY-1 CATEGORY-2
comments: true
image:
summary:
---
An experiment you could do, to learn more about the fragility of value and utility functions and ML and stuff (yeah, I know, not the finest preregistration):
1. Choose a thing to value in a dataset, e.g. narrow vertical stripes
2. Among a tiny and non-uniform subset of the data, try to train a model to evaluate things as good according to your metric, e.g. using only pictures of streetscapes, try to get it to rate the extent to which images involve narrow vertical stripes
3. Do this until it is pretty good in the training set
4. Explore its valuations of the larger set:
- Find the overall best examples according to your metric, and see what it thinks of them
- What do its favorite things look like, and how good are they according to your metric? (In this miniature universe, would turning decision-making over to the AI get you almost your favorite outcome, or almost the worst outcome?)
- Find the best-according-to-you thing that it also gives a high score to - how much worse is it than the best thing, on your values? Is it basically narrow vertical stripes, but not the narrowest ones available, or is it a mish-mash checkerboard?
- Construct artificially the optimal example according to your values - the narrowest and verticalest of stripes, say. What does it think of those?

I don't expect any of this is necessarily that similar to what happens when every part of this is at a vastly different scale, but I expect it is more similar than a human's abstract speculations, and might have patterns or issues in common that are harder to come up with.
