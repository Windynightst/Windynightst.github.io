---
layout: post
title: CrowdRecruiter: Selecting Participants for Piggyback Crowdsensing under Probabilistic Coverage Constraint 
---
**Summary：**

This paper proposes a novel participant selection framework, named CrowdRecruiter, for mobile crowdsensing. CrowdRecruiter operates on top of PCS and minimizes incentive payments by selecting a small number of participants while still satisfying probabilistic coverage constraint. The author used cell towers as the coverage metrics, that is, if the number of cell towers in a given region being covered is larger than a threshold, then we can say that the area is covered. 

To achieve the objective, the author created a two-phase algorithm. In the first phase, the algorithm predicts each user’s call/mobility habit using the call/mobility profile of each user. In the second phase, the algorithm selects participants iteratively by using the prediction result in first phase. In next phrase, the detail of this algorithm will be introduced.

In the first phase, there are two steps, 1) mapping call/mobility traces and 2) predicting each user’s call/mobility. In the first step, it maps each user’s historical call/mobility traces onto N sensing cycles. Then it counts λu,i,t–the average number of calls placed by each user (u∈U) at each cell tower (t∈T) in each sensing cycle (0≤ i <N). In next step, it estimates Pi,t(u)–the probability of the user (u∈U) placing at least one call at each cell tower (t∈T) during each sensing cycle (0≤i<N). Assuming the call sequence follows an inhomogeneous Poisson process, the probability of a user u to place n phone calls at cell tower t(t∈T) in sensing cycle i(0≤i<N) can be modeled as: 
