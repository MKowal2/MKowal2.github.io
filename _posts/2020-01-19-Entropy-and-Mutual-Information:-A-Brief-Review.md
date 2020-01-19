---
layout: post
title: "Entropy and Mutual Information: A Brief Overview"
author: "Matthew Kowal"
meta: "Springfield"
--- 

## Understanding Mutual Information

For this post I hope to accomplish a few different things. I will review a brilliant [document](https://people.cs.umass.edu/~elm/Teaching/370_F09/mutInf.pdf) put together by Erik G. Learned-Miller. I found this document when attempting to better understand the concept of 'Mutual Information', and it has been by far the most influential document in my understanding of entropy and mutual information. It is a short document, only 3 pages, with the purpose of being an introduction to entropy and mutual information for discrete random variables. Erik does something that I think so many teachers miss when introducing students to new concepts, which is using real-world, easy to understand examples to aid with the formulas. I hope I can add some intuition behind what entropy, joint entropy, and mutual information actually represent, as well as review some simple and more complex examples that I am currently working on in my research. 

### Entropy

When I started to dig into what mutual information really represents, the word I kept running into was: Entropy. Now I heard about entropy way back in highschool chemistry and physics but I'll be perfectly honest; I had no real understanding of the term, especially since I couldn't see how it could seemingly be so related to every field of science. So, what does *entropy* mean?

Entropy refers to the amount of uncertainty that an event has. If an event A has multiple outcomes, and you have no idea which outcome will occur, the event A has *high* entropy. For example, if you roll a fair 6-sided die, this event has a high entropy because each number is equally likely to appear during the roll. If event B has multiple outcomes, and you are very certain about the outcome, the event has *low* entropy. For example, if event is whether or not the sun will come up tomorrow, this event (hopefully) has a low entropy, since we are confident that the sun will come up tomorrow morning. 

As Erik points out in his document, entropy is a function of two things: 1) the number of possible outcomes, and 2) the frequency (probability) of each outcome. Erik gives very good intuition when he says: 

>  Consider a random variable X representing the number that comes up on a roulette wheel and a random variable Y representing the number that comes up on a fair 6-sided die. The entropy of X is greater than the entropy of Y. In addition to the numbers 1 through 6, the values on the roulette wheel can take on the values 7 through 36. In some sense, it is less predictable.

On top of this, if the roullete wheel is *rigged* to always come up as 15 lets say, then since the probability of it landing on 6 is 100%, the entropy is very low. To formalize the entropy of a discrete random variable $X$ that takes on the values in the set $\chi = \{x_1, x_2, ..., x_n\}$ and is definied by a probability distribution $P(X)$, we can write:

$H(X)=-\sum_{x\in\chi}P(x)logP(x)$


### Joint Entropy


### Mutual Information
