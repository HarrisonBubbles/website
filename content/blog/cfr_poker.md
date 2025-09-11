+++
title = 'CFR Poker'
date = 2025-09-11T15:50:13-04:00
description = "A project on Counterfactual Regret Minimization I did during an ML summer program"
+++

![CFR Poker Screenshot](/images/pocket_poker.png)

This post is months overdue at this point, but I figure late is better than never! Back in May, I did a project and presentation as part of the [ML Summer School 2025](https://sites.google.com/view/rtg-northeastern/graduate/summer-schools/ml-summer-school-2025?authuser=0) at Northeastern University. Specifically, I created a variation of Poker (which I deem "Pocket Poker") and then utilized Counterfactual Regret Minimization (CFR) to train a playable opponent bot. 


CFR is essentially a self-play algorithm which iteratively minimizes average overall "regret" for both players used in training. In doing so, CFR uncovers a strategy which is guaranteed to converge to a Nash equilibirum -- the ultimate defensive strategy that cannot be beaten in expectation.


You can check out my brief presentation slides [here](/CFR.pdf), or play against my bot [here!](https://cfr-poker-web.vercel.app/)

# Pocket Poker Rules

- 20 card deck (4 suits of 10,J,Q,K,A)
- 2 hole cards dealt to each player
- 1 shared community card
- 1 chip mandatory blind bet
- 1 round of fixed betting
- If no player folds, go to showdown and compare hands
- **Hand ranking:**
  - Three-of-a-kind
  - Pair
  - High card


# Resources

- [My CFR Poker Repository](https://github.com/HarrisonBubbles/CFRPoker)
- [Video on the exact algorithm I used (MCCFR)](https://www.youtube.com/watch?v=iU14jOue9Dk)
- [Comprehensive page about CFR](https://int8.io/counterfactual-regret-minimization-for-poker-ai/)
