id: "10.1145/3377811"
title: "How to Not Get Rich: An Empirical Study of Donations in Open Sourc"
authors: ["Overney, Cassandra", "Meinicke, Jens", "Kästner, Christian", "College, Bogdan Vasilescu Olin", "USA"]
year: 2020
doi: "10.1145/3377811"
venue: {type: "conference", name: "ACM Reference format:", volume: null, issue: null, pages: null}
citation: "Overney et al. (2020). How to Not Get Rich: An Empirical Study of Donations in Open Sourc. ACM Reference format:."
article_type: "empirical"
method: {design: "longitudinal", approach: "other", evidence_level: "moderate", preregistered: false}
gist: >
  This source gives the project a retrieval card for open-source maintainer wellbeing and
  sustainability: Open source is ubiquitous and many projects act as critical infrastructure,
  yet funding and sustaining the whole ecosystem is challenging.
claims:
  - text: "1 INTRODUCTION Open-source software is ubiquitous, but sustaining it is a challenge."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["burnout", "job-engagement"]
    predictors: ["social-support", "workload", "open-source-maintenance", "community-engagement"]
  - text: "With increasing popularity, demands for maintenance and support work typically rise, including large numbers of support requests, feature requests, and reported issues."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["burnout", "job-engagement"]
    predictors: ["social-support", "workload", "open-source-maintenance", "community-engagement"]
population:
  who: "software developers"
  where: ["USA", "Korea"]
  when: null
  n: null
  sector: ["tech", "open-source", "education"]
  sample_notes: >
    When open-source infrastructure is insuciently maintained or even abandoned by their
    developers, this can raise signicant costs and risks for users of such infrastructure, who
    might need to work around known bugs or make signicant changes to nd alternatives.
limitation:
  primary: "Since these limitations restrict the pool of projects, we only ran this analysis on the larger Github corpus, with 337 projects meeting our conditions, of which only 16 projects received more than 1000 USD in the analyzed 9 month window."
  others: ["We model the two interrupted time series, one per outcome variables, as multiple mixed-effects linear regression models, similar to prior work [69, 78].", "We follow standard model fit and diagnostic procedures, as described above in Sec."]
risk_of_bias: "medium"
relevance_to_project: >
  Useful for practitioner-facing context on open-source maintainer burnout, sustainability
  pressures, recognition, documentation, and community support. Treat claims as signals
  unless the source reports a clear empirical design.
tags:
  topic: ["burnout", "open-source", "maintainer-burnout"]
  method: ["longitudinal"]
  population: ["software-developers", "tech", "open-source", "education"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/How to Not Get Rich An Empirical Study of Donations in Open Source/How to Not Get Rich An Empirical Study of Donations in Open Source.md"
  pdf: null
  notes: null
