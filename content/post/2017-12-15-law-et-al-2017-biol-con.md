---
title: Law et al. (2017) Biol Con
author: Elise Gould
date: '2017-12-15'
slug: law-et-al-2017-biol-con
categories:
  - reading
tags:
  - causal inference
  - prediction
  - evidence-based
  - policy
header:
  caption: ''
  image: ''
bibliography: ../../static/files/citations/posts_read.bib
---

## Law, E. A., Ferraro, P. J., Arcese, P., Bryan, B. A., Davis, K., Gordon, A., Holden, M. H., Iacona, G., Martinez, R. M., McAlpine, C. A., Rhodes, J. R., Sze, J. S., Wilson, K. A. (2017) Projecting the performance of conservation interventions. BIOC doi: 10.1016/j.biocon.2017.08.029.


Projecting the performance of conservation interventions

Predictive models are used for projecting future impacts of interventions for conservation / environmental decision-making. successful decision making for EM requires reliable evidence of future performance and efficacy of interventions. This is not a straight-forward task. And faces the following issues:

- complex social, ecological, economic and ethical factors
- Trade-offs between objectives
- poor-evidence base impacts on the ability to make accurate inferences from past interventions.
- DM's often must extrapolate projections to novel contexts, which is made difficult by:
        - unfounded assumptions of causality
        - reliance on potentially biased limited data
        
The paper discusses techniques that:
- aid in untangling cause from correlation
- evaluate and transfer models between contexts
- characterise uncertainty
- address imperfect data

*improving evidence base with retrospective evaluations*

Increasing undertaking of retrospective evaluations of past policy impacts and a general move towards enhanced transparency and reducing bias in the evidence base in conservation science (p142). Current studies that come to mind are Kate's bush heritage work.
Retrospective evaluations typically use principals of causal inference. and focus on "clarifyign the assumptions needed to infer causal relationships from data, and on reducing the bias of impact estimtes". 

Causal inference, typically framed around a causal model, a set of hypotheses about how some treatment affects an outcome, consisting of a description of the causal pathway. 
- Potential mechanisms (the path by which the treatment causes the outcome), 
- confounders (confounding factors, rival explanations or variables that are systematically associated with the outcome and the treatment / mechanisms along the pathway. They may result in an association that is not direct or causal... OR could mask the effects of a direct treatment), 
- and moderators (interaction effect, a variable that affects the outcome of the treatment, but not correlated with exposure to the treatment)

Distinguishing between confounders and mechanisms is vital for ensuring accurate inferences of past interventions: By controlling for the influence of a mechanism you will remove the impact being sought, while controlling for the influence of a confounding variables is required to reduce bias.

Challenge when framing causal analysis, to define the counterfactual outcome. Ie the unobserved outcome for a given unit, that is what would have occurred if the treatment status were different. The **estimand** or causal effect is the difference between a unit's actual state and counterfactural state.

There are two ways of addressing this: experimental designs and quasi-experimental designs. The latter is kind of like what Kate Cranney has done. Wherein observable stand-ins are used instead of the unobservable counterfactual.

## From retrospective evaluations to projection analyses

Retrospective evaluations are importatn for informing future policy and interventions, however they are insufficient for achieving this goal. This is because this evidence is highly context-specific, and often does not extrapolate to other times and areas. Projection analyses / predictive models address this need: predicting intervention impacts across time and space using models.

What is a robust projection analysis / successful conservation decision-making?

- don't overestimate the benefits associated with proposed interventions: else sub-optimal outcomes
- don't underestimate their benefits: else better alternatives over-looked.

There are a number of issues in ideveloping projection analyses that may diminish successful conservation decision-making by reducing the 'scientific credibility' (plausibility and technical accuracy) of the science, i.e. models.

1. untested assumptions - associations observed in the past may not hold in the future
2. limited data
3. imperfect use of this data - unclear treatment of uncertainty, or poor interpretation of potentially biased results.

The authors review the relevance, benefits, challenges of integrating principles of causal inference and systematic literature review, expert elicitation and scenario analysis into prospective evaluation of conservation interventions.

1. How these techniques can improve the problem definition by clarifying causal assumptions, key variables, alternative scnearios and appropriate model frameworks
2. How the techniques can improve model parameterisation by identifying bias in data, and avoiding them
3. improving model use ands interpretation through analyses to understand model senstivieity + parameter / model uncertainty.

## Problem definition

### characterizing key variables in a causal context

Defining the problem is a key challenge in creating robust and transparent model projections. At this stage the analyst / decision-maker wants to understand how the intervention is expected to work within the environmental, social, and economic context.

-> models depecting mechanism-based causal relationships between interventions, processes and variables are developed to address this Querstion. Graphical models are recommended because thyey enable elucidation of assumed causal impacts through potentially complex pathways. BUT they must be informative and detailed enough.

Another challenge is identifying treatments and outcomes that are relvent across the social and environmental context.

### Establishing valid baselines and alternative scenarios

future scenarios (hypotheses of how a system may operate under different conditions or assumptions... a set of functions and parameters that lead to potential future states).
Baseline scenarios, are usually set as a continuation of current or historical conditions, a projection of the most likely or 'business as usual' scenario.

The difference between retrospective and prospective analyses of conservation interventions is that retrospective analyses have a fact for alternative scenarios to run counter to, there is an observable, factual case against which alternative scenarios can be compared. However, for prospective analyses both scenarios and baselines must be constructed through assumptions and narrative. Analysts need to ensure that scenarios are not impossible or highly improbabale, because this can give the impression that a particularly positive or negative outcome is likely.

Must ensure each scenario has its assumpptions transparently communicated. 'Robust' prospective evaluation needs clearly articulated, conscientious, defendable definitions of baselines and alternative scnarios.

The output and subsequent recommendations may substantially differ if there is variation in the scenario definition.

When testing decision tools / models using scenario analysis, the analyst must give proper thought to them, ensuring they are plausible.

### choosing appropriate model framework, given causal assumptions

The authors note 3 frameworks common for predictive models:

1. Exploratory models with many variables, aka "kitchen sink variables", e.g. multiple regression analyses and correlation-based procedures.
2. "reductionist models" 
3. "all-cause models"


Exploratory models are not useful for future projections because of their assumptions: 
Causal effects among predictors are not required
Assumes no specification error, i.e. of the form of the regression, e.g. no incorrect functional forms, missing predictors.
If models are parameterised based on corelation rather than causality, there is little *a priori* confidence 

