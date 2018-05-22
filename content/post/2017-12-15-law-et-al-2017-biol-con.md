---
title: Law et al. (2017) Biol Con
author: Elise Gould
date: '2017-12-15'
categories:
  - reading
  - systematic review
  - coding criteria
tags:
  - causal inference
  - evidence-based
  - policy
  - prediction
slug: law-et-al-2017-biol-con
header:
  caption: ''
  image: ''
bibliography: ../../static/files/citations/posts_read.bib
---

**Law, E. A., Ferraro, P. J., Arcese, P., Bryan, B. A., Davis, K., Gordon, A., Holden, M. H., Iacona, G., Martinez, R. M., McAlpine, C. A., Rhodes, J. R., Sze, J. S., Wilson, K. A. (2017) Projecting the performance of conservation interventions. BIOC doi: 10.1016/j.biocon.2017.08.029.**


# Problem: Projecting the performance of conservation interventions

Successful decision-making for environmental management requires reliable evidence for both the performance and efficacy of proposed conservation actions.
Predictive models are used for projecting future impacts of interventions for conservation / environmental decision-making. However the process is beset by a range of:

- complex social, ecological, economic and ethical factors (i.e. the actual problem context is complex), and importantly is complicated by:
- Trade-offs between (multiple, and perhaps competing) objectives

And technical issues:

- poor-evidence base impacts on the ability to make accurate inferences from past interventions.
- Need for DM's to extrapolate projections to novel contexts, which is made difficult by:
        - unfounded assumptions of causality
        - reliance on potentially biased limited data




*improving evidence base with retrospective evaluations*

Increasing undertaking of retrospective evaluations of past policy impacts and a general move towards enhanced transparency and reducing bias in the evidence base in conservation science (p142) is taking place. Retrospective evaluations are important for improving the evidence base 

Current studies that come to mind are Kate's bush heritage work.
Retrospective evaluations typically use principals of causal inference. and focus on "clarifying the assumptions needed to infer causal relationships from data, and on reducing the bias of impact estimtes". 

Causal inference, typically framed around a causal model, a set of hypotheses about how some treatment affects an outcome, consisting of a description of the causal pathway. 
- Potential mechanisms (the path by which the treatment causes the outcome), 
- confounders (confounding factors, rival explanations or variables that are systematically associated with the outcome and the treatment / mechanisms along the pathway. They may result in an association that is not direct or causal... OR could mask the effects of a direct treatment), 
- and moderators (interaction effect, a variable that affects the outcome of the treatment, but not correlated with exposure to the treatment)

Distinguishing between confounders and mechanisms is vital for ensuring accurate inferences of past interventions: By controlling for the influence of a mechanism you will remove the impact being sought, while controlling for the influence of a confounding variables is required to reduce bias.

Challenge when framing causal analysis, to define the counterfactual outcome. Ie the unobserved outcome for a given unit, that is what would have occurred if the treatment status were different. The **estimand** or causal effect is the difference between a unit's actual state and counterfactural state.

There are two ways of addressing this: experimental designs and quasi-experimental designs. The latter is kind of like what Kate Cranney has done. Wherein observable stand-ins are used instead of the unobservable counterfactual.

## What the paper sets out to do

The paper aoutlines the relevence, benefits and challenges of using the principles of causal inference and associated principles of: a) systematic literature reviews, b) expert elicitation, c) scenario planning. They highlight 3 steps in projection modelling that need addressing using the above principles:

1. Problem definition - clarifying causal assumptions
2. Model Parameterisation - Identifying bias in data, and therefore avoidign bias
3. Improving Model use and parameterisation - using model sensitivity analyses and exploring parameter / model uncertainty

The paper discusses techniques that:
- aid in untangling cause from correlation
- evaluate and transfer models between contexts
- characterise uncertainty
- address imperfect data

## From retrospective evaluations to projection analyses

Retrospective evaluations are important for informing future policy and interventions, however they are insufficient for achieving this goal. This is because this evidence is highly context-specific, and often does not extrapolate to other times and areas. Projection analyses / predictive models address this need: predicting intervention impacts across time and space using models.

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

## 1. Problem definition

### characterizing key variables in a causal context

Defining the problem is a key challenge in creating robust and transparent model projections. At this stage the analyst / decision-maker wants to understand how the intervention is expected to work within the environmental, social, and economic context.

-> models depecting mechanism-based causal relationships between interventions, processes and variables are developed to address this Querstion. Graphical models are recommended because thyey enable elucidation of assumed causal impacts through potentially complex pathways. BUT they must be informative and detailed enough.

Another challenge is identifying treatments and outcomes that are relvent across the social and environmental context.

### Establishing valid baselines and alternative scenarios

future scenarios (hypotheses of how a system may operate under different conditions or assumptions... a set of functions and parameters that lead to potential future states).
Baseline scenarios, are usually set as a continuation of current or historical conditions, a projection of the most likely or 'business as usual' scenario.

The difference between retrospective and prospective analyses of conservation interventions is that retrospective analyses have a fact for alternative scenarios to run counter to, there is an observable, factual case against which alternative scenarios can be compared. However, for prospective analyses both scenarios and baselines must be constructed through assumptions and narrative. Analysts need to ensure that scenarios are not impossible or highly improbabale, because this can give the impression that a particularly positive or negative outcome is likely.

Must ensure each scenario has its assumptions transparently communicated. 'Robust' prospective evaluation needs clearly articulated, conscientious, defendable definitions of baselines and alternative scnarios.

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

### Transportability

This refers to the extrapolation or generalisation of impact estimates from one sample to a population of interest.

Historically it has been criticised for extrapolation being incorrect or problematic "narrative criticism"

There is emerging work on develop structural causal theory to formally define model transportability and best methods of implementing.

What's the utility of this?

- transportation of impact estimates from experiment / pilot to larger populations (sample selection bias)
- between study systems (e.g. woodlands problem, river systems problem)
- to identify surrogate variables
- meta-analysis

# 2. Parameterisation: using better data

sources of bias include

1. observational and experimental data
2. Biases in collated data

This paper talks about these biases in the context of parameter selection.

## Biases in collated data

1. Analyst / modeller: selecting and interpreting the literature

- bias towards parameters used by previous / similar work
- towards parameters that have been highly cited
- to those in most recent analyses
- confirmation bias: i.e. those values htat fundamentally support the researcher's decision.

2. In the published literature itself

In addition to bias in the selection and interpretation of the literature, there is bias WITHIN the literature itself.

3. Expert judgment / elicitation

This is compounded by bias in expert judgment. There is both bias in published evidence base, and in expert's experience and translation of this evidence base.

The paper lists a whole bunch of sources of bias in expert elicitation. 

### Overcoming bias

- Worth noting that there are lots of emerging methods being developed that aim to ensure the elicitation procedure is robust to biases -- especially in contexts where there are no data for some variables, usually when developing novel conservation policies / interventions.
- Systematic reviews can be used, but might not be feasible / warranted for every single parameter (Addison et al. 2013).
- The principles of systematic review can be worked into workflows when synthesising information (e.g. hwo the literature can be sampled, evaluated, and evidence weighted).

# 3. Interpretation: using data better

Biases are often unavoidable, even with improved experimental design and analysis, systematic review procedures and expert elicitaiton methods. Particularly when data are used for purposes other than what they were intended (which is what we do in building decision models!!).

At minimum, data shortcomings need to be transparent such that improvements in model specification and interpretation are possible.

1. Sensitivity analyses

> Sensitivity analysis aims to characterize how variation in model inputs cause changes in model outputs (Saltelli and Annoni, 2010). It de- termines which model input parameters are most influential, and identifies where reducing model uncertainty might improve model performance.

Often only one-way SA. but this approach is misleading, the authors say, becaue most of the input parameter space is unexplored, AND is problematic where there are nonlinear interactions between parameters. Global analyses are preferable.

2. Uncertainty analyses

Provide confidence bounds on model output, or probability density function. The focus of this analysis is on"how uncertainty in all model intputs propagates through the model and results in uncertainty in the output."

Ideally when developing projections, uncertainty accounts for full uncertainty in all model input parameters AS WELL AS structural uncertainty.

> Rigorous uncertainty analyses allow for defensible confidence intervals on model projections, in particular when modelling specific alternative scenarios, as the size of these confidence intervals will determine whether a model predicts a statistically significant impact. It also allows best and worst case outcomes to be identified, explicitly allowing levels of risk aversion to be incorporated into decisions made using the model projections.


3. partial identification

Another or complementary method for deailing with uncertainty in assumptions: 
> Partial identification is an analysis framework that sequentially explores the implications of assumptions regarding the counterfactual. Assumptions decrease in credibility due to increasing strengths of the claims regarding the counterfactual, which increases the potential for criticism, and the need for evidence to support the claims.

Hasn't really been used in prospective analyses, but can be useful when there is uncertainty or controversy around potential impacts of interventions.

# Synthesis, and ways forward

Argue for more transparency of assumptions and more "believable" causal models, engender greater confidence in predictions of prospective evaluations, and aid in their justification.

Poor data, inappropriate models, erroneous assumptions, and bias may result in advice that systematically over or under-estimates impacts of policies or programs.

Can reduce bias and uncertainty in prospective analyses:

- causal inference
- scenario analysis
- systematic literature review
- expert elicitation

When extrapolating to novel contexts:

- structural causal modelling (inc. transportability theory)
- partial identification

Importantly, paper doesn't argue that elaborate, fine-scaled projection models are required for every conservation problem. BUT, at minimum, the following can be done for little or no additional cost (and increases confidence in the robustness of resultant policy advice):

- transparent clafication of causal assumptions
- consider potential bias in parameter data
conduct simple uncertainty and sensitivity analyses

# Summary, how this paper is useful to me:

ALthough the paper discusses projection analyses for conservation. A lot of this material is relevant to decision support tools in general - more often than not we are using 'prospective analyses' to generate predictions of the response of the system to a set of alternative actions. Prospective analyses form the primary tool considered in this study.

1. Identifies sources of bias that can emerge during projection analyses development, as well as techniques and principles for overcoming them. Breaks down the process into three phases (problem definition, parameterisation, interpretation). I think this is applicable to devision support tool development. And the three phases here map onto the "predict consequences or outcomes" stage of SDM.

The most relevant element, to me, relates to the section on "collated data." I.e. how analysts / modellers act as self-appointed experts to select and interpret the literature, choosing parameter values.

2. Model transportation theory

I think this theory could be relevant to the replication of DST's. But I need to continue thinking about the role of replication for DST's, why would we want to do this? And how would you do it?

3. Thinking about quantitative evaluation methods for DST's in the systematic review -- DST outputs.

Uncertainty analyses yield "confidence intervals on model projections, for alternative scenarios. The size of these confidence intervals determines whether the model predicts statistically significatn impact."

So we might actually have some numerical values which we can extract in the review.

4. Coding criteria thoughts:

The authors mention that risk attitudes can be explicitly incorporated into decisions based on model projections where confidence intervals are generated for different action / policy interventions.

This got me thinking about two things:

a. that the process of making the decision should be distinguished from the process of predicting the impacts of each intervention. Else you can't reproduce the decision.  So this could be a process model plus a decision model, or some simpler method of choosing one intervention over another. As long as it's documented and transparent. My hypothesis is that there are numerous papers out there that posit themselves to be decision support tools, or to somehow aid in some conservation decision, but do not explore the process of making a decision based on model outputs, they just present a model. My other hypothesis is that this is more common in conservation than in management contexts, e.g. in conservation prioritisation problems.

b. The reason why this is an issue, is because values and risk attitudes can impact on the chosen decision. If there is no process for incorporating them into the decision process, then the decision is not reproducible. Which brings me to my second point that should be coded, are decision maker values, risk attitudes explicitly treated / incorporated in the decision support tool? (And is it relevant, can i think about cases where it's not relevant or important)?
