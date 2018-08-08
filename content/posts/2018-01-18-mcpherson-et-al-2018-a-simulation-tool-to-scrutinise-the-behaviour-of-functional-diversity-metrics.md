---
title: McPherson et al 2018 A simulation tool to scrutinise the behaviour of functional
  diversity metrics
author: Elise Gould
date: '2018-01-18'
slug: mcpherson-et-al-2018-a-simulation-tool-to-scrutinise-the-behaviour-of-functional-diversity-metrics
categories:
  - reading
tags:
  - indices
  - accuracy
header:
  caption: ''
  image: ''
bibliography: ../../static/files/citations/posts_read.bib
---

\cite{MEE3:MEE312855}

**Problem**

More and more indices of diversity are created with time. Accurately quantifying functional diversity is important because we want to know how biodiversity loss affects ecosystem functioning.

Functional diversity is the "values and range of functionally important traits in a community".

The authors describe four dimensions to functional diversity:

1. functional richness
2. evenness
3. divergence
4. redundancy

And they each characterise how organisms interact with ecosystem functioning.

Although the choice of index should be guided by the functional diversity component of interest, there are multiple indices available for each component, and then there are synthetic indices that summarise all four components as a whole. Importantly, different indices are sensitive to the number of traits, the nature and distribution of trait values, as well as abundance frequencies. 

**What they did**

In order to help researchers choose the most appropriate index that best reflects the underlying properties of the ecological communities. The authors developed the R-function *simul.comms*, which simulates artificial ecological communities to explore the sensitivities of differnt diversity indices.

The authors test the *simul.comms* function on the functional redundancy function *R*.

# References

