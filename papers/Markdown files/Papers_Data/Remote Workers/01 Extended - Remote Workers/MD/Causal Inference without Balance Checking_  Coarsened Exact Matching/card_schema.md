id: "business-2007-causal-inference-without-balance-checking-coarsened-exac"
title: "Causal Inference without Balance Checking: Coarsened Exact Matching"
authors: ["Business", "Statistics", "Conservatorio, Via", "Milan, I-"]
year: 2007
doi: null
venue: {type: "journal", name: "Stefano M. Iacus", volume: null, issue: null, pages: null}
citation: "Business et al. (2007). Causal Inference without Balance Checking: Coarsened Exact Matching. Stefano M. Iacus."
article_type: "empirical"
method: {design: "rct", approach: "experiment", evidence_level: "strong", preregistered: false}
gist: >
  This source gives the project a retrieval card for remote-work isolation, collaboration,
  wellbeing, and performance: We show that CEM possesses a wide range of statistical
  properties not available in most other matching methods but is at the same time
  exceptionally easy to comprehend and use.
claims:
  - text: "All information necessary to replicate the results in this paper appear in Iacus, King, and Porro (2011b). the only inferences necessary are those relatively close to the data, leading to less model dependence and reduced statistical bias than without matching (Ho et al."
    evidence: "rct"
    support_strength: "strong"
    outcomes: []
    predictors: ["open-source-maintenance"]
  - text: "This disconnect gives rise to the most difficult problem in real empirical applications of matching: in many observational data sets, finding a matching solution that improves balance between the treated and control groups is easy for most covariates, but the result often leaves balance worse for some other..."
    evidence: "rct"
    support_strength: "strong"
    outcomes: []
    predictors: ["open-source-maintenance"]
  - text: "Thus, analysts are left with the nagging worry that all their ''improvements'' in applying matching may actually have increased bias and model dependence."
    evidence: "rct"
    support_strength: "strong"
    outcomes: []
    predictors: ["open-source-maintenance"]
population:
  who: "remote workers or employees"
  where: ["Italy"]
  when: null
  n: null
  sector: ["tech", "open-source", "education"]
  sample_notes: >
    They guarantee the matched sample size ex ante (thus fixing most aspects of the variance)
    and produce some level of reduction in imbalance between the treated and control groups
    (hence reducing bias and model dependence) only as a consequence and only sometimes.
limitation:
  primary: "Trial context and follow-up window may limit generalizability beyond the tested population."
  others: ["Implementation fidelity and attrition should be checked before adapting the intervention model."]
risk_of_bias: "low"
relevance_to_project: >
  Useful for the remote-work stream because it indexes evidence on isolation, mediated
  communication, wellbeing, job engagement, boundary management, and performance.
tags:
  topic: ["open-source"]
  method: ["rct", "theory"]
  population: ["remote-workers-or-employees", "tech", "open-source", "education"]
source:
  markdown: "Papers_Data/Remote Workers/01 Extended - Remote Workers/MD/Causal Inference without Balance Checking_  Coarsened Exact Matching/Causal Inference without Balance Checking_  Coarsened Exact Matching.md"
  pdf: null
  notes: null
