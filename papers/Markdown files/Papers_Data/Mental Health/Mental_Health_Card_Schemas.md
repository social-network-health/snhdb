# Card Schemas - Mental Health

<!-- GENERATED FILE - do not edit. Source of truth is each paper's
     MD/<paper>/card_schema.md. Regenerate with:
     python3 tools/audit/build_combined_cards.py -->

id: "anon-2022-14-points-the-evidence-the-networks"
title: "14 Points: The Evidence (The Networks of Support Approach — Essential Factors for Effective Prevention Programming)"
authors:
year: 2022
doi: null
venue: {type: "report", name: "Networks of Support Approach (internal evidence brief)", volume: null, issue: null, pages: null}
citation: "Networks of Support Approach (internal evidence brief) (2022). 14 Points: The Evidence (The Networks of Support Approach — Essential Factors for Effective Prevention Programming). Networks of Support Approach (internal evidence brief)."
article_type: "review"
method: {design: "review-scoping", approach: "secondary-data", evidence_level: "low", preregistered: false}
gist: >
  This is an internal evidence brief that assembles quotes and results from the Wingman-
  Connect Air Force suicide-prevention program (a 2017-2019 cluster RCT and its follow-up
  social-network-analysis sub-study), a 38-high-school youth-adult network study (N=10,291),
  and the Sources of Strength peer-leader program, organized into 14 'why' points supporting
  a 'Networks of Support Approach' to prevention programming. It argues for group-level,
  network-informed, peer-delivered interventions over individual risk-detection, citing
  findings such as increased class cohesion and help-seeking acceptability, reduced suicide-
  risk and depression scores, nearly 50% fewer occupational-impairment incidents, and
  reduced disconnection drift among Airmen at elevated suicide risk. The document itself is
  a curated synthesis for program advocacy, not an original study or systematic review.
claims:
  - text: "In the Wingman-Connect cluster RCT with Air Force trainees (2017-2019), training produced statistically significant increases in class cohesion, morale, positive bonds, and acceptability of help-seeking, and reductions in suicide-risk scores, depression, and anger reactivity, alongside nearly a 50% reduction in occupational impairment (corrective training, negative counseling)."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation", "depression", "wellbeing"]
    predictors: ["team-cohesion", "social-support", "intervention"]
  - text: "A social-network-analysis sub-study of the same cluster RCT (Social Science & Medicine, 2022) found Wingman-Connect counteracted the typical drift toward disconnection among Airmen at elevated suicide risk; at six months, at-risk Airmen in the program made on average three times more new valued-connection nominations than the active control condition."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["isolation", "sense-of-belonging"]
    predictors: ["network-structure", "team-cohesion", "intervention"]
  - text: "In a network study of 38 high schools (N=10,291 students, J Child Psychol Psychiatry, 2019), more integrated youth-adult networks (students sharing trusted adults with friends) were associated with lower rates of suicide attempts, the first empirical evidence linking integrated youth-adult connection patterns to suicide-attempt outcomes at the school-population level."
    evidence: "cross-sectional"
    support_strength: "low-to-moderate"
    outcomes: ["suicidal-ideation", "sense-of-belonging"]
    predictors: ["social-support", "network-structure"]
population:
  who: "Composite of cited study samples: U.S. Air Force personnel in technical training (Wingman-Connect cluster RCT and its network sub-study), students across 38 U.S. high schools, and adolescents in the Sources of Strength peer-leader program; the brief itself has no independent sample."
  where: ["USA"]
  when: "2010-2022"
  n: null
  sector: ["military", "education", "mental-health"]
  sample_notes: >
    Aggregates results from at least four separate published/submitted studies rather than
    reporting a single sample; one cited source (an NIH grant submission dated 2022) has no
    publicly accessible published results, and exact recruitment/response-rate details for
    the underlying studies are not reproduced in this brief.
limitation:
  primary: "This is a promotional evidence brief that selectively quotes favorable findings from studies of a single program family (Wingman-Connect/Sources of Strength) to argue for 14 design principles, with no described method for source selection, no critical appraisal, and no discussion of null results or limitations of the underlying studies."
  others:
    - "No systematic search strategy or inclusion criteria are described, so it functions as an index of supporting quotes rather than a synthesis of the full evidence base"
    - "One key citation is an unpublished NIH grant submission with no publicly accessible study results"
    - "Effect estimates (e.g., '50% reduction', '3x more nominations') are reproduced without confidence intervals or full statistical context"
risk_of_bias: "high"
relevance_to_project: >
  Indexes the strongest available evidence for network-informed, group-cohesion-based
  suicide-prevention interventions (Wingman-Connect), directly relevant to designing SNH
  interventions that build peer cohesion and counteract social disconnection drift in at-
  risk populations; useful as a pointer into the primary Wingman-Connect RCT and its social-
  network-analysis sub-study for evidence on group-level interventions versus individual
  risk-detection approaches.
tags:
  topic: ["suicide-prevention", "social-support", "community-health", "psychological-safety", "wellbeing"]
  method: ["review-scoping", "secondary-data"]
  population: ["military-personnel", "adolescents"]
source:
  markdown: "Papers_Data/Mental Health/MD/14 points - the evidence.docx/14 points - the evidence.docx.md"
  pdf: null
  notes: "no-doi: confirmed none (manual review)"

---

id: "pickering-2022-a-comparison-of-peer-change-agent"
title: "A comparison of peer change agent selection methods: Evidence from a high-school based suicide preventive intervention"
authors:
  - "Pickering, Trevor A."
  - "Wyman, Peter A."
  - "Valente, Thomas W."
year: 2022
doi: "10.1186/s12889-022-13372-w"
venue: {type: "journal", name: "BMC Public Health", volume: 22, issue: 1, pages: null}
citation: "Pickering et al. (2022). A comparison of peer change agent selection methods: Evidence from a high-school based suicide preventive intervention. BMC Public Health, 22(1). https://doi.org/10.1186/s12889-022-13372-w"
article_type: "empirical"
method: {design: "longitudinal", approach: "secondary-data", evidence_level: "moderate", preregistered: false}
gist: >
  Using baseline social-network survey data from 5,746 students across 20 high schools
  implementing the Sources of Strength suicide-prevention program, this study compares the
  school staff's actual peer-leader selections against several theoretical, network-informed
  selection methods (opinion leadership, friendship-network centrality metrics, key-players
  algorithm, and hybrid combinations). It finds low overlap between adult-selected and
  network-optimal peer leader sets, systematic demographic trade-offs across methods, and
  that schools whose adult-selected leaders more closely matched network-informed sets saw
  greater diffusion of the intervention, especially peer-to-peer communication and media
  exposure.
claims:
  - text: "Adult-selected peer leaders (APL) had low concordance with theoretically-optimal peer leader sets identified from network data, ranging from 13.3% overlap with the Key Players method to 22.7% overlap with an influence-weighted hybrid method."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["collaboration"]
    predictors: ["network-structure", "sampling-method"]
  - text: "Selection method produced systematic demographic trade-offs: friendship-network-based selection (in-degree, closeness) produced peer leader sets that were more white and younger than the general student body, while the Key Players algorithm produced the most demographically representative sets across sex, race, age, and grade."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["sense-of-belonging"]
    predictors: ["network-structure", "inclusiveness", "sampling-method"]
  - text: "School-level concordance between adult-selected leaders and theoretical network-informed sets predicted intervention diffusion: a 1-percentage-point increase in Peer Opinion Leader concordance was associated with a 0.82 percentage-point increase in students reporting direct peer communication about the program (p<.001), and nearly all network-informed methods placed peer leaders closer than adult-selected leaders to at-risk students (suicidal ideation/attempt, network-peripheral, no trusted adult)."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["communication", "suicidal-ideation", "help-seeking"]
    predictors: ["network-structure", "peer-mentoring", "intervention"]
population:
  who: "High-school students (grades 9-12) in schools implementing the Sources of Strength peer-led suicide prevention program, plus the subset of 429-459 students selected as adult-chosen peer leaders each school year"
  where: ["United States (New York, North Dakota)"]
  when: "2010-2013 (baseline enrollment across four intervention cohorts; diffusion assessed after first program year)"
  n: 5746
  sector: ["education", "youth-mental-health"]
  sample_notes: >
    20 high schools (of 40 in a larger effectiveness-implementation RCT) randomized to
    immediate implementation; schools in predominantly rural/small-town/micropolitan
    counties with above-average youth suicide rates; average survey enrollment 82.2% (range
    65.9-98.3%) of students; peer leaders were staff-nominated (up to 6 nominations per
    staff member) targeting 5-10% of students, with 83.2% of invited students enrolling with
    parent permission and youth assent.
limitation:
  primary: "The theoretical, network-informed peer leader sets were never actually implemented in schools -- the study only correlates hypothetical set concordance with observed diffusion, so causal claims about which selection method would improve diffusion are unverified."
  others:
    - "Adult selection of peer leaders followed no fully standardized algorithm, so APL sets may be unreproducible, limiting generalizability of concordance findings to other studies or contexts."
    - "School-level regression analyses of concordance and diffusion relied on only 20 school-level observations, limiting statistical power and precision."
    - "Important non-network determinants of diffusion (peer leader willingness, attitudes, persuasiveness, attendance, personality) were not measured and could confound the observed associations."
risk_of_bias: "medium"
relevance_to_project: >
  Directly informs how the SNH project might identify and recruit community 'peer leaders'
  or connectors for support and prevention efforts: it shows that intuitive, staff-driven
  selection under-uses available network information, that different network metrics
  (centrality vs. key-players vs. opinion leadership) trade off representativeness against
  closeness to at-risk/isolated members, and that a hybrid selection approach may best
  balance reach, diversity, and proximity to at-risk individuals -- a concrete, evidence-
  based method for designing peer-support or ambassador programs in remote/distributed
  communities.
tags:
  topic: ["suicide-prevention", "community-health", "social-support", "methodology"]
  method: ["longitudinal", "secondary-data", "network-analysis"]
  population: ["adolescents", "school-based", "at-risk-youth"]
source:
  markdown: "Papers_Data/Mental Health/MD/A Comparison of Peer Change Agent Selection Methods Evidence from a High-School Based Suicide Preventive Intervention/A Comparison of Peer Change Agent Selection Methods Evidence from a High-School Based Suicide Preventive Intervention.md"
  pdf: "papers/Mental Health/A Comparison of Peer Change Agent Selection Methods Evidence from a High-School Based Suicide Preventive Intervention.pdf"
  notes: null

---

id: "anon-2010-supplemental-material-for-a-general-multilevel"
title: "Supplemental Material for A General Multilevel SEM Framework for Assessing Multilevel Mediation"
authors:
year: 2010
doi: "10.1037/a0020141.supp"
venue: {type: "journal", name: "Psychological Methods", volume: null, issue: null, pages: null}
citation: "Psychological Methods (2010). Supplemental Material for A General Multilevel SEM Framework for Assessing Multilevel Mediation. Psychological Methods. https://doi.org/10.1037/a0020141.supp"
article_type: "methods"
method: {design: "methods", approach: "modelling", evidence_level: "reference", preregistered: false}
gist: >
  This is a statistics methods paper (Preacher, Zyphur, & Zhang, 2010, Psychological
  Methods) that develops a general multilevel structural equation modeling (MSEM) framework
  for testing mediation hypotheses in nested/clustered data, such as individuals nested in
  teams or organizations. It shows analytically that conventional multilevel modeling (MLM)
  approaches to mediation conflate within-group and between-group effects and cannot handle
  designs where the mediator or outcome is measured at the group level, and it demonstrates
  with three re-analyzed datasets that MSEM can yield substantively different conclusions
  than conventional MLM/two-step approaches, including finding a significant indirect effect
  of perceived transformational leadership on team performance via team satisfaction where a
  standard aggregation approach found none. For the SNH project it functions as the
  reference method for correctly testing multilevel mediation hypotheses (e.g., team-level
  leadership or culture predicting individual burnout or turnover via individual-level
  social support or engagement) without the conflation bias inherent to naive MLM mediation
  tests.
claims:
  - text: "Standard MLM approaches to mediation with nested data conflate the between-group and within-group components of the indirect effect into a single biased slope, and the common group-mean-centering fix (the 'unconflated multilevel model,' UMM) still yields a biased between-group indirect effect when cluster sizes are small or a predictor's intraclass correlation (ICC) is low; the paper derives the expected bias analytically (Eq. 1-2)."
    evidence: "theory"
    support_strength: "strong"
    outcomes: ["measurement-bias"]
    predictors: ["sampling-method"]
  - text: "Reanalyzing survey data from 79 team leaders and 429 team members at a Chinese telecom customer-service center, MSEM found a significant indirect effect of leader-reported shared vision on member-reported team potency via leader identification with the team (indirect effect = .218, 90% CI [0.055, 0.432]), a larger and less precise estimate than the conventional two-step OLS+MLM approach applied to the identical data (.146, p < .05, 90% CI [0.044, 0.269])."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["collaboration"]
    predictors: ["leadership-style", "team-cohesion"]
  - text: "Reanalyzing the same team dataset for an upward (bottom-up) 1-1-2 mediation model, MSEM found a significant indirect effect of members' perceived transformational leadership on manager-rated team performance via team satisfaction (a x b = .697, 90% CI [0.022, 1.459]), whereas the conventional two-step aggregation approach on the identical data found no significant effect (a x b = .053, p < .85), showing that method choice alone can reverse a mediation study's substantive conclusion."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["performance", "job-satisfaction"]
    predictors: ["leadership-style"]
population:
  who: "Not a substantive study population; the paper's target audience is quantitative researchers testing multilevel mediation hypotheses. Its three illustrative reanalyses use: (1) 2,993 sixth-grade students nested in 126 teachers from the Michigan Study of Adolescent Life Transitions (1983-1985); (2) and (3) 429 team members nested in 79 team leaders at a Chinese telecommunications customer-service center."
  where: ["USA", "China"]
  when: "1983-1985 (Example 1, MSALT); data period unreported for Examples 2-3 (customer service center dataset)"
  n: null
  sector: ["education", "telecommunications"]
  sample_notes: >
    The datasets are re-used purely to demonstrate the MSEM technique, not to test SNH-
    relevant hypotheses; no response-rate or representativeness information is given, and
    results should not be read as generalizable substantive findings about leadership,
    teams, or students.
limitation:
  primary: "As a statistical methods paper, its 'results' are illustrative model comparisons on datasets unrelated to social network health (student achievement, team potency, leadership) rather than tests of loneliness, isolation, burnout, or turnover, so its relevance to the project is entirely methodological (how to correctly analyze nested SNH data), not substantive."
  others:
    - "The proposed MSEM framework cannot easily accommodate more than two hierarchical levels and cannot use restricted maximum likelihood estimation for small samples."
    - "Confidence-interval methods for MSEM indirect effects (e.g., the parametric bootstrap used here) were novel and less validated at time of publication than single-level mediation CI methods."
    - "The authors' own examples show that 2-2-1 and 1-1-2 indirect-effect estimates are highly sensitive to modeling choice (MSEM vs. two-step/aggregation), so applied use requires careful, theory-driven specification to avoid analogous over- or under-estimation of effects."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Provides the statistical framework the project would need to correctly test multilevel
  mediation hypotheses common in SNH research -- e.g., whether team-level leadership style
  or organizational culture affects individual burnout or turnover via individual-level
  social support, isolation, or engagement -- without the within/between conflation bias
  that its own examples show can flip a mediation study's substantive conclusion
  (significant vs. null).
tags:
  topic: ["methodology", "measurement"]
  method: ["structural-equation-modeling", "multilevel-modeling", "quantitative"]
  population: ["students", "teams", "employees"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/A General Multilevel SEM Framework for Assessing Multilevel Mediation/A General Multilevel SEM Framework for Assessing Multilevel Mediation.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/A General Multilevel SEM Framework for Assessing Multilevel Mediation.pdf"
  notes: null

---

id: "hughes-2004-a-short-scale-for-measuring-loneliness"
title: "A Short Scale for Measuring Loneliness in Large Surveys"
authors:
  - "Hughes, Mary Elizabeth"
  - "Waite, Linda J."
  - "Hawkley, Louise C."
  - "Cacioppo, John T."
year: 2004
doi: "10.1177/0164027504268574"
venue: {type: "journal", name: "Research on Aging", volume: 26, issue: 6, pages: "655-672"}
citation: "Hughes et al. (2004). A Short Scale for Measuring Loneliness in Large Surveys. Research on Aging, 26(6), 655-672. https://doi.org/10.1177/0164027504268574"
article_type: "methods"
method: {design: "cross-sectional", approach: "survey", evidence_level: "moderate", preregistered: false}
gist: >
  The paper develops and validates a brief Three-Item Loneliness Scale (later known as the
  UCLA-3) suitable for telephone-administered large-scale surveys, distilled from the
  20-item Revised UCLA Loneliness Scale. Using two population-based U.S. samples of older
  adults (HRS, n=2,182; CHASRS, n=229), the scale showed alpha=.72 in both samples and
  correlated .82 with the full R-UCLA. The authors also show that objective indicators of
  social isolation (marital status, living arrangements, volunteering) are significantly but
  only modestly associated with subjective loneliness, indicating the two are related but
  distinct constructs.
claims:
  - text: "The Three-Item Loneliness Scale had internal reliability of alpha=.72 in both the HRS (n=2,182) and CHASRS (n=229) samples, and correlated .82 (p<.001) with the full 20-item R-UCLA Loneliness Scale, showing it reproduces the full scale's construct despite being ten times shorter and telephone-administrable."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["loneliness"]
    predictors: ["sampling-method"]
  - text: "In Study 1 (HRS), all objective isolation indicators were significantly associated with loneliness in the expected direction (e.g., being married: beta=-.42, p<.001; living single and alone: beta=.47, p<.001), but these variables explained no more than 5% of the variance in loneliness scores."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["loneliness"]
    predictors: ["isolation", "social-support"]
  - text: "In Study 2 (CHASRS), the Berkman Social Network Index was inversely correlated with loneliness (beta=-.42, p<.001) on the standardized R-UCLA, replicating the Study 1 pattern that objective and subjective isolation are significantly but only modestly related, supporting the conclusion that they tap distinct aspects of social experience."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["loneliness"]
    predictors: ["isolation", "network-structure"]
population:
  who: "Two U.S. population-based samples of midlife/older adults: 2,182 respondents to HRS Module 6 (2002 wave, nationally representative, born 1947 or earlier, mean age 63.9) and 229 respondents to Year 1 of the Chicago Health, Aging, and Social Relations Study (CHASRS; ages 50-67, White/Black/Hispanic, Cook County, Illinois)."
  where: ["United States"]
  when: "2002 (HRS Module 6); CHASRS Year 1, early-to-mid 2000s"
  n: 2182
  sector: []
  sample_notes: >
    HRS module was assigned to 3,008 potential respondents; 15.6% refused and 11.4% were
    proxy respondents (excluded), yielding a final n=2,182; HRS cohort response rates ranged
    70-80% with 92-95% reinterview rates. CHASRS response rate among eligible households was
    45%, with Black and Hispanic respondents oversampled; participation required an ~8-hour
    lab visit, likely selecting healthier, more mobile older adults (final n=229).
limitation:
  primary: "Validation relies on cross-sectional, single-wave analyses of two U.S. samples of older adults, so the scale's psychometric properties are not established for younger populations, non-U.S. samples, or non-English-speaking respondents."
  others:
    - "CHASRS had only a 45% response rate and required an all-day laboratory visit, likely introducing selection bias toward healthier, more mobile, and more cooperative participants."
    - "Objective isolation indicators (marital status, living arrangement, volunteering, neighborhood safety rating) are proxies rather than direct measures of social contact frequency, limiting interpretation of the modest objective-subjective correlations."
    - "The brief three-item format, while practical for telephone surveys, sacrifices content coverage relative to the full R-UCLA and cannot distinguish loneliness subtypes (e.g., relational vs. collective connectedness)."
risk_of_bias: "medium"
relevance_to_project: >
  This paper is the origin of the widely-used UCLA-3 / Three-Item Loneliness Scale, a
  validated brief instrument (alpha=.72, r=.82 with the full R-UCLA) the SNH project can
  reuse for quick loneliness measurement in remote-worker or community surveys where a full
  20-item instrument is impractical. It also demonstrates that objective isolation proxies
  explain only modest variance (<=5%) in subjective loneliness, supporting the project's
  design choice to measure perceived isolation/belonging directly rather than inferring it
  from contact frequency or headcount alone.
tags:
  topic: ["loneliness", "isolation", "measurement", "social-support"]
  method: ["survey", "cross-sectional"]
  population: ["older-adults", "general-population"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/A Short Scale for Measuring Loneliness in Large Surveys - Results from Two Population-Based Studies/A Short Scale for Measuring Loneliness in Large Surveys - Results from Two Population-Based Studies.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/A Short Scale for Measuring Loneliness in Large Surveys - Results from Two Population-Based Studies.pdf"
  notes: null

---

id: "mackinnon-2004-confidence-limits-for-the-indirect-effect"
title: "Confidence Limits for the Indirect Effect: Distribution of the Product and Resampling Methods"
authors:
  - "MacKinnon, David P."
  - "Lockwood, Chondra M."
  - "Williams, Jason"
year: 2004
doi: "10.1207/s15327906mbr3901_4"
venue: {type: "journal", name: "Multivariate Behavioral Research", volume: 39, issue: 1, pages: "99-128"}
citation: "MacKinnon et al. (2004). Confidence Limits for the Indirect Effect: Distribution of the Product and Resampling Methods. Multivariate Behavioral Research, 39(1), 99-128. https://doi.org/10.1207/s15327906mbr3901_4"
article_type: "methods"
method: {design: "simulation-study", approach: "modelling", evidence_level: "strong", preregistered: false}
gist: >
  This methods paper uses large-scale Monte Carlo simulation to show that the standard
  z-test confidence limits for an indirect (mediated) effect are imbalanced because the
  sampling distribution of a product of two regression coefficients is not normal. It
  evaluates two fixes -- confidence limits based on the distribution of the product (the M
  and empirical-M tests) and six resampling methods (jackknife, percentile/bias-
  corrected/bootstrap-t/bootstrap-Q bootstrap, Monte Carlo) -- and finds the bias-corrected
  bootstrap gives the most accurate coverage and greatest statistical power, illustrated
  with an applied mediation example from a school-based steroid-prevention trial.
claims:
  - text: "Confidence limits for the indirect effect based on the traditional z test (dividing the effect by its multivariate-delta standard error and comparing to the normal distribution) are consistently imbalanced: across 80 simulated combinations of sample size (50-1000) and path effect sizes, the proportion of true values falling outside the confidence interval was almost always below the nominal .025 per tail, indicating reduced statistical power to detect true mediated effects."
    evidence: "simulation-study"
    support_strength: "strong"
    outcomes: ["statistical-power"]
    predictors: ["mediation-analysis"]
  - text: "The distribution-of-product (M) test, which uses critical values from the non-normal distribution of the product of two normal random variables, produced confidence limits closer to the nominal Type I error rate than the z test in nearly all 80 parameter combinations in Study 1, though it was still imperfect for zero/small effect sizes and small samples."
    evidence: "simulation-study"
    support_strength: "strong"
    outcomes: ["statistical-power"]
    predictors: ["mediation-analysis"]
  - text: "Among six resampling methods compared across sample sizes of 25-200 in Study 2, the bias-corrected bootstrap had the best overall performance -- Type I error rates closest to nominal levels and the greatest statistical power -- while the traditional z test and jackknife performed worst (outside robustness criteria 144 and 138 times respectively out of 240 checks, versus 73 for bias-corrected bootstrap)."
    evidence: "simulation-study"
    support_strength: "strong"
    outcomes: ["statistical-power"]
    predictors: ["mediation-analysis"]
population:
  who: "Not a human sample: a Monte Carlo simulation across 80 (Study 1) and 40 (Study 2) combinations of sample size and path effect sizes for a single-mediator regression model; illustrated with an applied example of N=861 high-school football players from the ATLAS anabolic-steroid-prevention program (15 treatment, 16 control schools)."
  where: ["USA"]
  when: "Simulation conducted circa early 2000s; ATLAS example data collected in the 1990s"
  n: 861
  sector: ["academic", "education"]
  sample_notes: >
    Simulation population is entirely synthetic (SAS-generated normal data), so
    representativeness is not applicable to the core method; the illustrative ATLAS example
    is a real but unrelated prevention-trial dataset used only to demonstrate the
    computations, not as a research sample for this paper's own claims.
limitation:
  primary: "Findings are limited to a single indirect-effect model with one mediator and ordinary least-squares regression; extension to indirect effects involving three or more paths (product of three+ random variables) lacks tabled critical values and was not simulated here."
  others:
    - "The paper is silent on conceptual/causal-inference issues in mediation (correct temporal ordering, no omitted variables, no measurement error), assuming the mediation model is correctly specified."
    - "Resampling methods require raw data and more computation, and the 'first law of statistical analysis' problem means different analysts bootstrapping the same data can reach different conclusions."
risk_of_bias: "low"
relevance_to_project: >
  SNH research frequently tests mediation hypotheses (e.g., remote-work intensity ->
  isolation -> burnout, or social support -> belonging -> retention); this paper's finding
  that traditional z-based confidence intervals for indirect effects understate significance
  and that bias-corrected bootstrap or distribution-of-product tests are more accurate
  directly informs which statistical test the project should use/cite when evaluating
  mediator-based claims in the corpus.
tags:
  topic: ["methodology", "measurement"]
  method: ["quantitative", "simulation"]
  population: ["general-population"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Confidence Limits for the Indirect Effect  Distribution of the Product and Resampling Methods/Confidence Limits for the Indirect Effect  Distribution of the Product and Resampling Methods.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Confidence Limits for the Indirect Effect  Distribution of the Product and Resampling Methods.pdf"
  notes: null

---

id: "hidaka-2012-depression-as-a-disease-of-modernity"
title: "Depression as a disease of modernity: Explanations for increasing prevalence"
authors:
  - "Hidaka, Brandon H."
year: 2012
doi: "10.1016/j.jad.2011.12.036"
venue: {type: "journal", name: "Journal of Affective Disorders", volume: 140, issue: 3, pages: "205-214"}
citation: "Hidaka (2012). Depression as a disease of modernity: Explanations for increasing prevalence. Journal of Affective Disorders, 140(3), 205-214. https://doi.org/10.1016/j.jad.2011.12.036"
article_type: "review"
method: {design: "review-scoping", approach: "analytical", evidence_level: "moderate", preregistered: false}
gist: >
  This narrative/evolutionary-medicine review synthesizes epidemiological, cross-cultural,
  and mechanistic evidence to argue that depression prevalence has risen over the past
  century and that this rise reflects a mismatch between the human environment of
  evolutionary adaptedness and modern living. It weighs physical-health drivers (obesity,
  diet, inactivity, light/sleep loss) alongside a 'toxic social environment' of rising
  competition, inequality, and social isolation as candidate mediators, and closes with
  public-health and policy recommendations rather than new primary data.
claims:
  - text: "Longitudinal community studies mostly support rising depression prevalence: U.S. adult one-year MDD prevalence rose from 3.33% to 7.06% between 1991-92 and 2001-02, and young adults in 2007 were 6-8 times more likely than 1938 peers to meet a clinical depression cutoff on MMPI norms; a Swedish cohort found a tenfold increased risk for young adults from 1957-1972 vs. 1947-1957."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["depression"]
    predictors: ["technostress"]
  - text: "Across countries in the World Mental Health Survey initiative, higher GDP per capita (a proxy for modernization) trended toward correlating with greater lifetime risk of a mood disorder (p=0.06), and income inequality (Gini coefficient) correlated significantly with mood-disorder risk in developed countries (p=0.03), consistent with a 'depressiogenic' modern social milieu."
    evidence: "review-scoping"
    support_strength: "low-to-moderate"
    outcomes: ["depression", "mental-health"]
    predictors: ["network-structure"]
  - text: "U.S. General Social Survey data show the mean/mode number of confidants people could discuss important matters with fell from 3/3 in 1985 to 2/0 in 2004 (McPherson et al. 2006); the review cites evidence that loneliness spreads contagiously through social networks (Cacioppo, Fowler & Christakis 2009), framing declining social capital, geographic mobility, and internet use as contributors to isolation and depression risk."
    evidence: "review-scoping"
    support_strength: "low-to-moderate"
    outcomes: ["loneliness", "isolation", "depression"]
    predictors: ["network-structure", "social-support"]
population:
  who: "Not a primary-data study; a narrative review synthesizing dozens of epidemiological, cross-cultural, and clinical studies of depression prevalence and its correlates, spanning community surveys (e.g., NCS, NCS-R, GSS), cross-national cohorts, and small-scale anthropological accounts of traditional/hunter-gatherer societies."
  where: ["United States", "Sweden", "Canada", "China", "Nigeria", "Japan", "cross-national (WHO World Mental Health Survey countries)"]
  when: null
  n: null
  sector: ["general-population"]
  sample_notes: >
    Evidence base is heterogeneous secondary literature (retrospective and longitudinal
    community surveys, cross-cultural comparisons, occasional anthropological case reports);
    author explicitly flags recall bias in retrospective lifetime-prevalence estimates and
    notes some findings (e.g., GDP correlation) are only marginally significant or
    contested.
limitation:
  primary: "As a narrative (non-systematic) review, it selectively synthesizes literature to support an evolutionary-mismatch thesis rather than applying a systematic search/inclusion protocol, and most cited correlational evidence (GDP, inequality, social capital) cannot establish causal contribution to depression trends."
  others:
    - "Author acknowledges the underlying epidemiological evidence for rising depression prevalence itself is conflicting and confounded by recall bias, changing diagnostic criteria, and measurement inconsistency across decades."
    - "Cross-cultural claims about low depression in 'traditional'/hunter-gatherer societies rely on a handful of older anthropological case studies without systematic sampling or validated diagnostic instruments."
    - "Social-environment mechanisms (isolation, inequality, competition) are presented as plausible mediators among many co-occurring modernization factors (diet, sleep, obesity, sunlight) without controlling for confounding between them."
risk_of_bias: "medium"
relevance_to_project: >
  Provides a well-cited evidence trail (GSS confidant decline, Cacioppo/Fowler/Christakis
  network contagion of loneliness, McPherson et al. social isolation in America, Putnam's
  declining social capital) supporting the SNH project's premise that eroding social
  connectedness in modern/industrialized life is a plausible upstream driver of depression,
  useful for framing why interventions on social support and belonging matter for mental-
  health outcomes.
tags:
  topic: ["mental-health", "isolation", "loneliness", "social-support", "community-health"]
  method: ["review", "secondary-data"]
  population: ["general-population", "cross-national"]
source:
  markdown: "Papers_Data/Mental Health/MD/Depression as a Disease of Modernity Explanations for Increasing Prevalence/Depression as a Disease of Modernity Explanations for Increasing Prevalence.md"
  pdf: "papers/Mental Health/Depression as a Disease of Modernity Explanations for Increasing Prevalence.pdf"
  notes: null

---

id: "moussavi-2007-depression-chronic-diseases-and-decrements-in"
title: "Depression, chronic diseases, and decrements in health: results from the World Health Surveys"
authors:
  - "Moussavi, Saba"
  - "Chatterji, Somnath"
  - "Verdes, Emese"
  - "Tandon, Ajay"
  - "Patel, Vikram"
  - "Ustun, Bedirhan"
year: 2007
doi: "10.1016/s0140-6736(07)61415-9"
venue: {type: "journal", name: "The Lancet", volume: 370, issue: 9590, pages: "851-858"}
citation: "Moussavi et al. (2007). Depression, chronic diseases, and decrements in health: results from the World Health Surveys. The Lancet, 370(9590), 851-858. https://doi.org/10.1016/s0140-6736(07)61415-9"
article_type: "empirical"
method: {design: "cross-sectional", approach: "survey", evidence_level: "strong", preregistered: false}
gist: >
  Using WHO World Health Survey data from 245,404 adults in 60 countries, this study
  directly compares the health-decrement effect of depression against four common chronic
  physical diseases (angina, arthritis, asthma, diabetes). Depression alone was associated
  with the lowest health scores of any single condition, and depression comorbid with a
  chronic physical disease produced the steepest decrements of all, including a specific
  interactive worsening effect when comorbid with diabetes. The authors argue depression
  should be treated as a public-health priority on par with major chronic physical illness.
claims:
  - text: "Respondents with depression alone had a mean health score of 72.9, the lowest of any single chronic condition, versus 90.6 for respondents with no disease and 78.9-80.3 for angina, arthritis, asthma, or diabetes alone (p<0.0001); regression-adjusted, depression alone carried a coefficient of -13.89 versus -3.53 to -6.68 for the physical diseases alone."
    evidence: "cross-sectional"
    support_strength: "strong"
    outcomes: ["mental-health", "wellbeing"]
    predictors: ["sampling-method"]
  - text: "Depression was highly comorbid with chronic physical disease: 9.3% of respondents with diabetes, 10.7% with arthritis, 15.0% with angina, and 18.1% with asthma also had depression, and 23% of those with two or more chronic conditions had comorbid depression, all significantly higher than the 3.2% baseline depression prevalence in those without chronic disease (p<0.0001)."
    evidence: "cross-sectional"
    support_strength: "strong"
    outcomes: ["mental-health"]
    predictors: ["sampling-method"]
  - text: "Comorbid depression produced the largest health decrements of any disease combination, with regression coefficients ranging from -16.77 (depression+arthritis) to -23.43 (depression+diabetes) and -24.38 for depression plus two or more chronic conditions (mean health score 56.1), substantially worse than two or more chronic conditions without depression (coefficient -11.97, mean score 71.8), suggesting an interactive rather than purely additive effect, particularly with diabetes."
    evidence: "cross-sectional"
    support_strength: "strong"
    outcomes: ["mental-health", "wellbeing"]
    predictors: ["sampling-method"]
population:
  who: "General adult population (18+) surveyed via the WHO World Health Survey, standardised face-to-face (or telephone in Luxembourg/Israel) interviews"
  where: ["Global (60 countries across Africa, Americas, Europe, Eastern Mediterranean, Southeast Asia, Western Pacific)"]
  when: "2003"
  n: 245404
  sector: ["healthcare", "public-health"]
  sample_notes: >
    Nationally representative, probabilistically sampled countries with post-stratification
    weighting; regression analysis restricted to a pooled 46-country subset (n=142,755) that
    administered the long-form questionnaire including diabetes items; disease diagnoses
    derived from validated symptom algorithms calibrated against a smaller diagnostic item
    probability study in 7 countries.
limitation:
  primary: "Cross-sectional design precludes causal inference about onset, duration, or treatment effects, and cannot establish whether depression causes health decline or vice versa."
  others:
    - "Diabetes prevalence relied on self-reported prior diagnosis, likely underestimating true prevalence and introducing reporting bias."
    - "Asthma and arthritis diagnostic algorithms were validated only in a small multi-country study and could benefit from broader validation."
    - "Self-report of health and depression symptoms may be subject to reporting bias driven by depressed mood itself, though the authors' vignette and recursive-regression checks did not find evidence of this."
risk_of_bias: "low"
relevance_to_project: >
  Provides strong population-level evidence, from a very large multi-country sample, that
  depression degrades self-rated health/wellbeing more than common chronic physical diseases
  and that comorbid depression compounds decline non-additively -- useful as a baseline
  evidence anchor when the SNH project frames mental-health/depression outcomes as a first-
  order concern alongside physical health in remote-worker or community wellbeing measures.
tags:
  topic: ["mental-health", "wellbeing", "measurement"]
  method: ["cross-sectional", "survey"]
  population: ["general-population", "global"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Depression Chronic Diseases and Decrements in Health Results from the World Health Surveys/Depression Chronic Diseases and Decrements in Health Results from the World Health Surveys.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Depression Chronic Diseases and Decrements in Health Results from the World Health Surveys.pdf"
  notes: null

---

id: "fried-2015-depression-is-not-a-consistent-syndrome"
title: "Depression is not a consistent syndrome: An investigation of unique symptom patterns in the STAR*D study"
authors:
  - "Fried, Eiko I."
  - "Nesse, Randolph M."
year: 2015
doi: "10.1016/j.jad.2014.10.010"
venue: {type: "journal", name: "Journal of Affective Disorders", volume: 172, issue: null, pages: "96-102"}
citation: "Fried et al. (2015). Depression is not a consistent syndrome: An investigation of unique symptom patterns in the STAR*D study. Journal of Affective Disorders, 172, 96-102. https://doi.org/10.1016/j.jad.2014.10.010"
article_type: "empirical"
method: {design: "cross-sectional", approach: "secondary-data", evidence_level: "moderate", preregistered: false}
gist: >
  Analyzing baseline data from 3703 depressed outpatients in the STAR*D trial, the authors
  show that DSM-5 symptom-based diagnoses of major depressive disorder mask enormous
  heterogeneity: 1030 distinct symptom profiles emerged, nearly half endorsed by only a
  single person, and this heterogeneity persisted even after controlling for overall
  severity. The paper argues that summing symptoms into a single severity score obscures
  qualitatively different presentations of 'depression,' which may help explain inconsistent
  treatment-efficacy findings and motivates analyzing individual symptoms and their causal
  networks rather than relying on sum-scores alone.
claims:
  - text: "Among 3703 depressed outpatients in the STAR*D baseline sample, 1030 unique DSM-5 symptom profiles were identified; 864 profiles (83.9%) were endorsed by five or fewer participants and 501 (48.6%) by only one individual, with the single most common profile occurring in just 1.8% of the sample."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["mental-health", "depression"]
    predictors: ["symptom-profile-heterogeneity"]
  - text: "Restricting the analysis to 569 participants who all had the same overall symptom count (the sample median of 6) still produced 188 unique profiles, with 86.2% endorsed by five or fewer people and 51.6% endorsed by only one person, showing the heterogeneity is not merely an artifact of severity differences between patients."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["mental-health", "depression"]
    predictors: ["symptom-profile-heterogeneity"]
  - text: "The authors argue that because patients with identical sum-scores can share almost no symptoms in common, standard sum-score depression measures (e.g., HAM-D, BDI) likely misrepresent psychosocial impairment and may partly explain the field's difficulty documenting consistent antidepressant treatment efficacy."
    evidence: "cross-sectional"
    support_strength: "low-to-moderate"
    outcomes: ["mental-health", "depression"]
    predictors: ["symptom-measurement-approach"]
population:
  who: "3703 nonpsychotic MDD outpatients (mean age 41.2, 63% female) enrolled in the first treatment stage of the STAR*D trial, all receiving citalopram; recruited via relatively inclusive criteria to be representative of treatment-seeking MDD patients"
  where: ["United States"]
  when: null
  n: 3703
  sector: []
  sample_notes: >
    Multisite NIH-sponsored RCT across 14 US institutions with broad inclusion criteria (age
    18-75, DSM-IV nonpsychotic MDD, HAM-D >=14) intended to maximize representativeness of
    real-world treatment-seeking depressed outpatients; excluded
    bipolar/psychotic/schizoaffective disorders, certain eating disorders, and treatment-
    refractory cases. Symptom data drawn from telephone-administered QIDS-16 during the
    first week of treatment.
limitation:
  primary: "Symptoms were dichotomized into present/absent from a 4-point severity scale to construct profiles, which likely inflates the apparent number of distinct profiles and discards within-symptom severity information."
  others:
    - "The QIDS-16 assesses most MDD symptoms with only a single item, so item wording could have biased which profiles emerged."
    - "Analysis was limited to 12 symptoms derived from the 9 DSM-5 criteria, likely underestimating true heterogeneity by excluding clinically relevant non-criterion symptoms such as anxiety, anger, and helplessness."
    - "Many participants had comorbid medical conditions and were taking other medications that may have influenced symptom presentation independent of depression itself."
risk_of_bias: "medium"
relevance_to_project: >
  This paper is a methodological caution rather than an SNH-specific study: it demonstrates
  that sum-score approaches to mental-health measurement (as commonly used in
  wellbeing/burnout surveys) can conflate qualitatively different experiences under one
  number, which is directly relevant to how the SNH project should design and interpret any
  depression, burnout, or distress screening instruments used with remote workers or
  maintainers.
tags:
  topic: ["mental-health", "measurement", "methodology"]
  method: ["cross-sectional", "secondary-data"]
  population: ["clinical-population", "adults"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Depression is Not a Consistent Syndrome An Investigation of Unique Symptom Patterns in the STAR-D Study/Depression is Not a Consistent Syndrome An Investigation of Unique Symptom Patterns in the STAR-D Study.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Depression is Not a Consistent Syndrome An Investigation of Unique Symptom Patterns in the STAR-D Study.pdf"
  notes: null

---

id: "murray-2007-design-and-analysis-of-group-randomized"
title: "Design and Analysis of Group-Randomized Trials"
authors:
  - "Murray, David M"
year: 2007
doi: "10.1093/oso/9780195120363.001.0001"
venue: {type: "book", name: null, volume: null, issue: null, pages: null}
citation: "Murray (2007). Design and Analysis of Group-Randomized Trials.. https://doi.org/10.1093/oso/9780195120363.001.0001"
article_type: "methods"
method: {design: "theory", approach: "analytical", evidence_level: "reference", preregistered: false}
gist: >
  This is a training slide deck by David Murray (NIH OBSSR) on the design and analysis of
  group-randomized trials (GRTs) and individually randomized group treatment trials (IRGTs)
  — designs where an intervention is delivered to intact groups (worksites, clinics,
  communities, small treatment groups) rather than to independent individuals. It explains
  why the intraclass correlation (ICC) among members of the same group inflates variance and
  Type I error when analyses ignore the nested structure, and lays out which analytic
  strategies (mixed-model ANOVA/ANCOVA, random coefficients models, GEE, randomization
  tests) preserve valid inference. It is a methodological reference for anyone planning to
  evaluate a group- or community-level intervention rather than an empirical SNH study
  itself.
claims:
  - text: "Analyzing data from a group-randomized or individually-randomized-group-treatment trial as if participants were independently randomized (ignoring the positive intraclass correlation among group members) inflates the Type I error rate — often to 30-50% in GRTs and 15-25% in IRGTs — even when the ICC is small."
    evidence: "theory"
    support_strength: "moderate"
    outcomes: ["type-i-error-rate"]
    predictors: ["intraclass-correlation", "network-structure"]
  - text: "The design effect (DEFF), which quantifies how much variance is inflated by clustering, rises sharply with both the ICC and the number of members per group; worked examples show DEFF reaching 25.95 for a GRT with ICC=0.05 and 500 members per group, meaning statistical power collapses unless this is accounted for at the design stage."
    evidence: "theory"
    support_strength: "moderate"
    outcomes: ["type-i-error-rate"]
    predictors: ["intraclass-correlation", "network-structure"]
  - text: "Mixed-model ANOVA/ANCOVA (General or Generalized Linear Mixed Model) maintains nominal Type I error rates across a wide range of GRT conditions when there are one or two measurement time points, but has an inflated Type I error rate when group-specific trends are heterogeneous over three or more time points — in which case random coefficients (growth curve) models are recommended instead."
    evidence: "theory"
    support_strength: "moderate"
    outcomes: ["type-i-error-rate"]
    predictors: ["study-design", "cluster-randomization"]
population:
  who: "No original human sample; a statistical-methods lecture illustrating GRT/IRGT design and analysis using examples from named NIH-funded trials (e.g., the Health Care Systems Collaboratory's 7 pragmatic trials, the Childhood Obesity Prevention and Treatment Research studies) and citations to prior simulation work."
  where: ["USA"]
  when: "2015"
  n: null
  sector: ["healthcare", "academia"]
  sample_notes: >
    Conference/training slide deck (2015 OBSSR Summer Institute); presents no original data
    collection, only worked formulas, illustrative tables, and references to prior published
    simulation studies (e.g., Gail et al. 1996; Varnell et al. 2001) to support its
    recommendations.
limitation:
  primary: "As a slide-deck training presentation rather than a peer-reviewed paper, its claims are stated without full methodological detail and rely on citing prior primary/simulation studies by author-year rather than reproducing their results."
  others:
    - "Not an empirical or SNH-specific study — it is general statistical methodology for cluster/group-randomized designs applicable to any group-level health intervention, not specifically to remote work, isolation, or social network health."
    - "Several illustrative figures (power/precision tradeoffs, design diagrams) are embedded images not captured as text in this conversion, limiting reproducibility of some numeric examples."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Directly useful if the SNH project ever evaluates a team-, org-, or community-level
  intervention (e.g., a manager-training or community-engagement program rolled out to whole
  teams) rather than randomizing individuals: it explains why individual-level analysis of
  such designs produces false-positive intervention effects and prescribes the mixed-model,
  random-coefficients, and GEE approaches needed for valid inference and power calculations
  in that scenario.
tags:
  topic: ["methodology", "measurement"]
  method: ["theory"]
  population: ["research-methodologists"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Design and Analysis of Group-Randomized Trials - Murray 2015 OBSSR Summer Institute/Design and Analysis of Group-Randomized Trials - Murray 2015 OBSSR Summer Institute.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Design and Analysis of Group-Randomized Trials - Murray 2015 OBSSR Summer Institute.pdf"
  notes: null

---

id: "wyman-2014-developmental-approach-to-prevent-adolescent-suicides"
title: "Developmental Approach to Prevent Adolescent Suicides"
authors:
  - "Wyman, Peter A."
year: 2014
doi: "10.1016/j.amepre.2014.05.039"
venue: {type: "journal", name: "American Journal of Preventive Medicine", volume: 47, issue: 3, pages: "S251-S256"}
citation: "Wyman (2014). Developmental Approach to Prevent Adolescent Suicides. American Journal of Preventive Medicine, 47(3), S251-S256. https://doi.org/10.1016/j.amepre.2014.05.039"
article_type: "commentary"
method: {design: "review-scoping", approach: "analytical", evidence_level: "low-to-moderate", preregistered: false}
gist: >
  This perspective piece from the National Action Alliance for Suicide Prevention's Research
  Prioritization Task Force proposes a developmentally sequenced model for preventing
  adolescent suicide: childhood programs that strengthen self-regulation (e.g., the Good
  Behavior Game, which cut suicide attempts by half at ages 19-21 in a landmark classroom
  RCT) followed by adolescent programs that leverage peer and family influence to curb
  substance abuse, bullying, and disconnection. It argues that upstream, universal
  interventions delivered through schools and families have greater population-level
  suicide-prevention potential than downstream identify-and-treat approaches, and lays out
  short-term (4-8 year) and long-term (12-20 year) research pathways -- pooling existing
  trial data, adding suicide-behavior measures to ongoing prevention trials, and running
  large community-randomized trials -- to establish causal links between specific
  interventions and reduced suicide mortality.
claims:
  - text: "In a rigorous RCT, the Good Behavior Game delivered by teachers in first- and second-grade urban classrooms reduced self-reported suicidal ideation and attempts by roughly half when assessed 15 years later, at ages 19-21; a less-rigorously implemented version in a second cohort showed a directionally similar but nonsignificant effect."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation"]
    predictors: ["intervention"]
  - text: "A randomized trial of the New Beginnings Program for divorcing families found that strengthening parenting and child coping skills reduced adolescent mental health disorders, substance use, and behavioral problems, with positive effects increasing over time -- but, as with nearly all youth prevention trials besides the Good Behavior Game, suicidal behavior itself was never assessed as an outcome."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["mental-health"]
    predictors: ["intervention", "leadership-style"]
  - text: "Youth in juvenile justice facilities have a suicide rate approximately three times that of the general youth population, yet only about 0.25% of U.S. youth are in such facilities at any given time -- meaning interventions confined to reparative/high-risk settings cannot substantially reduce population-level suicide rates on their own."
    evidence: "cross-sectional"
    support_strength: "low-to-moderate"
    outcomes: ["suicidal-ideation"]
    predictors: ["intervention"]
population:
  who: "Not a single sampled population; a narrative synthesis of completed and proposed youth-focused preventive intervention trials in the U.S. (e.g., Good Behavior Game in urban first/second-grade classrooms; New Beginnings Program with divorcing families; Sources of Strength peer-leader program in high schools), framed as a developmental pipeline from childhood through adolescence."
  where: ["United States"]
  when: null
  n: null
  sector: ["education", "healthcare"]
  sample_notes: >
    No original sample; population claims are drawn selectively from cited prior trials
    (e.g., Kellam et al. 2008 GBG cohort; Wolchik et al. 2002 NBP cohort) rather than from a
    systematic search or pooled reanalysis.
limitation:
  primary: "This is a narrative perspective/research-agenda article, not a systematic review -- it does not use a documented search or quality-appraisal method, and its evidence base is a selective set of trials, several from the author's own group."
  others:
    - "Only the Good Behavior Game has been rigorously tested for suicide-specific outcomes; most other cited programs (NBP, Life Skills, Olweus, Communities That Care) only assessed proximal risk factors, not suicidal behavior or mortality."
    - "The proposed developmental model and its long-term (12-20 year) research pathway are conceptual recommendations, not empirically validated, and depend on future trials that had not yet been conducted."
risk_of_bias: "medium"
relevance_to_project: >
  For SNH's upstream/prevention framing, this paper offers a template for building a
  developmental, systems-level (family, school, peer, community) prevention pipeline rather
  than relying on individual-level identify-and-treat detection -- directly relevant to
  designing peer-network connectedness interventions (e.g., the Sources of Strength model
  referenced here) and to arguing for population-level, universal supports over narrowly
  targeted high-risk outreach.
tags:
  topic: ["suicide-prevention", "mental-health", "community-health"]
  method: ["review-scoping"]
  population: ["adolescents", "school-based"]
source:
  markdown: "Papers_Data/Mental Health/MD/Developmental Approach to Prevent Adolescent Suicides Research Pathways to Effective Upstream Preventive Interventions/Developmental Approach to Prevent Adolescent Suicides Research Pathways to Effective Upstream Preventive Interventions.md"
  pdf: "papers/Mental Health/Developmental Approach to Prevent Adolescent Suicides Research Pathways to Effective Upstream Preventive Interventions.pdf"
  notes: null

---

id: "petras-2008-developmental-epidemiological-courses-leading-to-antisocial"
title: "Developmental epidemiological courses leading to antisocial personality disorder and violent and criminal behavior: Effects by young adulthood of a universal preventive intervention in first- and second-grade classrooms"
authors:
  - "Petras, Hanno"
  - "Kellam, Sheppard G."
  - "Brown, C. Hendricks"
  - "Muthén, Bengt O."
  - "Ialongo, Nicholas S."
  - "Poduska, Jeanne M."
year: 2008
doi: "10.1016/j.drugalcdep.2007.10.015"
venue: {type: "journal", name: "Drug and Alcohol Dependence", volume: 95, issue: null, pages: "S45-S59"}
citation: "Petras et al. (2008). Developmental epidemiological courses leading to antisocial personality disorder and violent and criminal behavior: Effects by young adulthood of a universal preventive intervention in first- and second-grade classrooms. Drug and Alcohol Dependence, 95, S45-S59. https://doi.org/10.1016/j.drugalcdep.2007.10.015"
article_type: "empirical"
method: {design: "rct", approach: "experiment", evidence_level: "strong", preregistered: false}
gist: >
  Reports young-adult (age 19-21) follow-up of the Baltimore Good Behavior Game (GBG)
  trials, a randomized classroom behavior-management intervention delivered in first and
  second grade. Using growth mixture modeling, the paper identifies three developmental
  trajectories of aggressive/disruptive behavior (persistent-high, escalating/persistent-
  medium, stable-low) and shows GBG substantially cut later antisocial personality disorder
  (ASPD) and violent/criminal behavior among high-risk males in the original effectiveness
  cohort, but the effect weakened and lost significance in a replication cohort delivered
  with less teacher training and monitoring. The paper's core contribution is evidence that
  a low-cost, universal, group-contingency classroom intervention targeting early social-
  field behavior norms can alter life-course antisocial trajectories in a defined high-risk
  subgroup, contingent on implementation fidelity.
claims:
  - text: "Among Cohort 1 males in the persistent-high aggression trajectory, 40.1% of GBG-classroom males were diagnosed with ASPD by young adulthood versus 100% of control-classroom males, a significant reduction (chi-square = 17.18, df = 1, p < 0.001); effects on escalating-medium and stable-low males were smaller and not significant."
    evidence: "rct"
    support_strength: "strong"
    outcomes: ["mental-health", "antisocial-personality-disorder"]
    predictors: ["intervention", "peer-mentoring"]
  - text: "Combined ASPD and violent/criminal-record outcomes were also significantly reduced in Cohort 1 persistent-high males (34% of GBG males had both outcomes or ASPD alone vs. 50%/50% of controls; chi-square = 25.062, df = 3, p < 0.001), but in the Cohort 2 replication -- run with the same teachers but markedly less mentoring/monitoring of implementation -- the young-adult effect on ASPD and violent/criminal behavior was non-significant, though in the hypothesized direction (chi-square = 0.997, df = 3, p = 0.80), despite a significant GBG effect on the behavior trajectory itself through 7th grade."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["mental-health", "antisocial-personality-disorder"]
    predictors: ["intervention"]
  - text: "GBG impact on young-adult outcomes was not significant for females in either cohort (e.g., Cohort 1 persistent-high females: 38.7% GBG vs. 50.6% control ASPD diagnosis, p = 0.71; a zero-impact model fit best, chi-square = 3.298, df = 3, p = 0.35), attributed to females' much lower baseline prevalence of persistent-high aggression and ASPD/violent outcomes, limiting statistical power."
    evidence: "rct"
    support_strength: "low"
    outcomes: ["mental-health"]
    predictors: ["intervention", "sampling-method"]
population:
  who: "First-grade students (mean age ~6.4) from 19 Baltimore City Public Schools in five urban, poor-to-lower-middle-income, predominantly African-American areas, randomized at the classroom/school level to the Good Behavior Game, a reading-mastery program, or standard practice, and followed to age 19-21."
  where: ["United States (Baltimore, Maryland)"]
  when: "Two first-grade cohorts recruited in the 1985-1986 and 1986-1987 school years, with young-adult outcomes assessed at age 19-21 and criminal-record searches continuing through February 2006"
  n: 768
  sector: ["education", "public-health"]
  sample_notes: >
    Analytic sample of 768 (403 Cohort 1 / 365 Cohort 2) drawn from an original pool of 2311
    first-graders after excluding students in intervention arms not relevant to this paper
    and those without valid teacher ratings; 76-77% of each cohort contributed young-adult
    follow-up data. Key subgroup analyses (e.g., persistent-high aggression class) involve
    small strata (e.g., 14-18% of males, 8-9% of females), reducing power, especially for
    females and for the Cohort 2 replication.
limitation:
  primary: "Significant benefits on adult ASPD and violent/criminal behavior were confined to a small high-risk male subgroup in the original effectiveness trial; the Cohort 2 replication -- delivered with reduced teacher training and monitoring -- reproduced the behavioral trajectory effect but not the significant young-adult diagnostic/criminal-record effect, so durability of impact appears contingent on implementation fidelity rather than guaranteed by the intervention alone."
  others:
    - "Female analyses were underpowered given females' much lower base rates of persistent-high aggression and of ASPD/violent-crime outcomes, so null findings for females cannot be read as evidence of no effect."
    - "Missing data (up to ~24% non-follow-up plus item-level attrition) required model-based full-information maximum-likelihood adjustment under a missing-at-random assumption that cannot be directly verified."
    - "Violent/criminal outcomes relied on Baltimore juvenile court and Maryland Department of Correction records, which would miss offenses or incarceration occurring after relocation out of the study's jurisdiction."
risk_of_bias: "medium"
relevance_to_project: >
  As a foundational developmental-epidemiology/prevention-science trial, this paper offers a
  template for the SNH project's interest in upstream, group-level interventions: it shows a
  low-cost, universal, peer-reinforced 'social field' intervention (classroom teams and
  rewards) can shift long-term wellbeing/behavioral trajectories in a defined at-risk
  subgroup, while also demonstrating that intervention fidelity and mentoring of
  implementers (here, teachers; analogously, managers or community leads) are decisive
  moderators of whether benefits persist -- a direct caution for designing and evaluating
  any SNH team- or community-level intervention.
tags:
  topic: ["mental-health", "community-health", "methodology"]
  method: ["rct", "longitudinal"]
  population: ["children", "low-income", "urban-communities"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Developmental Epidemiological Courses Leading to Antisocial Personality Disorder and Violent Criminal Behavior/Developmental Epidemiological Courses Leading to Antisocial Personality Disorder and Violent Criminal Behavior.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Developmental Epidemiological Courses Leading to Antisocial Personality Disorder and Violent Criminal Behavior.pdf"
  notes: null

---

id: "gratz-2008-multidimensional-assessment-of-emotion-regulation-and"
title: "Multidimensional Assessment of Emotion Regulation and Dysregulation: Development, Factor Structure, and Initial Validation of the Difficulties in Emotion Regulation Scale"
authors:
  - "Gratz, Kim L."
  - "Roemer, Lizabeth"
year: 2008
doi: "10.1007/s10862-008-9102-4"
venue: {type: "journal", name: "Journal of Psychopathology and Behavioral Assessment", volume: 30, issue: 4, pages: "315-315"}
citation: "Gratz et al. (2008). Multidimensional Assessment of Emotion Regulation and Dysregulation: Development, Factor Structure, and Initial Validation of the Difficulties in Emotion Regulation Scale. Journal of Psychopathology and Behavioral Assessment, 30(4), 315-315. https://doi.org/10.1007/s10862-008-9102-4"
article_type: "methods"
method: {design: "cross-sectional", approach: "survey", evidence_level: "moderate", preregistered: false}
gist: >
  Reports development and initial psychometric validation of the Difficulties in Emotion
  Regulation Scale (DERS), a 36-item self-report measure built on an integrative,
  multidimensional conceptualization of emotion regulation (awareness, clarity, acceptance,
  impulse control, goal-directed behavior, and access to effective strategies). Across two
  undergraduate samples, exploratory factor analysis yielded six correlated factors, the
  scale showed high internal consistency and good test-retest reliability, and DERS scores
  predicted deliberate self-harm and (among men) intimate partner abuse beyond an existing
  mood-regulation measure. The paper contributes a validated, multidimensional instrument
  for measuring emotion dysregulation rather than treating it as a single global construct.
claims:
  - text: "Exploratory factor analysis of 357 undergraduates identified six interpretable, correlated factors (Nonacceptance, Goals, Impulse, Awareness, Strategies, Clarity) accounting for 55.68% of variance; the final 36-item DERS had high overall internal consistency (Cronbach's alpha = .93) and all six subscales had alpha > .80."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["mental-health"]
    predictors: ["emotion-regulation"]
  - text: "The DERS overall score showed good test-retest reliability over 4-8 weeks in a 21-person subsample (intraclass correlation = .88, p < .01), with subscale test-retest correlations ranging from .57 (Impulse) to .89 (Strategies), and construct validity was supported by significant correlations with an existing mood-regulation measure (r = -.69), experiential avoidance (r = .60), and emotional expressivity (r = -.23), all in the expected direction."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["mental-health", "stress"]
    predictors: ["emotion-regulation"]
  - text: "DERS overall scores were significantly correlated with frequency of deliberate self-harm among both women (r = .20) and men (r = .26), and with frequency of intimate partner abuse among men (r = .34) but not women (r = .08); the Goals subscale uniquely predicted partner-abuse frequency among men (r = .37) even after controlling for the existing mood-regulation measure."
    evidence: "cross-sectional"
    support_strength: "low-to-moderate"
    outcomes: ["mental-health"]
    predictors: ["emotion-regulation"]
population:
  who: "Undergraduate psychology students at a US urban public university, drawn as two separate samples: one for factor analysis, reliability, and validity testing, and a second, smaller subsample for test-retest reliability."
  where: ["United States"]
  when: "Data collected prior to 2003 publication (exact year not stated)"
  n: 357
  sector: ["higher-education"]
  sample_notes: >
    Main sample: 373 of 479 distributed packets returned (78% response rate), 357 retained
    after excluding incomplete cases; 73% female, 65% White, mean age 23.1. No significant
    differences found between responders and non-responders. Test-retest subsample was a
    separate convenience sample of 194 recruited from campus public areas, of whom only 21
    completed a second DERS administration 4-8 weeks later for a small monetary incentive;
    that subsample was 62% female and 67% White.
limitation:
  primary: "Test-retest reliability is estimated from a very small subsample (n = 21) recruited opportunistically for an unrelated study, so this key reliability estimate needs replication with a larger sample."
  others:
    - "Both samples were predominantly White, female, nonclinical undergraduates, so generalizability to men, other racial/ethnic groups, and clinical populations (e.g., borderline personality disorder) is untested."
    - "Construct validity relies on only a few self-report measures of emotional responding; no physiological or observer-rated indices were included."
    - "Predictive validity was examined for only two behavioral outcomes (self-harm, partner abuse) chosen partly on theoretical/convenience grounds, not a broad range of clinically relevant behaviors."
risk_of_bias: "medium"
relevance_to_project: >
  The DERS is a widely used, multidimensional measure of emotion dysregulation whose
  subscales (especially limited access to regulation strategies and difficulty with goal-
  directed behavior under distress) offer the SNH project ready-made, validated constructs
  for measuring individual-level emotion-regulation deficits that could mediate or moderate
  links between social isolation, workplace stress, and burnout or self-harm risk in remote-
  worker or maintainer populations.
tags:
  topic: ["mental-health", "measurement", "methodology"]
  method: ["cross-sectional", "survey"]
  population: ["general-population"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Difficulties in Emotion Regulation Scale - Development Factor Structure and Validation/Difficulties in Emotion Regulation Scale - Development Factor Structure and Validation.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Difficulties in Emotion Regulation Scale - Development Factor Structure and Validation.pdf"
  notes: null

---

id: "ali-2015-disease-prevention-and-health-promotion"
title: "Disease Prevention and Health Promotion"
authors:
  - "Ali, Ather"
  - "Katz, David L."
year: 2015
doi: "10.1016/j.amepre.2015.07.019"
venue: {type: "journal", name: "American Journal of Preventive Medicine", volume: 49, issue: 5, pages: "S230-S240"}
citation: "Ali et al. (2015). Disease Prevention and Health Promotion. American Journal of Preventive Medicine, 49(5), S230-S240. https://doi.org/10.1016/j.amepre.2015.07.019"
article_type: "commentary"
method: {design: "theory", approach: "analytical", evidence_level: "speculative", preregistered: false}
gist: >
  This conceptual paper by Ali and Katz argues that integrative medicine (the blending of
  conventional care with complementary and alternative medicine, CAM) maps naturally onto
  the primary/secondary/tertiary prevention framework, and proposes an evidence-based
  decision framework (safety, effectiveness, quality of evidence, alternatives, cost, and
  patient preference) for deciding when to recommend CAM therapies despite frequently weak
  or mixed supporting evidence. It contributes a general model for balancing rigorous
  evidence standards against patient-centered care and preference under uncertainty, which
  is analogous to how the SNH project must weigh weak-evidence but plausible interventions
  (e.g., informal peer support, community rituals) against formal, better-evidenged
  programs.
claims:
  - text: "Roughly one third of the U.S. adult population and 12% of children have used at least one CAM therapy, yet fewer than 40% of CAM-using patients disclose this use to their conventional physicians, indicating a substantial patient-provider communication gap."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["communication", "help-seeking"]
    predictors: ["organizational-culture"]
  - text: "The authors propose a Clinical Applications of Research Evidence framework in which recommendation decisions weigh safety, efficacy, quality/quantity of evidence, availability of alternative treatments, cost/accessibility, and patient preference jointly, rather than requiring definitive evidence before any therapy can be offered, particularly for conditions (e.g., fibromyalgia, chronic fatigue syndrome) that lack a definitive conventional therapy."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["wellbeing"]
    predictors: ["intervention"]
  - text: "Psychological stress is described as having robust, broad-based negative effects on infectious and chronic disease, morbidity, mortality, and recovery, while positive emotional states and personality traits such as internal locus of control and sense of meaningfulness are associated with decreased illness in high-stress environments."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["stress", "wellbeing", "mental-health"]
    predictors: ["hope", "psychological-safety"]
population:
  who: "Not an empirical study of a sample; a conceptual/policy paper synthesizing prior epidemiological and clinical-effectiveness literature on CAM/integrative medicine use in the general U.S. population"
  where: ["United States"]
  when: "Synthesizes literature published roughly 1988-2015"
  n: null
  sector: ["healthcare"]
  sample_notes: >
    No primary data collection; population figures (e.g., one-third of adults using CAM) are
    drawn secondhand from cited national health surveys (e.g., NHIS-based reports), not
    generated by this paper.
limitation:
  primary: "The paper is explicitly conceptual/argumentative rather than empirical: it acknowledges 'the relative deficiency of research on the effectiveness of practice-based integrative care' and does not itself test or quantify outcomes."
  others:
    - "Relies heavily on the authors' own prior commissioned IOM paper and decision framework, which is asserted rather than validated against outcomes data."
    - "Evidence cited for specific CAM therapies (e.g., CoQ10, licorice, probiotics) is a mix of positive and null findings presented narratively rather than via systematic synthesis."
risk_of_bias: "not-applicable"
relevance_to_project: >
  The paper's evidence-vs-preference decision framework (safety, efficacy, quality of
  evidence, alternatives, cost, patient preference) is a useful analogy for the SNH
  project's own dilemma of recommending weakly-evidenced but plausible social-connection
  interventions (peer support, informal rituals) when rigorous RCT evidence is sparse; its
  discussion of stress, positive emotion, and locus-of-control as protective factors is also
  relevant to designing wellbeing-oriented interventions.
tags:
  topic: ["wellbeing", "mental-health", "measurement"]
  method: ["theory", "review-scoping"]
  population: ["healthcare"]
source:
  markdown: "Papers_Data/Mental Health/MD/Disease Prevention and Health Promotion How Integrative Medicine Fits/Disease Prevention and Health Promotion How Integrative Medicine Fits.md"
  pdf: "papers/Mental Health/Disease Prevention and Health Promotion How Integrative Medicine Fits.pdf"
  notes: null

---

id: "anon-2008-drug-and-alcohol-dependence-purpose-and"
title: "Drug and Alcohol Dependence: Purpose and Scope / Editorial Board"
authors:
year: 2008
doi: null
venue: {type: "journal", name: "Drug and Alcohol Dependence (Elsevier Ireland Ltd.)", volume: null, issue: null, pages: null}
citation: "Drug and Alcohol Dependence (Elsevier Ireland Ltd.) (2008). Drug and Alcohol Dependence: Purpose and Scope / Editorial Board. Drug and Alcohol Dependence (Elsevier Ireland Ltd.)."
article_type: "commentary"
method: {design: "theory", approach: "other", evidence_level: "reference", preregistered: false}
gist: >
  This is journal front matter for Drug and Alcohol Dependence, not a research article: it
  states the journal's aims and scope (chemistry, pharmacology, epidemiology, sociology, and
  economics of drug, alcohol, and tobacco use/dependence), lists accepted article types,
  authorship and conflict-of-interest policies, and lists the editor-in-chief, associate
  editors, and international editorial board as of 2008. It contains no data, findings, or
  claims relevant to social network health.
claims:
  - text: "The journal explicitly states its scope covers etiology, epidemiology, prevention, and policy research on drug, alcohol, and tobacco use/dependence, spanning molecular, clinical, and social-science (sociology, economics) methods, but does not include social network health, remote work, or workplace wellbeing as topics."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["mental-health"]
    predictors: ["intervention"]
  - text: "The masthead lists three accepted manuscript types (full-length reports, review articles, short communications) and requires authors to disclose funding, conflicts of interest, and ethical compliance, per the Farmington Consensus Statement."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["mental-health"]
    predictors: ["intervention"]
population:
  who: "Not applicable: this document is a journal's editorial masthead (editor-in-chief, associate editors, ~40-member international editorial board) rather than a study of a human sample."
  where: []
  when: "2008"
  n: null
  sector: []
  sample_notes: >
    No study population; this is administrative/editorial front matter (aims and scope,
    editorial board roster, subscription information) bound with a 2008 journal issue.
limitation:
  primary: "This is not a research paper: it contains no methodology, data, or findings, and its subject (substance use/dependence research policy) is only tangentially related to social network health."
  others:
    - "Purely descriptive/administrative content with no empirical claims to evaluate for bias."
    - "Likely mis-filed in the SNH corpus, possibly captured incidentally alongside a substantive article from the same journal issue."
risk_of_bias: "not-applicable"
relevance_to_project: >
  This document offers no evidence for SNH design decisions; it is retained in the corpus
  only as journal masthead/scope text, and should not be cited as a source of findings on
  isolation, burnout, or social support.
tags:
  topic: ["methodology"]
  method: ["theory"]
  population: ["general"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Drug and Alcohol Dependence - Journal Scope and Editorial Board/Drug and Alcohol Dependence - Journal Scope and Editorial Board.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Drug and Alcohol Dependence - Journal Scope and Editorial Board.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "brown-2006-dynamic-wait-listed-designs-for-randomized"
title: "Dynamic wait-listed designs for randomized trials: new designs for prevention of youth suicide"
authors:
  - "Brown, C Hendricks"
  - "Wyman, Peter A"
  - "Guo, Jing"
  - "Peña, Juan"
year: 2006
doi: "10.1191/1740774506cn152oa"
venue: {type: "journal", name: "Clinical Trials", volume: 3, issue: 3, pages: "259-271"}
citation: "Brown et al. (2006). Dynamic wait-listed designs for randomized trials: new designs for prevention of youth suicide. Clinical Trials, 3(3), 259-271. https://doi.org/10.1191/1740774506cn152oa"
article_type: "methods"
method: {design: "design-report", approach: "modelling", evidence_level: "moderate", preregistered: false}
gist: >
  This paper introduces the 'dynamic wait-listed design,' a generalization of the classic
  randomized wait-listed trial in which units (e.g., schools) are assigned to intervention
  at multiple random time points rather than just two. Using Poisson power calculations, the
  authors show this design nearly always increases statistical power over a standard wait-
  listed design, with efficiency gains ranging from 33% to 100% depending on effect size and
  time-varying background rates. They illustrate the method with an ongoing school-based
  gatekeeper training (QPR) trial for youth suicide prevention in a Georgia school district.
claims:
  - text: "Dynamic wait-listed designs always yield higher statistical power than a traditional two-phase wait-listed design; efficiency gains are typically 33% and can approach 100% when the intervention effect is large or background rate variation across time is low."
    evidence: "design-report"
    support_strength: "moderate"
    outcomes: ["measurement"]
    predictors: ["intervention"]
  - text: "Converting the Georgia gatekeeper trial's second phase from a fixed wait-list to a dynamic design raises statistical power to detect a 23% increase in suicidal-youth referral rates (vs. needing a 32% increase under the standard design at 80% power), equivalent to adding six more schools to the study without added cost."
    evidence: "design-report"
    support_strength: "moderate"
    outcomes: ["help-seeking"]
    predictors: ["intervention", "network-structure"]
  - text: "Baseline surveillance data from the district showed roughly 6% of middle/high schoolers reported a suicide attempt in the past year (~3,600 of 60,000 students), yet school staff successfully identified and referred only an estimated 5% of these suicidal youth (193/3,600) prior to gatekeeper training."
    evidence: "cross-sectional"
    support_strength: "low-to-moderate"
    outcomes: ["help-seeking", "suicidal-ideation"]
    predictors: ["intervention", "sampling-method"]
population:
  who: "Middle and high school staff (~2,500 in early-intervention schools) and students (ages 11-18) in 32 schools of a large Georgia public school district, used as the applied case for a QPR gatekeeper-training suicide-prevention trial that motivated the new statistical design."
  where: ["USA (Georgia)"]
  when: "2003-2006 (trial began January 2004; baseline surveys 2003-2004 school year)"
  n: 60000
  sector: ["education", "mental-health-services"]
  sample_notes: >
    Applied example is a real, funded (NIMH) cluster-randomized wait-listed trial in 32
    schools stratified by school level and prior crisis-referral rate; staff baseline survey
    used a random 10% sample per school; student suicidality data came from an anonymous
    online survey with only a 'modest fraction' of eligible eighth/tenth graders completing
    it, limiting representativeness. The paper's main content, however, is
    statistical/mathematical derivation, not an empirical outcome study.
limitation:
  primary: "Like all wait-listed designs, the dynamic version can only evaluate short-term intervention impact, since by design every unit eventually receives the intervention and no long-term control group remains."
  others:
    - "Power gains are derived under Poisson/gamma-Poisson modeling assumptions (count or rate outcomes with time-varying but exchangeable background rates); benefits are much smaller or absent for single-measurement or non-count outcomes."
    - "The design is inappropriate when high-risk participants might withdraw before receiving a delayed intervention (e.g., trials in individuals with prior suicide attempts)."
    - "The Georgia trial application is illustrative/prospective in this paper (power projections), not a completed outcome evaluation of the QPR program's effect on suicide referrals."
risk_of_bias: "not-applicable"
relevance_to_project: >
  This paper is a statistical/design methods reference relevant to how SNH-adjacent
  prevention or intervention trials (e.g., gatekeeper training, peer-support programs,
  community-based interventions) could be evaluated more efficiently when outcomes are low-
  base-rate counts (such as help-seeking, crisis referrals, or suicidal ideation); it offers
  a concrete design pattern for staged rollout studies that also improves logistics of
  training delivery, which is analogous to phased deployment of SNH interventions across
  teams or communities.
tags:
  topic: ["suicide-prevention", "methodology", "measurement"]
  method: ["design-report", "modelling"]
  population: ["adolescents"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Dynamic Wait-Listed Designs for Randomized Trials - New Designs for Prevention of Youth Suicide/Dynamic Wait-Listed Designs for Randomized Trials - New Designs for Prevention of Youth Suicide.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Dynamic Wait-Listed Designs for Randomized Trials - New Designs for Prevention of Youth Suicide.pdf"
  notes: null

---

id: "wyman-2020-effect-of-the-wingman-connect-upstream"
title: "Effect of the Wingman-Connect Upstream Suicide Prevention Program for Air Force Personnel in Training"
authors:
  - "Wyman, Peter A."
  - "Pisani, Anthony R."
  - "Brown, C. Hendricks"
  - "Yates, Bryan"
  - "Morgan-DeVelder, Lacy"
  - "Schmeelk-Cone, Karen"
  - "Gibbons, Robert D."
  - "Caine, Eric D."
  - "Petrova, Mariya"
  - "Neal-Walden, Tracy"
  - "Linkh, David J."
  - "Matteson, Alicia"
  - "Simonson, Jordan"
  - "Pflanz, Steven E."
year: 2020
doi: "10.1001/jamanetworkopen.2020.22532"
venue: {type: "journal", name: "JAMA Network Open", volume: 3, issue: 10, pages: "e2022532"}
citation: "Wyman et al. (2020). Effect of the Wingman-Connect Upstream Suicide Prevention Program for Air Force Personnel in Training. JAMA Network Open, 3(10), e2022532. https://doi.org/10.1001/jamanetworkopen.2020.22532"
article_type: "empirical"
method: {design: "rct", approach: "experiment", evidence_level: "strong", preregistered: true}
gist: >
  This cluster randomized clinical trial tested Wingman-Connect, a group-based network
  health intervention delivered to entire Air Force training classes to build cohesion,
  shared purpose, and healthy coping, against an active stress-management comparison
  condition. Among 1485 Airmen in 215 classes, Wingman-Connect reduced suicidal ideation and
  depression symptoms and occupational problems at 1 month, with depression benefits
  sustained at 6 months, and mediation analyses showed the effect operated through increased
  class-level cohesion, morale, healthy norms, and bonds. It is offered as the first
  universal upstream suicide-prevention program shown in an RCT to reduce suicidal ideation
  and depression in a general (non-clinical) military population, providing direct empirical
  support for a network-health model in which strengthening natural group bonds protects
  individual mental health.
claims:
  - text: "At 1-month follow-up, Wingman-Connect participants showed lower suicidal ideation severity (effect size -0.23; 95% CI -0.39 to -0.09; P=.001), lower depression symptoms (ES -0.24; 95% CI -0.41 to -0.08; P=.002), and fewer occupational problems (ES -0.14/-0.13; 95% CI -0.31 to -0.02; P=.02) compared with the stress-management control group."
    evidence: "rct"
    support_strength: "strong"
    outcomes: ["suicidal-ideation", "depression", "mental-health"]
    predictors: ["intervention", "team-cohesion"]
  - text: "Depression benefits were sustained at 6 months (ES -0.16; 95% CI -0.34 to -0.02; P=.03), with 20% lower odds of elevated depression across follow-ups (OR 0.80; 95% CI 0.64-0.97) and a number needed to treat of 21; suicidal ideation was not significantly lower at 6 months (ES -0.13; P=.06) and occupational-problem benefits did not persist past 1 month."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["depression", "suicidal-ideation", "mental-health"]
    predictors: ["intervention"]
  - text: "Wingman-Connect participants gained on all four hypothesized class protective factors -- cohesion, morale, bonds to classmates, and healthy class norms (ES 0.18 to 0.23) -- and formal mediation tests showed this 'connected, healthy class' latent factor significantly mediated the program's effect on 1-month suicidal ideation (estimate -0.035; 95% CI -0.07 to -0.01; P=.02) and depression symptoms (estimate -0.039; 95% CI -0.07 to -0.01; P=.02), directly supporting the network health theoretical model. No group differences were found for loneliness or emotion dysregulation as mediators."
    evidence: "rct"
    support_strength: "strong"
    outcomes: ["mental-health", "suicidal-ideation", "depression"]
    predictors: ["team-cohesion", "sense-of-belonging", "social-support"]
population:
  who: "US Air Force enlisted personnel newly entering technical training, organized into intact training classes (squadrons at a single technical training school)"
  where: ["United States"]
  when: "October 2017 to October 2019"
  n: 1485
  sector: ["military"]
  sample_notes: >
    215 of 216 randomized classes (1485 of 1897 exposed Airmen, 85.7% enrollment)
    participated; classes paired within squadron and randomized to Wingman-Connect (748) vs
    active stress-management control (737); 84% retention at 6 months with no differential
    attrition by condition; predominantly young (mean age 20.9), male (82.3%) sample from a
    single Air Force base, limiting generalizability to other services, older personnel, or
    operational (non-training) units.
limitation:
  primary: "Participants and school leadership were not blinded to intervention condition, so awareness of assignment could have influenced self-reported outcomes despite comparable training-satisfaction ratings across arms."
  others:
    - "All primary outcomes relied on self-report (though validated against structured clinical interviews)."
    - "Training was delivered by research-team staff rather than routine military personnel, limiting generalizability to real-world scale-up."
    - "Single-site study restricted to initial technical training; effects on occupational problems and suicidal ideation did not persist to 6 months, and impact on actual suicidal behavior (vs. ideation) was not tested."
risk_of_bias: "low"
relevance_to_project: >
  Provides strong causal (RCT) evidence that a brief, universal group intervention targeting
  natural-unit cohesion, shared purpose, and healthy norms reduces depression and suicidal
  ideation, and that the effect is statistically mediated by class-level
  cohesion/bonds/morale -- directly validating the network-health mechanism (strengthening
  peer bonds as upstream prevention) that the SNH project's design work draws on for
  community and remote-team interventions. Its 4-measure protective-factor battery
  (cohesion, morale, healthy norms, named peer bonds) is a reusable model for
  operationalizing 'team/community health' as a measurable, intervenable construct.
tags:
  topic: ["suicide-prevention", "mental-health", "community-health", "psychological-safety"]
  method: ["rct", "mediation-analysis", "survey"]
  population: ["military"]
source:
  markdown: "Papers_Data/Mental Health/MD/Effect of the Wingman-Connect Upstream Suicide Prevention Program for Air Force Personnel in Training A Cluster Randomized Clinical Trial/Effect of the Wingman-Connect Upstream Suicide Prevention Program for Air Force Personnel in Training A Cluster Randomized Clinical Trial.md"
  pdf: "papers/Mental Health/Effect of the Wingman-Connect Upstream Suicide Prevention Program for Air Force Personnel in Training A Cluster Randomized Clinical Trial.pdf"
  notes: null

---

id: "kellam-2008-effects-of-a-universal-classroom-behavior"
title: "Effects of a universal classroom behavior management program in first and second grades on young adult behavioral, psychiatric, and social outcomes"
authors:
  - "Kellam, Sheppard G."
  - "Brown, C. Hendricks"
  - "Poduska, Jeanne M."
  - "Ialongo, Nicholas S."
  - "Wang, Wei"
  - "Toyinbo, Peter"
  - "Petras, Hanno"
  - "Ford, Carla"
  - "Windham, Amy"
  - "Wilcox, Holly C."
year: 2008
doi: "10.1016/j.drugalcdep.2008.01.004"
venue: {type: "journal", name: "Drug and Alcohol Dependence", volume: 95, issue: null, pages: "S5-S28"}
citation: "Kellam et al. (2008). Effects of a universal classroom behavior management program in first and second grades on young adult behavioral, psychiatric, and social outcomes. Drug and Alcohol Dependence, 95, S5-S28. https://doi.org/10.1016/j.drugalcdep.2008.01.004"
article_type: "empirical"
method: {design: "rct", approach: "experiment", evidence_level: "moderate", preregistered: false}
gist: >
  This 19-21-year-old follow-up of Baltimore's first-generation Good Behavior Game (GBG)
  trial found that a universal, teacher-delivered classroom behavior-management intervention
  played in first and second grade produced durable reductions in young-adult lifetime drug
  and alcohol abuse/dependence disorders, regular smoking, and antisocial personality
  disorder, with the largest gains concentrated among males rated highly
  aggressive/disruptive in first grade; effects on depression and generalized anxiety were
  null. A second, replication cohort taught by the same teachers but given far less ongoing
  mentoring and monitoring showed weaker, mostly non-significant effects in the same
  direction, pointing to implementation fidelity as a driver of sustained impact.
claims:
  - text: "Among Cohort 1 males, a classroom-random-effects (GLMM) model found GBG significantly reduced lifetime drug abuse/dependence disorder relative to internal controls (log OR = -0.999, S.E. = 0.450, p = .035), roughly a 2.7-times-greater risk of the disorder among controls; population-adjusted rates were 19% for GBG vs. 38% for internal controls."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["substance-abuse", "mental-health"]
    predictors: ["intervention"]
  - text: "GBG significantly reduced lifetime alcohol abuse/dependence disorders across Cohort 1 males and females combined (log OR = -0.70, S.E. = 0.35, p = .05), roughly a 50% reduction in the odds of a lifetime alcohol diagnosis, with adjusted population rates of 13% (GBG) vs. 20% (internal controls)."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["substance-abuse", "mental-health"]
    predictors: ["intervention"]
  - text: "GBG's impact on lifetime antisocial personality disorder (ASPD) varied strongly by baseline aggressive/disruptive behavior (interaction chi-square = 10.05, 3 d.f., p = .018): among males rated highly aggressive/disruptive in first grade, the adjusted ASPD rate fell from 86% in controls to 41% in the GBG group, versus an overall reduction from 25% (controls) to 17% (GBG, males and females combined)."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["mental-health"]
    predictors: ["intervention"]
population:
  who: "First- and second-grade children in 19 Baltimore City Public Schools randomized (by classroom, nested in matched schools) to the Good Behavior Game or control conditions in 1985-1986, followed up by structured telephone interview at ages 19-21"
  where: ["United States"]
  when: "Baseline cohort entered first grade in 1985-1986 (replication cohort 1986-1987); young-adult follow-up interviews conducted at ages 19-21"
  n: 922
  sector: ["education", "public-health"]
  sample_notes: >
    Analytic sample of 922 (238 GBG, 169 internal GBG controls, plus 515 additional
    ML/external controls) drawn from an original cohort of 1,196 children in five poor-to-
    lower-middle-class, mainly African American urban Baltimore areas; 75% (689/922) were
    interviewed at young-adult follow-up, with significantly lower follow-up among males
    (66%) than females (83%) and variation by urban area, though attrition was unrelated to
    intervention condition or baseline scores.
limitation:
  primary: "Randomization occurred at the classroom level with only 8 GBG and 6 internal-control classrooms nested in 6 schools, so within-school small-sample tests had low statistical power and some large-sample model results may have inflated Type I error."
  others:
    - "Design relies on two single time points 14 years apart (first-grade baseline and one young-adult interview), precluding examination of developmental trajectories or mediating mechanisms linking classroom behavior to adult outcomes."
    - "A second (replication) cohort that received substantially less teacher mentoring and monitoring showed markedly weaker, largely non-significant effects, suggesting the strong Cohort 1 results depended on high-fidelity implementation not guaranteed in typical dissemination."
    - "Sample is drawn from poor-to-lower-middle-class, predominantly African American urban Baltimore communities in the 1980s, limiting generalizability to other populations, eras, or school contexts."
risk_of_bias: "medium"
relevance_to_project: >
  Shows that a low-cost, universal classroom-level intervention built around peer-team
  social structure and behavior management can produce large, durable reductions in
  adulthood substance-abuse and antisocial-personality outcomes, especially for high-risk
  males, offering evidence for the SNH project's interest in upstream, structural (rather
  than individual-therapy) interventions that reshape peer/social context to prevent later
  isolation-linked and mental-health-adjacent outcomes; it also demonstrates that
  intervention fidelity (mentoring/monitoring of implementers) is critical to sustaining
  such community-level effects.
tags:
  topic: ["mental-health", "community-health", "suicide-prevention"]
  method: ["rct", "longitudinal"]
  population: ["children", "low-income", "urban"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Effects of a Universal Classroom Behavior Management Program on Young Adult Outcomes (3)/Effects of a Universal Classroom Behavior Management Program on Young Adult Outcomes (3).md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Effects of a Universal Classroom Behavior Management Program on Young Adult Outcomes (3).pdf"
  notes: null

---

id: "kellam-2008-effects-of-a-universal-classroom-behavior"
title: "Effects of a universal classroom behavior program in first and second grades on young adult problem outcomes"
authors:
  - "Kellam, Sheppard G."
  - "Reid, John"
  - "Balster, Robert L."
year: 2008
doi: "10.1016/j.drugalcdep.2008.01.006"
venue: {type: "journal", name: "Drug and Alcohol Dependence", volume: 95, issue: null, pages: "S1-S4"}
citation: "Kellam et al. (2008). Effects of a universal classroom behavior program in first and second grades on young adult problem outcomes. Drug and Alcohol Dependence, 95, S1-S4. https://doi.org/10.1016/j.drugalcdep.2008.01.006"
article_type: "commentary"
method: {design: "theory", approach: "other", evidence_level: "reference", preregistered: false}
gist: >
  This editorial introduces a Drug and Alcohol Dependence special issue reporting young-
  adult (age 19-21, some to 23) follow-up of the Good Behavior Game (GBG), a universal
  first- and second-grade classroom behavior-management intervention tested in randomized
  field trials with the Baltimore City Public School System. It frames the shared
  theoretical question across the five companion papers: whether an intervention targeting
  one early antecedent (aggressive, disruptive classroom behavior) can reduce risk across a
  broad profile of young adult outcomes (substance use disorders, antisocial personality
  disorder, delinquency, school failure, suicide ideation/attempts, depression/anxiety, and
  service use), and summarizes each paper plus the editorial development process.
claims:
  - text: "The five index papers test whether GBG's effect on a single shared early antecedent (aggressive, disruptive first-grade classroom behavior) reduces risk across a broad set of young-adult outcomes including drug and alcohol disorders, antisocial personality disorder, delinquency/incarceration, school failure, suicide ideation and attempts, and depressive/anxiety disorders."
    evidence: "theory"
    support_strength: "moderate"
    outcomes: ["mental-health", "suicidal-ideation", "depression"]
    predictors: ["intervention"]
  - text: "Consistent with life course/social field theory, GBG impact was hypothesized and generally found to be stronger among males and among children with higher baseline levels of aggressive, disruptive behavior, with the notable exception of suicidal ideation and attempts, where early aggression was a weaker predictor and impact patterns differed."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation", "mental-health"]
    predictors: ["intervention"]
  - text: "A second-cohort replication using the same teachers and schools but with much less continuing mentoring and monitoring of GBG fidelity showed significant effects only for drug abuse/dependence disorders and for service use related to emotional, behavioral, drug, or alcohol problems, with other outcomes trending in the predicted direction but not reaching significance."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["mental-health"]
    predictors: ["intervention", "community-engagement"]
population:
  who: "First-grade children in regular classrooms in the Baltimore City Public School System, followed longitudinally into young adulthood (ages 19-21, with some analyses extending to age 23)."
  where: ["Baltimore, MD, USA"]
  when: "First-grade intervention cohorts from an early-1980s partnership with BCPSS; young-adult follow-up outcomes reported in papers published in 2008"
  n: null
  sector: ["education", "public-health", "prevention-science"]
  sample_notes: >
    Editorial describes two cohorts: a primary effectiveness-trial cohort (41 classrooms, 19
    schools) and a second consecutive first-grade cohort taught by the same teachers but
    given much less continuing mentoring/monitoring of GBG implementation, used as a
    replication; exact total sample size is not stated in this editorial and must be pulled
    from the individual companion papers.
limitation:
  primary: "As an editorial, it synthesizes and previews companion papers rather than presenting independent data, methods, or effect sizes, so specific quantitative findings and study-level limitations must be verified against each underlying paper."
  others:
    - "The replication cohort had markedly reduced fidelity monitoring, which the editorial itself flags as complicating direct comparison between the two cohorts."
    - "The editorial notes GBG effects and early risk associations were consistently stronger for males than females across nearly all outcomes, leaving female-specific developmental pathways understudied."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Frames a multi-decade, school-based randomized prevention trial (the Baltimore GBG
  program) testing whether addressing one early, shared behavioral antecedent via a low-cost
  universal classroom intervention can shift a broad range of young-adult mental health,
  suicide-related, and substance-use outcomes, offering a model of upstream/preventive
  intervention design and long-term institutional partnership relevant to SNH's interest in
  community-level prevention strategies.
tags:
  topic: ["mental-health", "suicide-prevention", "methodology"]
  method: ["rct", "theory"]
  population: ["children", "school-based", "young-adults"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Effects of a Universal Classroom Behavior Management Program on Young Adult Outcomes (4)/Effects of a Universal Classroom Behavior Management Program on Young Adult Outcomes (4).md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Effects of a Universal Classroom Behavior Management Program on Young Adult Outcomes (4).pdf"
  notes: null

---

id: "diamanti-2009-endocrine-disrupting-chemicals-an-endocrine-society"
title: "Endocrine-Disrupting Chemicals: An Endocrine Society Scientific Statement"
authors:
  - "Diamanti-Kandarakis, Evanthia"
  - "Bourguignon, Jean-Pierre"
  - "Giudice, Linda C."
  - "Hauser, Russ"
  - "Prins, Gail S."
  - "Soto, Ana M."
  - "Zoeller, R. Thomas"
  - "Gore, Andrea C."
year: 2009
doi: "10.1210/er.2009-0002"
venue: {type: "journal", name: "Endocrine Reviews", volume: 30, issue: 4, pages: "293-342"}
citation: "Diamanti-Kandarakis et al. (2009). Endocrine-Disrupting Chemicals: An Endocrine Society Scientific Statement. Endocrine Reviews, 30(4), 293-342. https://doi.org/10.1210/er.2009-0002"
article_type: "review"
method: {design: "review-narrative", approach: "other", evidence_level: "moderate", preregistered: false}
gist: >
  This is The Endocrine Society's first Scientific Statement (2009) synthesizing animal,
  clinical, and epidemiological evidence that endocrine-disrupting chemicals (EDCs) such as
  BPA, phthalates, PCBs, and organochlorine pesticides interfere with hormone signaling and
  are linked to reproductive disorders, breast and prostate cancer, thyroid dysfunction,
  obesity/metabolic disease, cardiovascular effects, and neuroendocrine/behavioral changes.
  It argues the evidence converges across species and study types to justify treating EDCs
  as a public health concern and invoking the precautionary principle, and it closes with
  recommendations for research, clinical practice, and policy. The document is a
  toxicology/endocrinology consensus statement, not a study of social connection, work, or
  community.
claims:
  - text: "Developmental exposure to PCBs, phytoestrogens (e.g., coumestrol), and the fungicide vinclozolin altered sexual/mating behavior and neuroendocrine sexual differentiation in rodent studies, with vinclozolin-induced effects on mate preference persisting through the F3 generation via paternal germline epigenetic transmission despite F3 animals having no direct chemical exposure."
    evidence: "review-narrative"
    support_strength: "low-to-moderate"
    outcomes: ["neurodevelopment", "reproductive-behavior"]
    predictors: ["endocrine-disruptor-exposure"]
  - text: "Human and animal evidence links PCB and BPA exposure to neurodevelopmental/behavioral effects, including PCB body burden correlating with impaired response-inhibition in children with smaller corpus callosum volume, and BPA-exposed rats exhibiting ADHD-like symptoms consistent with BPA acting as a thyroid-hormone-receptor antagonist in the developing brain."
    evidence: "review-narrative"
    support_strength: "low"
    outcomes: ["mental-health", "neurodevelopment"]
    predictors: ["endocrine-disruptor-exposure"]
  - text: "The statement concludes that results from animal models, human clinical observations, and epidemiological studies (e.g., an ~90,000-participant Agricultural Health Study linking specific pesticides to elevated prostate cancer risk) converge to implicate EDCs as a significant public health concern across reproductive, thyroid, metabolic, and cardiovascular systems, warranting the precautionary principle in chemical policy."
    evidence: "review-narrative"
    support_strength: "moderate"
    outcomes: ["public-health-risk"]
    predictors: ["endocrine-disruptor-exposure"]
population:
  who: "No single study population; synthesizes rodent/wildlife experimental models and multiple human epidemiological cohorts (e.g., occupational pesticide applicators, prenatally-exposed children, DES-exposed women) drawn from the cited literature."
  where: ["United States", "Europe", "multi-country/global (wildlife and epidemiological studies)"]
  when: "Literature reviewed through 2009"
  n: null
  sector: []
  sample_notes: >
    Aggregate narrative synthesis, not a primary dataset; underlying evidence quality is
    highly heterogeneous, ranging from in vitro/animal mechanistic studies to large human
    epidemiological cohorts, with no single sample or response rate to report.
limitation:
  primary: "This is a narrative expert consensus statement, not a systematic review or meta-analysis; study selection and synthesis are not governed by a documented systematic search/inclusion protocol, so citation and emphasis may be selective."
  others:
    - "Much of the behavioral/neuroendocrine evidence comes from animal models with uncertain generalizability and unresolved low-dose, non-monotonic dose-response extrapolation to typical human mixture exposures."
    - "Long latency between developmental exposure and adult disease manifestation makes causal attribution in humans difficult across the cited epidemiological studies."
    - "The document contains no data or discussion of social network health, remote work, workplace social support, or community engagement — it is a toxicology/endocrinology statement, not a social/organizational study."
risk_of_bias: "medium"
relevance_to_project: >
  This document is fundamentally outside the SNH project's scope: it is an
  endocrinology/toxicology consensus statement about environmental chemical exposures and
  does not address social network health, remote work, isolation, belonging, or community
  engagement in any way. Its only tangential connection is that it describes neuroendocrine
  and HPA-axis stress-response pathways and brain-behavior effects (e.g., BPA/ADHD-like
  symptoms) that are sometimes cited as background biology in stress and mental-health
  research; it should not be relied on to inform any SNH design decision, measure, or claim.
tags:
  topic: ["mental-health"]
  method: ["review-narrative"]
  population: ["general-population", "animal-models"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Endocrine-Disrupting Chemicals - An Endocrine Society Scientific Statement/Endocrine-Disrupting Chemicals - An Endocrine Society Scientific Statement.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Endocrine-Disrupting Chemicals - An Endocrine Society Scientific Statement.pdf"
  notes: null

---

id: "benke-2024-environment-shapes-emotional-cognitive-abilities-more"
title: "Environment Shapes Emotional Cognitive Abilities More Than Genes"
authors:
  - "Benke, Kristopher"
year: 2024
doi: null
venue: {type: "other", name: "Neuroscience News", volume: null, issue: null, pages: null}
citation: "Benke (2024). Environment Shapes Emotional Cognitive Abilities More Than Genes. Neuroscience News."
article_type: "commentary"
method: {design: "cross-sectional", approach: "secondary-data", evidence_level: "low-to-moderate", preregistered: false}
gist: >
  This is a science-news summary (Neuroscience News, reporting on a Cell Reports study by
  Wan et al.) describing a twin study finding that metacognition and mentalizing -- the
  ability to monitor one's own thinking and to read others' mental states -- are shaped more
  by shared family environment than by genetics, in contrast to general intelligence which
  prior work puts at 50-80% heritable. The article contributes an environment-can-outweigh-
  genetics data point for social-cognitive capacities, relevant to how malleable
  empathy/mentalizing-adjacent skills may be through environmental or programmatic
  intervention rather than being fixed traits.
claims:
  - text: "General intelligence has previously been estimated as 50-80% heritable, but this twin study found metacognition and mentalizing showed a much weaker genetic signal and a stronger shared-environment signal, regardless of zygosity."
    evidence: "cross-sectional"
    support_strength: "low-to-moderate"
    outcomes: ["mental-health"]
    predictors: ["network-structure"]
  - text: "Among 57 monozygotic and 48 dizygotic adult twin pairs from the Beijing Twin Study (BeTwiSt), pairs whose parents had higher education and family income showed similarly high metacognitive performance whether the twins were identical or fraternal, pointing to a shared family-environment effect rather than a genetic one."
    evidence: "cross-sectional"
    support_strength: "low-to-moderate"
    outcomes: ["mental-health"]
    predictors: ["network-structure", "social-support"]
  - text: "Human cognitive abilities separate into two hierarchical orders: first-order abilities (perception, attention, memory, language, planning) were primarily genetically influenced, while second-order abilities (metacognition and mentalizing) were more influenced by shared environmental/family factors such as parental nurturing and cultural transmission."
    evidence: "cross-sectional"
    support_strength: "low-to-moderate"
    outcomes: ["mental-health"]
    predictors: ["network-structure"]
population:
  who: "105 adult twin pairs (57 monozygotic, 48 dizygotic) drawn from the ongoing Beijing Twin Study (BeTwiSt) cohort, performing perceptual-decision and confidence/mentalizing tasks"
  where: ["China"]
  when: "News article published April 18, 2024, reporting a study published April 2, 2024 in Cell Reports; BeTwiSt cohort established 2006"
  n: 105
  sector: []
  sample_notes: >
    Sample size and recruitment described only at the level of a news summary; no detail on
    response rate, exclusion criteria, or representativeness of the BeTwiSt cohort relative
    to the general population is given in this document.
limitation:
  primary: "This document is a secondary press-style summary of a single twin study, not the primary literature or an independent methodological review, so effect sizes, confidence intervals, and model specification for the heritability/shared-environment estimates are not reported here."
  others:
    - "Findings come from one cohort in Beijing, China and may not generalize to other populations or cultural contexts."
    - "The underlying study's own authors caution the findings were unexpected relative to decades of twin research and call for further replication and population studies."
risk_of_bias: "medium"
relevance_to_project: >
  Speaks to how malleable social-cognitive capacities like mentalizing (reading others'
  emotional/mental states) may be by shared environment rather than fixed by genetics, which
  is suggestive background for the SNH project's assumption that
  community/family/organizational environment can shift capacities underlying empathy and
  social connection -- though the evidence is indirect, drawn from a general-population twin
  study rather than remote-work or community-health contexts.
tags:
  topic: ["mental-health", "measurement"]
  method: ["cross-sectional", "secondary-data"]
  population: ["general-population", "adults"]
source:
  markdown: "Papers_Data/Mental Health/MD/Environment Shapes Emotional Cognitive Abilities More Than Genes/Environment Shapes Emotional Cognitive Abilities More Than Genes.md"
  pdf: "papers/Mental Health/Environment Shapes Emotional Cognitive Abilities More Than Genes.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "cicchetti-1996-equifinality-and-multifinality-in-developmental-psychopathology"
title: "Equifinality and multifinality in developmental psychopathology"
authors:
  - "Cicchetti, Dante"
  - "Rogosch, Fred A."
year: 1996
doi: "10.1017/s0954579400007318"
venue: {type: "journal", name: "Development and Psychopathology", volume: 8, issue: 4, pages: "597-600"}
citation: "Cicchetti et al. (1996). Equifinality and multifinality in developmental psychopathology. Development and Psychopathology, 8(4), 597-600. https://doi.org/10.1017/s0954579400007318"
article_type: "theory"
method: {design: "theory", approach: "analytical", evidence_level: "speculative", preregistered: false}
gist: >
  This is the editorial introduction to a special issue of Development and Psychopathology,
  in which Cicchetti and Rogosch define and argue for the centrality of two organizing
  principles: equifinality (diverse initial conditions and pathways can converge on the same
  developmental outcome) and multifinality (the same risk factor or component can lead to
  divergent outcomes depending on the organizational context in which it operates). The
  editors use these concepts to argue that variable-oriented, group-level research must be
  complemented by person-oriented, pathways-based, subgroup analyses to capture individual
  heterogeneity in adaptive and maladaptive development. It sets the conceptual agenda for
  the papers that follow in the issue rather than reporting original data.
claims:
  - text: "Equifinality: in an open developmental system, a diversity of pathways, chance events, and nonlinear epigenetic processes can lead to the same outcome, so a single adverse event does not necessarily produce the same psychopathological (or non-psychopathological) result in every individual."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["mental-health"]
    predictors: ["network-structure"]
  - text: "Multifinality: the effect of any one component (e.g., a risk factor or life event) on functioning varies depending on the organization of the system and the other components to which it is structurally linked, so individuals who begin on the same major developmental pathway can exhibit very different patterns of adaptation or maladaptation over time."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["mental-health"]
    predictors: ["network-structure"]
  - text: "The editors argue that group-level, variable-oriented analysis (useful for identifying average/most-expected outcomes) must be supplemented by person-oriented, homogeneous-subgroup analysis of longitudinal data to reveal the diverse individual pathways and processes underlying common outcomes, which they position as a necessary next step for the field."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["mental-health"]
    predictors: ["network-structure"]
population:
  who: "Not an empirical study of a specific sample; this is a conceptual editorial framing a special issue of Development and Psychopathology, referencing findings and populations (infancy through old age, conduct disorder, depression, substance use, schizophrenia, twin studies) covered by the issue's other papers."
  where: []
  when: null
  n: null
  sector: []
  sample_notes: >
    No original sample; the piece is a short (editorial-length, ~2-3 page) framing essay
    with no methods section of its own.
limitation:
  primary: "As an editorial introducing a special issue, it presents no original empirical data, systematic search, or analytic methodology of its own — it is a conceptual argument citing prior theoretical work and forward-referencing unspecified papers in the same issue."
  others:
    - "The markdown conversion is degraded (garbled column-merge artifacts and a mangled reference list), making some sentences and citations hard to verify against the original text."
    - "Concepts are asserted rather than tested; no criteria are given for when equifinality versus multifinality applies to a given outcome."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Equifinality and multifinality give the SNH project a principled reason to expect no
  single dominant pathway from a risk factor (e.g., isolation, workload) to an outcome
  (e.g., burnout, disengagement) and no single intervention likely to work for everyone;
  they motivate person-oriented, subgroup-based analysis of remote-worker and open-source
  contributor data rather than relying solely on average-effect (variable-oriented) models
  when designing or evaluating interventions.
tags:
  topic: ["mental-health", "methodology"]
  method: ["theory"]
  population: ["clinical-population"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Equifinality and Multifinality in Developmental Psychopathology/Equifinality and Multifinality in Developmental Psychopathology.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Equifinality and Multifinality in Developmental Psychopathology.pdf"
  notes: null

---

id: "ponte-2022-how-to-be-a-mental-health"
title: "How to Be a Mental Health Ally"
authors:
  - "Ponte, Katherine"
year: 2022
doi: null
venue: {type: "other", name: "Harvard Business Review", volume: null, issue: null, pages: null}
citation: "Ponte (2022). How to Be a Mental Health Ally. Harvard Business Review."
article_type: "commentary"
method: {design: "narrative-commentary", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  A Harvard Business Review practitioner article by Katherine Ponte laying out concrete
  tactics for being a workplace "mental health ally": how to open and sustain one-on-one
  conversations with a struggling colleague, scripted examples of supportive versus
  stigmatizing language, education formats (personal-account events vs. workshops), employee
  resource groups and peer group activities, and organizational policy levers (mental health
  director role, ADA-style accommodations, confidential leave, access-to-care benefits). It
  is grounded in the author's professional and lived experience rather than a formal study.
claims:
  - text: "Effective one-on-one allyship requires preparing to set aside implicit bias, timing conversations to a colleague's mood, starting gently and indirectly (e.g., asking about stressors rather than diagnoses), choosing a private or low-pressure channel (text/call before face-to-face), and assuring confidentiality before and during the conversation."
    evidence: "Author's practitioner guidance and lived-experience advice; no cited study or data."
    support_strength: "weak"
    outcomes: ["wellbeing", "help-seeking", "sense-of-belonging"]
    predictors: ["social-support"]
  - text: "Using person-first, non-judgmental, and non-platitude language (contrasted with paired 'don't say / say' examples) reduces stigma and self-stigma, while employee resource groups and shared non-mental-health-focused group activities counter loneliness and isolation for employees living with mental illness."
    evidence: "Author's practitioner recommendations illustrated with sample dialogue and program examples; not empirically tested in the article."
    support_strength: "weak"
    outcomes: ["isolation", "sense-of-belonging", "job-engagement"]
    predictors: ["peer-mentoring", "inclusiveness"]
  - text: "Organizational policy levers -- a designated mental health director, transparent benefit communication, ADA-style accommodations (flextime, remote or part-time work, quiet spaces), and confidential leave and care-access benefits -- support disclosure and help-seeking, but the article notes employees often perceive disclosure risks as outweighing benefits."
    evidence: "Author's policy recommendations referencing ADA accommodation categories and APA guidance on mental health apps; no primary data presented."
    support_strength: "weak"
    outcomes: ["help-seeking", "retention"]
    predictors: ["organizational-culture", "leadership-style"]
population:
  who: "General workplace colleagues, managers, and leaders addressed as potential 'mental health allies' to coworkers experiencing mental health challenges"
  where: []
  when: null
  n: null
  sector: []
  sample_notes: >
    Not an empirical study; no sample, participants, or data collection. Advice synthesized
    from the author's professional (NAMI-NYC board, Yale lecturer) and personal (living with
    bipolar I disorder) experience, adapted from the HBR Guide to Better Mental Health at
    Work.
limitation:
  primary: "Practitioner opinion piece with no cited primary research, data, or systematic evidence base; recommendations are asserted rather than tested."
  others:
    - "Single author with personal and organizational stake in the topic (ForLikeMinds founder, NAMI-NYC board member), creating potential advocacy bias."
    - "No discussion of contexts (industries, cultures, team structures) where the suggested tactics might fail or backfire."
risk_of_bias: "high"
relevance_to_project: >
  Directly actionable for the project's proposed peer check-in protocol: the article's
  scripted guidance on when/how to initiate one-on-one conversations, gentle regular check-
  ins, person-first and non-judgmental supportive language, and group/ERG engagement maps
  closely onto the protocol's core mechanics, and its policy section (accommodations,
  confidential leave, mental health director role) offers organizational-support language
  the project can reuse or cite.
tags:
  topic: ["mental-health", "social-support", "wellbeing", "psychological-safety", "community-health"]
  method: ["narrative-commentary"]
  population: ["knowledge-workers", "managers", "general-workforce"]
source:
  markdown: "Papers_Data/Mental Health/MD/How to Be a Mental Health Ally - HBR 2022/How to Be a Mental Health Ally - HBR 2022.md"
  pdf: null
  notes: "no-doi: HBR article"

---

id: "wyman-2023-impact-of-sources-of-strength-on"
title: "Impact of Sources of Strength on adolescent suicide deaths across three randomized trials"
authors:
  - "Wyman, Peter"
  - "Cero, Ian"
  - "Brown, Charles Hendricks"
  - "Espelage, Dorothy"
  - "Pisani, Anthony"
  - "Kuehl, Tomei"
  - "Schmeelk-Cone, Karen"
year: 2023
doi: "10.1136/ip-2023-044944"
venue: {type: "journal", name: "Injury Prevention", volume: 29, issue: 5, pages: "442-445"}
citation: "Wyman et al. (2023). Impact of Sources of Strength on adolescent suicide deaths across three randomized trials. Injury Prevention, 29(5), 442-445. https://doi.org/10.1136/ip-2023-044944"
article_type: "empirical"
method: {design: "rct", approach: "experiment", evidence_level: "moderate", preregistered: false}
gist: >
  This paper pools three cluster-randomized trials (78 high schools, ~40,748 student-years
  of exposure) of Sources of Strength, a peer-leader, social-network-informed suicide
  prevention program, to test its effect on actual student suicide deaths. No suicides
  occurred in intervention schools versus four in control schools (rate of 0 vs. 20.86 per
  100,000), but statistical significance depended on the test used: a state-level exact test
  across all 78 schools found fewer suicides in intervention schools (p=0.047), while a
  stricter test restricted to the 72 randomly paired schools found no significant difference
  (p=0.150). The authors argue the mixed result reflects the low statistical power inherent
  to mortality outcomes in RCTs and call for adaptive, state-wide roll-out trial designs to
  confirm the signal.
claims:
  - text: "Across three pooled cluster RCTs (78 schools, 40,748 student-years), zero suicides occurred in Sources of Strength intervention schools versus four in control schools, an aggregated suicide rate of 0 vs. 20.86 per 100,000 person-years."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation"]
    predictors: ["intervention", "peer-mentoring", "network-structure"]
  - text: "A state-level exact test pooling all 78 schools found significantly fewer suicides in intervention vs. control schools (p=0.047), but a stricter test limited to the 72 schools randomized in matched pairs found no significant difference (p=0.150), indicating results were sensitive to statistical model choice."
    evidence: "rct"
    support_strength: "low-to-moderate"
    outcomes: ["suicidal-ideation"]
    predictors: ["intervention", "sampling-method"]
  - text: "Across the underlying trials, Sources of Strength's benefits depended on implementation fidelity: one trial showed short-term increases in student help-seeking and adult support that were lost as fidelity declined, and the program became potentially iatrogenic for ninth-graders in low-fidelity schools, whereas a later trial with expanded adult mentor training showed more consistent reductions in suicidal behaviors."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["help-seeking", "suicidal-ideation"]
    predictors: ["intervention", "peer-mentoring", "social-support"]
population:
  who: "High school students across 78 schools in three pooled cluster-randomized trials of the Sources of Strength suicide prevention program"
  where: ["USA"]
  when: "2007-2019 (Georgia, North Dakota, New York, and Colorado trial cohorts)"
  n: 39960
  sector: ["education"]
  sample_notes: >
    Pooled analysis of three separately conducted cluster RCTs (school-level randomization,
    matched pairs with 6 schools unpaired due to logistics); trials varied in duration (one
    semester vs. two school years) and in state/region, which the authors note complicates
    direct synthesis; total student rosters across trials = 39,960.
limitation:
  primary: "Suicide mortality is a rare outcome, giving the exact tests low statistical power, and results were inconsistent across the two statistical models used (significant in the more inclusive state-level test, non-significant in the stricter matched-pairs test)."
  others:
    - "Trials differed in active study duration (one school semester vs. two school years), and no adjustment was made for this variability because trial 1 had zero deaths."
    - "Only three trials were available, making it difficult to disentangle effects of trial length or other between-trial differences from the intervention effect."
    - "Low implementation fidelity in one trial was associated with potentially adverse (iatrogenic) effects on suicidal behavior in younger students, raising concern that mortality effects could also be fidelity-dependent."
risk_of_bias: "low"
relevance_to_project: >
  Provides RCT-level evidence that a scalable, peer-led social-network intervention
  (training key opinion leaders to spread help-seeking norms through friendship networks)
  can plausibly reduce the most severe outcome (suicide mortality), directly informing SNH's
  interest in network-structure-based interventions and upstream suicide-prevention design;
  the fidelity-dependence finding is a caution for any SNH intervention relying on peer
  leaders or champions.
tags:
  topic: ["suicide-prevention", "community-health", "social-support"]
  method: ["rct", "cluster-randomized", "meta-analytic-pooling"]
  population: ["adolescents", "school-based"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Impact of Sources of Strength on Adolescent Suicide Deaths Across Three Randomized Trials/Impact of Sources of Strength on Adolescent Suicide Deaths Across Three Randomized Trials.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Impact of Sources of Strength on Adolescent Suicide Deaths Across Three Randomized Trials.pdf"
  notes: null

---

id: "poduska-2008-impact-of-the-good-behavior-game"
title: "Impact of the Good Behavior Game, a universal classroom-based behavior intervention, on young adult service use for problems with emotions, behavior, or drugs or alcohol"
authors:
  - "Poduska, Jeanne M."
  - "Kellam, Sheppard G."
  - "Wang, Wei"
  - "Brown, C. Hendricks"
  - "Ialongo, Nicholas S."
  - "Toyinbo, Peter"
year: 2008
doi: "10.1016/j.drugalcdep.2007.10.009"
venue: {type: "journal", name: "Drug and Alcohol Dependence", volume: 95, issue: null, pages: "S29-S44"}
citation: "Poduska et al. (2008). Impact of the Good Behavior Game, a universal classroom-based behavior intervention, on young adult service use for problems with emotions, behavior, or drugs or alcohol. Drug and Alcohol Dependence, 95, S29-S44. https://doi.org/10.1016/j.drugalcdep.2007.10.009"
article_type: "empirical"
method: {design: "rct", approach: "experiment", evidence_level: "moderate", preregistered: false}
gist: >
  This paper follows two cohorts of Baltimore City first-graders randomized (by classroom,
  within matched schools) to the Good Behavior Game (GBG), an alternative classroom
  intervention, or control, and tracks their self-reported use of services for behavioral,
  emotional, or substance problems into young adulthood (ages 19-21). It finds that a low-
  cost, universal first/second-grade classroom management intervention targeting aggressive-
  disruptive behavior reduced later school-based mental health service use for males who
  entered first grade at highest behavioral risk, but produced no such benefit for females,
  illustrating both the promise and the limits of upstream, environment-level prevention for
  later help-seeking and service utilization.
claims:
  - text: "Highly aggressive-disruptive males in GBG classrooms had substantially lower rates of ever receiving school-based services by young adulthood than their internal-control counterparts in both cohorts (Cohort 1: 17% vs. 33%; Cohort 2: 18% vs. 33%), with the GBG-by-baseline-risk interaction significant in Cohort 1 (p=0.001) and Cohort 2 (p=0.001)."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["mental-health", "help-seeking"]
    predictors: ["intervention"]
  - text: "GBG showed no significant impact on any category of service use for females in either cohort (e.g., any service use p=0.84-0.95), even though the intervention effect for males reached or approached significance across several sectors, indicating a strongly gender-specific effect."
    evidence: "rct"
    support_strength: "low-to-moderate"
    outcomes: ["mental-health", "help-seeking"]
    predictors: ["intervention"]
  - text: "In Cohort 2, males in GBG classrooms used mental or medical health provider services at a much lower rate than internal-control males (9.4% vs. 26%, p=0.01 in the Mantel-Haenszel test), though this specific effect was not replicated in Cohort 1, where rates were nearly identical between conditions."
    evidence: "rct"
    support_strength: "low-to-moderate"
    outcomes: ["mental-health", "help-seeking"]
    predictors: ["intervention"]
population:
  who: "First- and second-grade students in the Baltimore City Public School System, followed via telephone interview into young adulthood (ages 19-21)"
  where: ["United States"]
  when: "Baseline 1985-1987 school years; young-adult follow-up when cohorts reached ages 19-21"
  n: 2311
  sector: ["education", "public-health"]
  sample_notes: >
    Two cohorts (baseline N=1196 and N=1115); 75% (n=689) and 76% (n=656) completed the
    young-adult interview respectively. Baseline covariate balance across conditions was
    generally good, though attrition differed significantly by gender (women more likely to
    complete follow-up: 83%/81% vs. 66%/70% for men), and a few baseline differences (e.g.,
    depressive symptoms, shy behavior) existed for isolated cohort-condition comparisons.
limitation:
  primary: "The GBG intervention was experimentally randomized but subsequent service use was observed naturalistically (not manipulated), so the study cannot test the effectiveness of an integrated service system, only the downstream association between an early universal intervention and later service use."
  others:
    - "Outcome relies on retrospective self-report of lifetime service use via a single young-adult telephone interview, with likely under-reporting especially for services received earlier in life."
    - "Several primary tests (e.g., combined-gender any-service-use effect, some Mantel-Haenszel tests accounting for school blocking) did not reach conventional significance even where subgroup (high-risk males) effects were significant, and multiple service-sector comparisons were run without correction for multiplicity."
    - "Training and support for the intervention differed between the two cohorts and between first- and second-grade teachers, complicating interpretation of cross-cohort consistency."
risk_of_bias: "medium"
relevance_to_project: >
  Demonstrates that a low-cost, universal, environment-level intervention delivered early
  (first/second grade) can measurably reduce later use of mental-health/behavioral services
  for a high-risk subgroup, offering an evidentiary template for the SNH project's interest
  in upstream, structural interventions (e.g., community/team-level norms or onboarding
  practices) rather than individual-targeted fixes, while also cautioning that such
  interventions can have null or reversed effects for some subgroups (here, women) and
  require sustained implementation support to hold up over time.
tags:
  topic: ["mental-health", "suicide-prevention", "community-health"]
  method: ["rct", "longitudinal"]
  population: ["youth", "school-based"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Impact of the Good Behavior Game on Young Adult Service Use for Mental Health and Substance Problems/Impact of the Good Behavior Game on Young Adult Service Use for Mental Health and Substance Problems.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Impact of the Good Behavior Game on Young Adult Service Use for Mental Health and Substance Problems.pdf"
  notes: null

---

id: "anon-nd-consent-form"
title: "Consent form"
authors:
year: null
doi: "10.51200/bjms.v12i2.946.g801"
venue: {type: "other", name: null, volume: null, issue: null, pages: null}
citation: "Unknown (None). Consent form.. https://doi.org/10.51200/bjms.v12i2.946.g801"
article_type: "methods"
method: {design: "rct", approach: "experiment", evidence_level: "speculative", preregistered: true}
gist: >
  This is the IRB consent form (not a results paper) for a cluster-randomized trial
  (NCT05967364, PI Peter Wyman, University of Rochester) comparing two career-enhancement
  trainings delivered to Air Force Airmen entering Technical Training: a
  relationship/resilience-focused 'Wingman-Guardian Connect' program versus a briefer
  stress-management program. It describes the study's design, procedures, and risks but
  reports no outcomes, since consent forms are administered before data collection begins.
claims:
  - text: "The trial cluster-randomizes entire training classes (5-11 classes, ~30-80 Airmen per session) to one of two arms: Wingman-Guardian Connect (~6 hours over three days, teaching healthy-relationship and emotional-balance skills) or Stress Management (2 hours in one day, teaching stress-response knowledge and reduction techniques), with survey outcomes collected at baseline, 6 months, and 12 months from a planned total of approximately 2,970 subjects."
    evidence: "rct"
    support_strength: "speculative"
    outcomes: ["stress", "mental-health", "wellbeing"]
    predictors: ["intervention", "social-support"]
  - text: "Planned outcome measures include self-reported healthy career practices (e.g., having mentors), supportive relationships, ability to manage military-occupational stressors, and depression, suicide risk, and hopelessness, plus administratively obtained training-class graduation status (graduated, retrained, or separated) collected 2-4 weeks after course completion."
    evidence: "rct"
    support_strength: "speculative"
    outcomes: ["depression", "suicidal-ideation", "retention"]
    predictors: ["social-support", "intervention"]
  - text: "Both arms include a low-intensity maintenance component of approximately one text message per week reinforcing training content (short videos, polls) sent over the follow-up period, alongside an optional strength-based video public-service campaign for the Wingman-Guardian Connect arm."
    evidence: "rct"
    support_strength: "speculative"
    outcomes: ["job-engagement"]
    predictors: ["intervention", "peer-mentoring"]
population:
  who: "Airmen in Technical Training at Sheppard Air Force Base, in career fields supporting the Global Strike and Air Mobility Major Commands"
  where: ["USA"]
  when: null
  n: 2970
  sector: ["military"]
  sample_notes: >
    This is a consent form, not an enrollment or results report; n=2,970 is the
    planned/target sample size, not an achieved sample. Randomization is at the training-
    class (cluster) level, not the individual level; response rates and actual accrual are
    not reported in this document.
limitation:
  primary: "This document is a study consent form describing planned design and procedures only; it contains no enrollment, retention, or outcome data and cannot be used as evidence of the interventions' effects."
  others:
    - "The principal investigator discloses a financial interest in the Connect Program underlying the Wingman-Guardian Connect arm, which has been licensed to a commercial entity, a potential conflict of interest for that arm's evaluation."
    - "Outcome measures rely on self-report survey data collected in an off-duty context, with no description in this document of blinding, attrition handling, or analysis plan."
risk_of_bias: "unclear"
relevance_to_project: >
  Describes a cluster-RCT protocol directly testing whether a relationship/resilience-skills
  training (versus stress-management training) reduces stress, depression, hopelessness, and
  suicide risk in a young, career-transitioning population, which is directly analogous to
  SNH's interest in workplace social-support interventions and their effects on wellbeing
  and retention; the eventual trial results (not yet available) would be a strong
  intervention-evidence source for the corpus.
tags:
  topic: ["mental-health", "suicide-prevention", "wellbeing", "social-support"]
  method: ["rct", "survey"]
  population: ["military", "early-career"]
source:
  markdown: "Papers_Data/Mental Health/MD/Informed Consent Form Career Enhancement Training Study Delivered Across Career Phases/Informed Consent Form Career Enhancement Training Study Delivered Across Career Phases.md"
  pdf: "papers/Mental Health/Informed Consent Form Career Enhancement Training Study Delivered Across Career Phases.pdf"
  notes: null

---

id: "kraut-1998-internet-paradox-a-social-technology-that"
title: "Internet paradox: A social technology that reduces social involvement and psychological well-being?"
authors:
  - "Kraut, Robert"
  - "Patterson, Michael"
  - "Lundmark, Vicki"
  - "Kiesler, Sara"
  - "Mukophadhyay, Tridas"
  - "Scherlis, William"
year: 1998
doi: "10.1037/0003-066x.53.9.1017"
venue: {type: "journal", name: "American Psychologist", volume: 53, issue: 9, pages: "1017-1031"}
citation: "Kraut et al. (1998). Internet paradox: A social technology that reduces social involvement and psychological well-being?. American Psychologist, 53(9), 1017-1031. https://doi.org/10.1037/0003-066x.53.9.1017"
article_type: "empirical"
method: {design: "longitudinal", approach: "survey", evidence_level: "moderate", preregistered: false}
gist: >
  This landmark HomeNet field trial tracked 169 first-time home Internet users in Pittsburgh
  over their first 1-2 years online and found that, despite the Internet being used mainly
  for interpersonal communication, greater use predicted subsequent declines in family
  communication and local social-network size and increases in loneliness and depression.
  The authors argue the panel design (controlling for baseline levels) supports a causal
  interpretation in which Internet use displaces stronger, geographically-proximate ties
  with weaker, more diffuse online ones, rather than well-being problems driving Internet
  use.
claims:
  - text: "Controlling for baseline levels and demographics, greater Internet use over 12-24 months was associated with subsequent declines in time spent communicating with household family members (beta = -.08, p < .05) and in the size of participants' local social circle (beta = -.14, p < .05), with a marginal decline in the size of the distant social circle (p < .07)."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["communication", "isolation"]
    predictors: ["internet-use"]
  - text: "Greater Internet use predicted increases in loneliness (beta = .15, p < .05) and depression (beta = .19, p < .05) at follow-up, holding constant baseline loneliness/depression and demographic controls; effects on daily stress were only marginally significant (p = .08) and effects on social support were nonsignificant (p > .40)."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["loneliness", "depression", "stress"]
    predictors: ["internet-use"]
  - text: "Baseline social involvement and psychological well-being generally did not predict subsequent Internet use (the only exception being a marginal effect that people with larger local social circles later used the Internet less), which the authors interpret as evidence that the direction of causation runs from Internet use to declines in social involvement and well-being rather than the reverse."
    evidence: "longitudinal"
    support_strength: "low-to-moderate"
    outcomes: ["loneliness", "depression"]
    predictors: ["internet-use"]
population:
  who: "169 individuals (teens and adults) from 73 Pittsburgh-area households who completed both pretest and follow-up surveys in the Carnegie Mellon HomeNet field trial of first-time home computer/Internet adopters; recruited via preexisting community ties (high school journalism classes in 1995, community-development-organization board members in 1996)."
  where: ["United States (Pittsburgh, Pennsylvania)"]
  when: "1995-1997 (pretest at Internet installation, follow-up 12-24 months later)"
  n: 169
  sector: []
  sample_notes: >
    169 of 256 original consenting participants (66%) completed both waves; completers were
    wealthier, more likely to be adults, and less lonely at baseline than non-completers.
    Households with prior Internet access were excluded, and families were drawn from
    preexisting community groups rather than sampled randomly, limiting representativeness.
limitation:
  primary: "The sample was small, not randomly selected, and drawn from families already embedded in preexisting community organizations, so findings may not generalize to isolated populations, other regions, or later eras of the Internet."
  others:
    - "34% attrition between pretest and follow-up, with completers differing systematically from dropouts on income, age, and baseline loneliness"
    - "Data were collected in 1995-1997, before broadband, social media, smartphones, or mobile messaging existed, limiting applicability to today's always-on Internet use"
    - "Effects on social support, distant social circle, and stress did not reach conventional significance, and the causal mechanism (time displacement vs. displacement of strong ties by weak ties) was not directly tested"
risk_of_bias: "medium"
relevance_to_project: >
  As the origin of the 'Internet paradox' finding, this paper is a core evidentiary anchor
  for the SNH project's concern that mediated/online interaction can causally erode face-to-
  face social involvement and worsen loneliness and depression -- specifically via
  displacement of strong ties by weaker, topic-organized online ties -- which motivates
  designing remote-work and community tools that deliberately support existing strong
  relationships rather than only enabling broad weak-tie contact.
tags:
  topic: ["isolation", "loneliness", "mental-health", "wellbeing", "social-support"]
  method: ["longitudinal", "survey"]
  population: ["households", "teenagers", "adults", "general-population"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Internet Paradox A Social Technology That Reduces Social Involvement and Psychological Well-Being/Internet Paradox A Social Technology That Reduces Social Involvement and Psychological Well-Being.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Internet Paradox A Social Technology That Reduces Social Involvement and Psychological Well-Being.pdf"
  notes: null

---

id: "sharma-2023-let-s-talk-about-code-switching"
title: "Let's Talk About Code-Switching: A Double-Edged Sword"
authors:
  - "Sharma, Nirupika"
year: 2023
doi: null
venue: {type: "other", name: "UC Berkeley Graduate Division", volume: null, issue: null, pages: null}
citation: "Sharma (2023). Let's Talk About Code-Switching: A Double-Edged Sword. UC Berkeley Graduate Division."
article_type: "commentary"
method: {design: "theory", approach: "other", evidence_level: "weak", preregistered: false}
gist: >
  This UC Berkeley graduate-division blog post argues that code-switching -- adjusting
  speech, behavior, and self-presentation to fit the norms of academic or professional
  environments -- is a double-edged coping strategy: it can secure credibility, professional
  opportunities, and social belonging, but sustained code-switching produces identity
  confusion, hypervigilance, cognitive fatigue, and burnout. It summarizes existing
  psychology findings (resume whitening, perceptions of professionalism, 'acting white'
  accusations) and recommends institutional fixes (diverse representation, mentorship, peer
  support) and individual coping resources for graduate students.
claims:
  - text: "Job applications that downplay or conceal a racial minority identity ('resume whitening') are more likely to receive interview invitations from recruiters, per Kang et al. (2016), cited as supporting evidence in this piece."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["sense-of-belonging"]
    predictors: ["inclusiveness"]
  - text: "Employees who code-switch are perceived by others as more professional than those who do not code-switch, per McCluney et al. (2021) as cited in this article."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["job-satisfaction", "sense-of-belonging"]
    predictors: ["organizational-culture", "inclusiveness"]
  - text: "The sustained effort of code-switching -- remaining hypervigilant to monitor and adjust self-presentation across contexts -- is described as exacting a mental toll that can lead to cognitive fatigue, burnout, and identity confusion."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["burnout", "mental-health", "sense-of-belonging"]
    predictors: ["technostress", "psychological-safety"]
population:
  who: "Not an empirical study; the piece addresses graduate students and, secondarily, professional-workplace employees who code-switch across racial, ethnic, gender, sexuality, age, socioeconomic, or disability identities."
  where: ["United States"]
  when: null
  n: null
  sector: ["higher-education"]
  sample_notes: >
    No primary data collection; this is an opinion/advice blog post that synthesizes
    secondary psychology research and offers institutional and individual recommendations,
    written by a doctoral candidate for UC Berkeley's Graduate Division.
limitation:
  primary: "The piece is an advocacy/advice blog post with no original data collection or systematic literature review; cited studies (Kang et al. 2016, McCluney et al. 2021, Durkee & Williams 2015) are referenced only in passing without methodological detail."
  others:
    - "Author's own dissertation research on code-switching is mentioned but not presented or cited with findings."
    - "Recommendations (mentorship, peer support, DEI initiatives) are asserted as beneficial without supporting evaluation evidence."
risk_of_bias: "high"
relevance_to_project: >
  Frames identity-related code-switching as a burnout and belonging mechanism relevant to
  inclusiveness and psychological-safety design choices in remote/hybrid and academic
  communities, and is useful as a pointer to primary literature (Kang et al. 2016; McCluney
  et al. 2021; Durkee & Williams 2015) on identity concealment, perceived professionalism,
  and social sanction, though it should not itself be cited as empirical evidence.
tags:
  topic: ["mental-health", "burnout", "psychological-safety", "wellbeing"]
  method: ["theory"]
  population: ["graduate-students", "higher-education"]
source:
  markdown: "Papers_Data/Mental Health/MD/Lets Talk About Code-Switching A Double-Edged Sword/Lets Talk About Code-Switching A Double-Edged Sword.md"
  pdf: "papers/Mental Health/Lets Talk About Code-Switching A Double-Edged Sword.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "brown-2008-methods-for-testing-theory-and-evaluating"
title: "Methods for testing theory and evaluating impact in randomized field trials: Intent-to-treat analyses for integrating the perspectives of person, place, and time"
authors:
  - "Brown, C. Hendricks"
  - "Wang, Wei"
  - "Kellam, Sheppard G."
  - "Muthén, Bengt O."
  - "Petras, Hanno"
  - "Toyinbo, Peter"
  - "Poduska, Jeanne"
  - "Ialongo, Nicholas"
  - "Wyman, Peter A."
  - "Chamberlain, Patricia"
  - "Sloboda, Zili"
  - "MacKinnon, David P."
  - "Windham, Amy"
year: 2008
doi: "10.1016/j.drugalcdep.2007.11.013"
venue: {type: "journal", name: "Drug and Alcohol Dependence", volume: 95, issue: null, pages: "S74-S104"}
citation: "Brown et al. (2008). Methods for testing theory and evaluating impact in randomized field trials: Intent-to-treat analyses for integrating the perspectives of person, place, and time. Drug and Alcohol Dependence, 95, S74-S104. https://doi.org/10.1016/j.drugalcdep.2007.11.013"
article_type: "methods"
method: {design: "case-study", approach: "analytical", evidence_level: "reference", preregistered: false}
gist: >
  This methodology paper by the Prevention Science and Methodology Group establishes
  standards for intent-to-treat (ITT) analysis in multilevel, group-randomized field trials
  (RFTs), extending pharmaceutical-trial ITT conventions to designs where randomization
  occurs at classroom, school, district, or county level. Drawing on six real RFTs
  (including the Baltimore Prevention Program's Good Behavior Game and the Georgia
  Gatekeeper suicide-prevention training trial), the authors specify rules for defining the
  analytic denominator, classifying mobile/late-entering subjects, and handling missing
  longitudinal data (FIML, multiple imputation), then present growth mixture models (GMM)
  and generalized additive mixed models (GAMM) for detecting who benefits from an
  intervention, for how long, and under what contextual conditions. It contributes a
  reusable analytic and reporting framework rather than a single substantive finding about
  social connection.
claims:
  - text: "Two defensible but distinct ITT denominator rules are needed for group-randomized trials: (1) restrict to subjects present at the start of the intervention period, which protects against late entrants being informatively assigned to condition but limits sample size, versus (2) include all subjects who enter throughout the intervention period, which maximizes sample and generalizability but risks bias if late entrants are non-randomly steered into conditions (e.g., principals disproportionately placed late-entering aggressive children into Good Behavior Game classrooms in the First Generation Baltimore Prevention Program trial)."
    evidence: "case-study"
    support_strength: "moderate"
    outcomes: []
    predictors: ["sampling-method"]
  - text: "In the Georgia Gatekeeper suicide-prevention training trial, ITT impact analyses of school staff outcomes (knowledge, attitudes, referral behavior) showed somewhat smaller training effects than parallel 'as-treated' analyses that used staff's actual (not intended) training condition, illustrating the conservative bias built into ITT estimates when compliance/exposure is imperfect."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["help-seeking"]
    predictors: ["intervention", "peer-mentoring"]
  - text: "Standard missing-data handling of last-observation-carried-forward (LOCF), still common in pharmaceutical ITT submissions, is statistically inefficient and introduces bias and misleadingly precise standard errors; the authors instead recommend full-information maximum likelihood or multiple imputation, both of which require only a missing-at-random assumption and were demonstrated on a two-stage Conduct Disorder diagnostic follow-up in the First Generation Baltimore Prevention Program trial."
    evidence: "case-study"
    support_strength: "moderate"
    outcomes: []
    predictors: ["sampling-method"]
population:
  who: "Not a single sampled population; a methods/framework paper illustrated using six US randomized field trials of universal, selective, and indicated prevention programs, spanning individual-, classroom-, school-, district-, and county-level randomization (e.g., Rochester Resilience Program, First and Third Generation Baltimore Prevention Program, Georgia Gatekeeper suicide-prevention training, Adolescent Substance Abuse Prevention Study, California MTFC trial)"
  where: ["United States"]
  when: null
  n: null
  sector: ["education", "public-health", "mental-health-services"]
  sample_notes: >
    Sample sizes for the illustrative trials range from roughly 470 children (Rochester
    Resilience Program) to 50,000 students (Georgia Gatekeeper); no single unified sample
    underlies the paper's own claims since it is a statistical-methods exposition, not a
    primary empirical study.
limitation:
  primary: "As a methods/framework paper, its own 'findings' are prescriptive standards and illustrative re-analyses rather than new substantive evidence about social connection or wellbeing, so support_strength for its claims reflects methodological consensus, not effect-size precision."
  others:
    - "Recommendations are built almost entirely from the authors' own multi-decade portfolio of prevention trials (Prevention Science and Methodology Group), limiting independent validation of the proposed ITT standards."
    - "The paper explicitly warns that its variation-in-impact methods (GAMM, GMM) can produce spurious subgroup findings if applied exploratorily without correction for multiple comparisons or theoretical pre-specification."
    - "Growth mixture / latent class models discussed are acknowledged elsewhere in the literature to be sensitive to distributional assumptions and can overextract classes."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Because the SNH project draws on suicide-prevention and prevention-science methodology,
  this paper is a foundational reference for how to correctly define analytic denominators,
  handle attrition/missing data, and test for who benefits under what conditions when the
  project runs or evaluates group-level interventions (e.g., team- or org-level social-
  support programs) rather than individually randomized ones; it directly informs how to
  avoid inflated or spurious subgroup claims about intervention impact on isolation,
  burnout, or belonging.
tags:
  topic: ["suicide-prevention", "methodology", "measurement"]
  method: ["case-study", "analytical"]
  population: ["students", "school-staff", "youth"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Methods for Testing Theory and Evaluating Impact in Randomized Field Trials - Intent-to-Treat Analyses/Methods for Testing Theory and Evaluating Impact in Randomized Field Trials - Intent-to-Treat Analyses.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Methods for Testing Theory and Evaluating Impact in Randomized Field Trials - Intent-to-Treat Analyses.pdf"
  notes: null

---

id: "american-2019-model-school-district-policy-on-suicide"
title: "Model School District Policy on Suicide Prevention: Model Language, Commentary, and Resources (2nd ed.)"
authors:
  - "American Foundation for Suicide Prevention"
  - "American School Counselor Association"
  - "National Association of School Psychologists"
  - "The Trevor Project"
year: 2019
doi: null
venue: {type: "report", name: "American Foundation for Suicide Prevention (joint publication with ASCA, NASP, and The Trevor Project)", volume: null, issue: null, pages: null}
citation: "American Foundation for Suicide Prevention et al. (2019). Model School District Policy on Suicide Prevention: Model Language, Commentary, and Resources (2nd ed.). American Foundation for Suicide Prevention (joint publication with ASCA, NASP, and The Trevor Project)."
article_type: "commentary"
method: {design: "design-report", approach: "analytical", evidence_level: "reference", preregistered: false}
gist: >
  This is the second edition of a jointly authored model school-district suicide prevention
  policy (AFSP, ASCA, NASP, The Trevor Project, 2019), providing ready-to-adopt policy
  language covering prevention, intervention, parental notification, re-entry, and
  postvention, plus a commentary section that synthesizes existing research on risk and
  protective factors, at-risk populations (LGBTQ, bullied, homeless, foster-care, and AI/AN
  youth), and safe-messaging/contagion guidance for districts designing their own protocols.
  It functions as a practice and design template rather than an original empirical study.
claims:
  - text: "Citing a 2017 study of bullied youth, the document reports that adolescents who are bullied (in person or online) are 19 times more likely to experience suicidal ideation than youth with no history of bullying."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation", "mental-health"]
    predictors: ["isolation", "social-support"]
  - text: "Citing national survey data, the policy states LGB youth are 4.5 times, and questioning youth over twice as likely, to consider suicide compared to heterosexual peers; separately, 40% of transgender respondents in the 2015 U.S. Transgender Survey reported a lifetime suicide attempt, 73% of those before age 18."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation", "mental-health"]
    predictors: ["isolation", "sense-of-belonging"]
  - text: "The commentary summarizes research that LGBT youth rejected by parents show much higher rates of depression, suicide, illegal drug use, and unprotected sex, while family acceptance and support is associated with higher self-esteem, lower suicidal ideation and self-harm, and better overall physical health."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation", "depression", "wellbeing"]
    predictors: ["social-support", "sense-of-belonging"]
population:
  who: "K-12 school districts and school-based staff/mental-health professionals in the U.S.; commentary draws on studies of general adolescents, LGBTQ youth, bullied youth, homeless youth, foster-care/juvenile-justice youth, and American Indian/Alaska Native youth"
  where: ["United States"]
  when: "Cited studies span roughly 2010-2018; document published 2019"
  n: null
  sector: ["education", "mental-health"]
  sample_notes: >
    Not a primary study; this is a policy/advocacy document with a commentary section that
    cites roughly 26 external studies and reports rather than collecting original data. No
    sampling, recruitment, or response-rate information applies.
limitation:
  primary: "As a policy and advocacy document rather than primary research, its evidentiary claims rely entirely on secondary citations to other studies of varying age, design, and rigor, without systematic review methodology or critical appraisal."
  others:
    - "No original data collection or evaluation of the model policy's real-world effectiveness is presented"
    - "Individual statistics (e.g., odds ratios, percentages) are drawn from single studies with no synthesis across sources or discussion of heterogeneity"
risk_of_bias: "not-applicable"
relevance_to_project: >
  Offers a concrete, field-tested template for operationalizing suicide-prevention practice
  into escalation protocols (risk assessment, referral, parental notification, postvention,
  safe messaging) that the SNH project can draw on when designing upstream crisis-response
  and community-support features, and it consolidates evidence on risk/protective factors
  (family rejection vs. acceptance, bullying, isolation, LGBTQ vulnerability) directly
  relevant to community health design decisions.
tags:
  topic: ["suicide-prevention", "mental-health", "isolation", "community-health"]
  method: ["design-report", "secondary-data"]
  population: ["adolescents", "lgbtq-youth", "school-based"]
source:
  markdown: "Papers_Data/Mental Health/MD/Model School Policy/Model School Policy.md"
  pdf: "papers/Mental Health/Model School Policy.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "anon-2016-cobbler-2-cobbler-peer-mentoring-program"
title: "Cobbler 2 Cobbler Peer Mentoring Program"
authors:
year: 2016
doi: null
venue: {type: "other", name: "REL Central Newsletter (NAERA), Marzano Research", volume: null, issue: null, pages: null}
citation: "REL Central Newsletter (NAERA), Marzano Research (2016). Cobbler 2 Cobbler Peer Mentoring Program. REL Central Newsletter (NAERA), Marzano Research."
article_type: "commentary"
method: {design: "case-study", approach: "other", evidence_level: "weak", preregistered: false}
gist: >
  This newsletter feature profiles Cobbler 2 Cobbler, a peer mentoring and suicide-
  prevention program at Rapid City Central High School (South Dakota) built on the Sources
  of Strength model, following a cluster of 28 student/staff deaths between 2007-2011. It
  reports that no teen suicides occurred at the school since September 2011 and situates
  that outcome alongside the Wyman et al. (2010) randomized controlled trial of Sources of
  Strength, which found trained peer leaders were four times more likely than untrained
  peers to refer a suicidal friend for adult help and that positive peer networks reduced
  bullying, substance abuse, and violence. It also describes program structure (a credit-
  bearing mentoring course, freshman seminars, ~175 peer mentors/year) and a partnership
  extending the model to the Pine Ridge Indian Reservation.
claims:
  - text: "In the Wyman et al. (2010) RCT of Sources of Strength (18 high schools, 453 trained peer leaders, 2,675 surveyed students), trained peer leaders were four times more likely than untrained peers to refer a suicidal friend to an adult for help."
    evidence: "rct"
    support_strength: "strong"
    outcomes: ["help-seeking"]
    predictors: ["peer-mentoring", "intervention"]
  - text: "The same trial found that establishing positive peer social networks in the school environment protected against suicide risk and also reduced bullying, substance abuse, mental health problems, and violence among the broader student population."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["mental-health", "wellbeing"]
    predictors: ["social-support", "peer-mentoring"]
  - text: "Since September 2011, Rapid City Central High School has had no teen suicides, which district leaders and the article suggest may be linked to the peer mentoring network, though no controlled evaluation of the local program itself is presented."
    evidence: "case-study"
    support_strength: "weak"
    outcomes: ["suicidal-ideation", "sense-of-belonging"]
    predictors: ["peer-mentoring", "community-engagement"]
population:
  who: "Students and peer mentors at Rapid City Central High School (~1,900 students, ~175 peer mentors/year); the embedded Wyman et al. (2010) RCT sampled 453 trained peer leaders and a representative 2,675 students across 18 high schools."
  where: ["United States - South Dakota"]
  when: "Program: 2008-2016; cited RCT data collection circa 2008-2009"
  n: null
  sector: ["education"]
  sample_notes: >
    This is a program profile/case study, not primary data collection by the author; the
    only rigorous quantitative figures (n=453 peer leaders, n=2,675 students, 18 schools, 6
    urban/12 rural) belong to the previously published Wyman et al. (2010) trial, not to new
    research on Cobbler 2 Cobbler specifically.
limitation:
  primary: "The piece is a promotional newsletter case study of one school's program, not an independent evaluation of Cobbler 2 Cobbler; the 'zero suicides since 2011' claim is a correlational, anecdotal observation rather than a controlled outcome measure."
  others:
    - "Some evidence is drawn from informally cited or unpublished sources (e.g., McGowan, 2015, unpublished manuscript; a personal communication about trusted-adult effects on decision-making) that cannot be independently verified."
    - "No comparison school or control condition is used to evaluate Cobbler 2 Cobbler's own effectiveness, unlike the cited Sources of Strength RCT."
risk_of_bias: "high"
relevance_to_project: >
  Documents a concrete, low-cost peer-support intervention model (trained near-peer mentors,
  structured referral norms, trusted-adult access) with a cited effect size (4x increase in
  help-seeking referrals) that the SNH project can reference when designing peer-support,
  check-in, or maintainer-wellbeing mechanisms aimed at increasing help-seeking and
  connectedness before crisis points.
tags:
  topic: ["suicide-prevention", "social-support", "community-health", "mental-health"]
  method: ["case-study"]
  population: ["students", "adolescents"]
source:
  markdown: "Papers_Data/Mental Health/MD/NAERA Newsletter Q1 2016 Focus Article Cobbler 2 Cobbler Peer Mentoring Program/NAERA Newsletter Q1 2016 Focus Article Cobbler 2 Cobbler Peer Mentoring Program.md"
  pdf: "papers/Mental Health/NAERA Newsletter Q1 2016 Focus Article Cobbler 2 Cobbler Peer Mentoring Program.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "jones-2022-navigating-sel-from-the-inside-out"
title: "Navigating SEL From the Inside Out: Looking Inside &amp; Across 18 Leading SEL Programs: A Practical Resource for Schools and OST Providers—Middle &amp; High School Focus"
authors:
  - "Jones, Stephanie M."
  - "Brush, Katharine E."
  - "Wettje, Samantha"
  - "Ramirez, Thelma"
  - "Poddar, Aashna"
  - "Kannarr, Alisha"
  - "Barnes, Sophie P."
  - "Hooper, Annie"
  - "Brion-Meisels, Gretchen"
  - "Chng, Edwin"
year: 2022
doi: "10.59656/yd-os7616.001"
venue: {type: "report", name: null, volume: null, issue: null, pages: null}
citation: "Jones et al. (2022). Navigating SEL From the Inside Out: Looking Inside &amp; Across 18 Leading SEL Programs: A Practical Resource for Schools and OST Providers—Middle &amp; High School Focus.. https://doi.org/10.59656/yd-os7616.001"
article_type: "review"
method: {design: "review-scoping", approach: "secondary-data", evidence_level: "low-to-moderate", preregistered: false}
gist: >
  This Harvard Graduate School of Education report (Jones et al., 2017, funded by the
  Wallace Foundation) content-analyzes 25 widely-used elementary-school social and emotional
  learning (SEL) and character-education programs, coding each program's classroom/OST
  activities against 12 SEL skills across five domains (cognitive regulation, emotional
  processes, interpersonal skills, character, mindset), 17 instructional methods, and 10
  program components. It does not test whether the programs work; instead it maps what each
  program actually contains so schools and out-of-school-time (OST) providers can compare
  programs and select ones matching their goals. It synthesizes prior evidence (notably
  Durlak et al. 2011's SAFE framework and Durlak, Weissberg & Pachan's 2010 review of 68
  afterschool programs) to identify features associated with effective SEL programming and
  seven recurring implementation challenges.
claims:
  - text: "Programs vary widely in skill emphasis even within the same broad SEL label: e.g., interpersonal-skill focus ranged from 18% of activities (MindUP) to 100% (Good Behavior Game), and emotional-process focus ranged from near 0% (Good Behavior Game, Playworks) to 94% (RULER), showing 'SEL program' is not a homogeneous category for evaluation or selection purposes."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["wellbeing", "mental-health"]
    predictors: ["intervention", "sampling-method"]
  - text: "Synthesizing prior research, the report identifies the SAFE framework (Durlak et al., 2011) -- Sequenced activities, Active learning, a Focus on skill development, and Explicit skill targeting -- as the strongest predictor of program effectiveness, and adds that programs work best when they also occur in supportive contexts, build adult social-emotional competence, and address the broader community context."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["mental-health", "wellbeing"]
    predictors: ["intervention", "leadership-style", "organizational-culture"]
  - text: "The report identifies seven common implementation challenges even for well-evidenced programs -- insufficient exposure/intensity, poor integration into daily practice, failure to extend SEL beyond the classroom (e.g., to unsupervised hallways/playgrounds where students report feeling least safe), inadequate staff training (especially for non-teaching staff), weak buy-in/ownership, low use of data for program decisions, and difficulty transferring skills to real-time situations."
    evidence: "review-scoping"
    support_strength: "low-to-moderate"
    outcomes: ["mental-health", "job-engagement"]
    predictors: ["organizational-culture", "leadership-style", "intervention"]
population:
  who: "25 commercially/publicly available elementary-school-focused SEL and character-education programs (in-school curricular, in-school non-curricular, and out-of-school-time programs) used in US schools and OST settings; program developers for 23 of 25 reviewed their own profile for accuracy."
  where: ["United States"]
  when: "Program materials and evaluations reviewed Fall 2015-Spring 2016"
  n: 25
  sector: ["education", "youth-services"]
  sample_notes: >
    Unit of analysis is programs (and their published curricular activities), not individual
    children or classrooms; the report itself synthesizes external evaluation evidence for
    each program (of varying design and rigor) rather than reporting a single primary study.
    15 programs were selected first for relevance/diversity/accessibility, with 10 more
    added later for character-education or OST focus, so program selection was purposive,
    not systematic or exhaustive of the SEL market.
limitation:
  primary: "This is a content/curriculum-coding exercise, not an effectiveness study: it documents what each program's activities target, not whether the program improves child outcomes, and effectiveness evidence cited for individual programs varies enormously in quality (from RCTs to unavailable/no formal evaluation)."
  others:
    - "Coding captured only explicit, concrete skill-targeting in a maximum of two instructional methods per activity, likely undercounting implicit or tertiary skill-building and instructional methods (acknowledged by the authors)."
    - "Sample of 25 programs was purposively selected for relevance, diversity, and material accessibility rather than being a comprehensive or randomly sampled census of SEL programs."
    - "Findings are specific to elementary-school-age programming in US contexts and may not generalize to secondary schools, other countries, or non-English-language programs."
risk_of_bias: "medium"
relevance_to_project: >
  Offers a transferable design lens for the SNH project's own intervention/toolkit work: the
  SAFE criteria (sequenced, active, focused, explicit) and the five 'key features of
  effective programs' (supportive context, adult competency-building, community context,
  multi-domain skill targeting, reasonable goal-setting) are a concrete checklist for
  designing or evaluating any structured social-connection or belonging intervention, and
  the seven implementation-challenge list (staff training gaps, weak buy-in, poor transfer
  of skills, lack of data-driven iteration) maps directly onto pitfalls the project should
  anticipate when rolling out community-health interventions in remote-work or open-source
  settings.
tags:
  topic: ["mental-health", "wellbeing", "methodology", "community-health"]
  method: ["review-scoping", "secondary-data"]
  population: ["education", "youth"]
source:
  markdown: "Papers_Data/Mental Health/MD/Navigating SEL From the Inside Out Looking Inside and Across 25 Leading SEL Programs A Practical Resource for Schools and OST Providers/Navigating SEL From the Inside Out Looking Inside and Across 25 Leading SEL Programs A Practical Resource for Schools and OST Providers.md"
  pdf: "papers/Mental Health/Navigating SEL From the Inside Out Looking Inside and Across 25 Leading SEL Programs A Practical Resource for Schools and OST Providers.pdf"
  notes: null

---

id: "murthy-2023-our-epidemic-of-loneliness-and-isolation"
title: "Our Epidemic of Loneliness and Isolation: The U.S. Surgeon General's Advisory on the Healing Effects of Social Connection and Community"
authors:
  - "Murthy, Vivek H."
year: 2023
doi: null
venue: {type: "report", name: "Office of the U.S. Surgeon General, U.S. Department of Health and Human Services", volume: null, issue: null, pages: null}
citation: "Murthy (2023). Our Epidemic of Loneliness and Isolation: The U.S. Surgeon General's Advisory on the Healing Effects of Social Connection and Community. Office of the U.S. Surgeon General, U.S. Department of Health and Human Services."
article_type: "review"
method: {design: "review-narrative", approach: "secondary-data", evidence_level: "strong", preregistered: false}
gist: >
  This U.S. Surgeon General's Advisory synthesizes hundreds of epidemiological,
  psychological, and sociological studies to argue that social disconnection is a public
  health epidemic with mortality and disease risk comparable to smoking, obesity, and
  physical inactivity. It documents declining U.S. social participation (more time alone,
  fewer close friendships, shrinking networks) since the early 2000s, quantifies workplace
  and economic costs of loneliness, and lays out a six-pillar national strategy (social
  infrastructure, public policy, health sector, digital environment reform, research, and
  culture change) with sector-specific recommendations including for workplaces and
  technology companies.
claims:
  - text: "Loneliness and social isolation increase the risk of premature death by 26% and 29% respectively, with the mortality impact of lacking social connection comparable to smoking up to 15 cigarettes a day; poor social connection is also associated with a 29% increased risk of heart disease and a 32% increased risk of stroke."
    evidence: "review-narrative"
    support_strength: "strong"
    outcomes: ["mortality", "mental-health"]
    predictors: ["loneliness", "isolation"]
  - text: "National objective-time-use data (2003-2020) show time spent alone increased by 24 hours/month while time engaged with friends in-person decreased by 20 hours/month, with the decline steepest among 15-24 year olds (down nearly 70%, from ~150 to ~40 minutes/day); one study found network size dropped 16% between June 2019 and June 2020."
    evidence: "review-narrative"
    support_strength: "moderate"
    outcomes: ["isolation", "loneliness"]
    predictors: ["network-structure", "community-engagement"]
  - text: "Supportive and inclusive workplace relationships are associated with employee job satisfaction, creativity, competence, and better job performance, and quality social support/integration among coworkers is key to preventing chronic work stress and burnout; stress-related absenteeism attributed to loneliness is estimated to cost U.S. employers $154 billion annually, while social isolation among older adults alone accounts for an estimated $6.7 billion in excess Medicare spending."
    evidence: "review-narrative"
    support_strength: "moderate"
    outcomes: ["job-satisfaction", "burnout", "productivity"]
    predictors: ["social-support", "team-cohesion"]
population:
  who: "General U.S. population across the lifespan; the advisory synthesizes findings from hundreds of independent epidemiological, psychological, and sociological studies, national surveys, and meta-analyses rather than reporting on a single sample"
  where: ["United States"]
  when: "Evidence reviewed primarily through 2022-2023; underlying data sources span roughly 1972-2022 (e.g., time-use surveys 2003-2020, trust polling 1972-2016)"
  n: null
  sector: ["public-health", "government"]
  sample_notes: >
    Not a primary study: an expert-informed narrative synthesis prioritizing meta-analyses
    and systematic reviews, supplemented by expert consultation (50+ reviewers); the
    advisory explicitly states it is not an exhaustive literature review, so study selection
    and inclusion criteria are not fully systematic or transparent.
limitation:
  primary: "As the advisory itself acknowledges, few underlying studies measure more than one social connection component (structure, function, quality) in the same sample, which confounds understanding of independent versus synergistic effects on health."
  others:
    - "The advisory notes that most existing research does not distinguish remote/technology-mediated social connection from traditional in-person connection, limiting conclusions about digital and remote-work contexts specifically."
    - "As a narrative (non-systematic) synthesis authored by a government office rather than an independent research team, it does not report formal inclusion criteria, quality appraisal, or effect-size pooling for the studies it cites."
    - "Much of the community-level evidence cited is correlational, and the advisory calls for further causal research, especially among underrepresented groups."
risk_of_bias: "medium"
relevance_to_project: >
  This advisory is a foundational evidence source for the SNH project's core premise: it
  supplies widely-cited effect-size benchmarks (mortality, cardiovascular, and workplace-
  productivity risks of loneliness/isolation) that justify treating social connection as a
  health and organizational priority, and its 'Reform Digital Environments' and 'Workplaces'
  recommendations directly inform design choices for remote-work and tech-community
  interventions, including its explicit call for more research distinguishing
  remote/technology-mediated connection from in-person connection.
tags:
  topic: ["loneliness", "isolation", "wellbeing", "mental-health", "burnout", "community-health"]
  method: ["review-narrative", "secondary-data"]
  population: ["general-population", "workers", "older-adults"]
source:
  markdown: "Papers_Data/Mental Health/MD/Our Epidemic of Loneliness and Isolation US Surgeon General Advisory on the Healing Effects of Social Connection and Community/Our Epidemic of Loneliness and Isolation US Surgeon General Advisory on the Healing Effects of Social Connection and Community.md"
  pdf: "papers/Mental Health/Our Epidemic of Loneliness and Isolation US Surgeon General Advisory on the Healing Effects of Social Connection and Community.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "steiner-1995-reducing-risks-for-mental-disorders-frontiers"
title: "Reducing Risks for Mental Disorders: Frontiers for Preventive Intervention Research"
authors:
  - "Steiner, Jeanne L."
year: 1995
doi: "10.1176/ps.46.7.736"
venue: {type: "journal", name: "Psychiatric Services", volume: 46, issue: 7, pages: "736-736"}
citation: "Steiner (1995). Reducing Risks for Mental Disorders: Frontiers for Preventive Intervention Research. Psychiatric Services, 46(7), 736-736. https://doi.org/10.1176/ps.46.7.736"
article_type: "review"
method: {design: "review-scoping", approach: "analytical", evidence_level: "moderate", preregistered: false}
gist: >
  This landmark 1994 Institute of Medicine committee report reframes prevention of mental
  disorders around a risk-reduction model and proposes the now-standard
  universal/selective/indicated classification of preventive interventions (adapted from
  Gordon 1983), distinguishing prevention (before onset) from treatment and maintenance. It
  synthesizes evidence on biological and psychosocial risk and protective factors across
  five illustrative disorders (conduct disorder, depression, alcohol dependence,
  schizophrenia, Alzheimer's disease) and reviews dozens of illustrative preventive-
  intervention trials across the lifespan, including several centered on social support,
  workplace stress, job loss, caregiving, and bereavement. It concludes with a national
  research agenda and funding recommendations for building prevention-research
  infrastructure.
claims:
  - text: "In a randomized controlled trial of the JOBS Project (selective intervention teaching job-search skills and social support to recent job losers), the experimental group showed significantly reduced depressive symptoms at 2.5-year follow-up and obtained higher-paying, higher-quality jobs; the ~$300-per-person intervention cost was rapidly offset by increased tax revenue, and effects were largest for participants at highest risk of subsequent depression."
    evidence: "rct"
    support_strength: "strong"
    outcomes: ["depression", "retention"]
    predictors: ["social-support", "intervention"]
  - text: "A randomized trial of the Caregiver Support Program (Heaney, 1992) for group-home caregivers of the mentally ill/developmentally disabled -- an occupation marked by relative social isolation and low supervisor support -- found the strongest effects on improved supervisor support and reduced supervisor undermining, plus reduced depressive symptoms and somatization among employees most at risk of leaving their jobs."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["depression", "turnover", "isolation"]
    predictors: ["social-support", "isolation", "leadership-style"]
  - text: "In a quasi-experimental study of THEOS mutual-help groups for widowed persons, experimental participants who formed strong social linkages within the group improved on six of eight mental health measures (depression, anxiety, somatic symptoms, well-being, self-esteem, mastery) relative to attendees who did not develop such linkages, while a comparison sample of widowed persons deteriorated on nearly all measures over one year."
    evidence: "case-study"
    support_strength: "low-to-moderate"
    outcomes: ["depression", "wellbeing", "isolation"]
    predictors: ["social-support", "community-engagement"]
population:
  who: "Not a single study population; a multidisciplinary IOM committee synthesis covering the U.S. general population, at-risk subgroups, and specific trial samples cited within (e.g., recent job losers in Michigan, group-home caregivers, newly widowed women in Toronto, low-income primary-care patients)."
  where: ["United States", "Canada"]
  when: "Literature reviewed through approximately 1993"
  n: null
  sector: ["mental-health-policy", "public-health"]
  sample_notes: >
    A 636-page consensus report commissioned by the U.S. Congress; underlying evidence base
    is a narrative (non-systematic) synthesis of a large but methodologically uneven
    literature, supplemented by commissioned background papers and expert conferences rather
    than a single defined study sample.
limitation:
  primary: "The committee itself states that at the time of writing there was little evidence from research that any specific mental disorder could actually be prevented; conclusions rest on risk-factor reduction logic rather than demonstrated incidence reduction for most disorders."
  others:
    - "Narrative/expert synthesis rather than a systematic or meta-analytic review, so study selection and weighting are not fully transparent or reproducible."
    - "Most illustrative intervention programs cited (e.g., caregiver, bereavement, job-loss programs) are single small-to-moderate trials, several quasi-experimental rather than randomized, with self-report outcome measures and unclear generalizability beyond the specific tested population."
    - "Now three decades old (1994); diagnostic criteria (DSM-III-R), funding figures, and the described federal research infrastructure are outdated relative to current practice."
risk_of_bias: "medium"
relevance_to_project: >
  This report is the origin of the universal/selective/indicated prevention framework the
  SNH project can use to classify interventions (e.g., a workplace-wide async-communication
  norm as universal, onboarding support for new remote hires as selective, an intervention
  triggered by detected disengagement signals as indicated). Its illustrative trials on
  workplace social support (Caregiver Support Program), job loss and reemployment (JOBS
  Project), and social-linkage effects in mutual-help groups (THEOS) provide directly
  transferable evidence that structured social-support interventions measurably reduce
  depressive symptoms and isolation-related distress, informing both intervention design and
  expected effect sizes for SNH prevention pilots.
tags:
  topic: ["mental-health", "isolation", "social-support", "wellbeing", "suicide-prevention"]
  method: ["review-scoping", "rct"]
  population: ["general-population", "workers", "caregivers"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Reducing Risks for Mental Disorders Frontiers for Preventive Intervention Research/Reducing Risks for Mental Disorders Frontiers for Preventive Intervention Research.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Reducing Risks for Mental Disorders Frontiers for Preventive Intervention Research.pdf"
  notes: null

---

id: "mccauley-2013-relational-cultural-theory-fostering-healthy-coexistence"
title: "Relational-Cultural Theory: Fostering Healthy Coexistence Through a Relational Lens"
authors:
  - "McCauley, Melissa"
year: 2013
doi: null
venue: {type: "other", name: "Beyond Intractability (Conflict Information Consortium, University of Colorado Boulder)", volume: null, issue: null, pages: null}
citation: "McCauley (2013). Relational-Cultural Theory: Fostering Healthy Coexistence Through a Relational Lens. Beyond Intractability (Conflict Information Consortium, University of Colorado Boulder)."
article_type: "theory"
method: {design: "theory", approach: "analytical", evidence_level: "speculative", preregistered: false}
gist: >
  This essay synthesizes Relational-Cultural Theory (RCT), a feminist-psychology framework
  developed at the Stone Center at Wellesley (Jean Baker Miller, Judith Jordan, Janet
  Surrey, Irene Stiver), and applies its concepts of connection, disconnection, mutuality,
  and 'condemned isolation' to conflict transformation and peacebuilding. It argues that
  disconnection is a source of psychological suffering with a neurological basis, that
  dominant groups use shame and isolation to maintain subordination, and that community-
  based resistance strategies (naming, complaining, claiming strength, building communities
  of resilience) can rebuild connection and drive social transformation.
claims:
  - text: "RCT holds that 'growth-fostering relationships' require mutuality (the 'Five Good Things': zest, sense of worth, clarity, productivity, and desire for more connection), and that the absence of mutuality contributes to psychological problems and to the rise of violent conflict."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["wellbeing", "mental-health", "sense-of-belonging"]
    predictors: ["social-support", "psychological-safety"]
  - text: "Citing the Social Pain/Physical Pain Overlap Theory (Eisenberger & Lieberman), the essay argues disconnection produces real, biologically-grounded pain, while neuroplasticity research suggests empathic capacity and relational repair remain possible across the lifespan even after early attachment harm."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["mental-health", "isolation", "wellbeing"]
    predictors: ["isolation", "loneliness"]
  - text: "'Condemned isolation' describes how dominant groups use shame and enforced isolation to keep subordinated individuals feeling shut out of the human community and unable to reconnect; the essay proposes a four-step resistance sequence (naming the problem, complaining, claiming strength, developing communities of resilience and courage) as a pathway out of isolation toward mutuality."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["isolation", "sense-of-belonging", "wellbeing"]
    predictors: ["social-support", "community-engagement", "inclusiveness"]
population:
  who: "Not an empirical study; a conceptual essay synthesizing psychological theory (RCT) and peacebuilding/conflict-transformation literature, illustrated with secondary examples (e.g., dance movement therapy with ex-child soldiers in Sierra Leone, Seeds of Peace youth dialogue programs)."
  where: []
  when: null
  n: null
  sector: ["mental-health", "civil-society"]
  sample_notes: >
    No primary sample; written as a graduate (MA Peace Studies) capstone essay drawing
    entirely on secondary sources (bibliography of ~20 works), published on the Beyond
    Intractability knowledge-base website with two named peer reviewers.
limitation:
  primary: "Purely theoretical/synthesis piece with no original data collection, empirical test, or systematic literature search methodology described."
  others:
    - "Single-author graduate essay published on a practitioner knowledge-base site rather than peer-reviewed academic literature, so claims rest on selective secondary citation."
    - "Applies RCT (originally a feminist clinical psychology framework) to peacebuilding by analogy, with no empirical evaluation of whether RCT-informed interventions actually improve coexistence outcomes."
    - "Neuroscience claims (e.g., social/physical pain overlap) are asserted via a single secondary citation without discussion of effect sizes or replication status."
risk_of_bias: "not-applicable"
relevance_to_project: >
  RCT's concept of 'condemned isolation' -- shame-driven, self-reinforcing withdrawal from
  community -- and its 'growth-fostering relationship' model (mutuality, zest, sense of
  worth) offer a psychological vocabulary for how isolation is created and maintained, and a
  resistance sequence (naming, complaining, claiming strength, building communities of
  resilience) that could inform design interventions aimed at helping isolated remote
  workers or marginalized contributors reconnect rather than withdraw further.
tags:
  topic: ["isolation", "loneliness", "community-health", "social-support", "wellbeing", "mental-health"]
  method: ["theory"]
  population: ["general-population", "conflict-affected-groups"]
source:
  markdown: "Papers_Data/Mental Health/MD/Relational-Cultural Theory Fostering Healthy Coexistence Through a Relational Lens/Relational-Cultural Theory Fostering Healthy Coexistence Through a Relational Lens.md"
  pdf: "papers/Mental Health/Relational-Cultural Theory Fostering Healthy Coexistence Through a Relational Lens.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "anon-nd-research-summaries"
title: "Research Summaries"
authors:
year: null
doi: null
venue: {type: "other", name: "Unknown (internal research-summary compilation; underlying studies published in Journal of Child Psychology and Psychiatry, JAMA Network Open, and American Journal of Public Health)", volume: null, issue: null, pages: null}
citation: "Unknown (internal research-summary compilation; underlying studies published in Journal of Child Psychology and Psychiatry, JAMA Network Open, and American Journal of Public Health) (None). Research Summaries. Unknown (internal research-summary compilation; underlying studies published in Journal of Child Psychology and Psychiatry, JAMA Network Open, and American Journal of Public Health)."
article_type: "review"
method: {design: "review-scoping", approach: "secondary-data", evidence_level: "moderate", preregistered: false}
gist: >
  This is an internal research-summary compilation extracting key findings from four
  published studies on network-based suicide prevention: a 38-high-school network study of
  10,291 students linking friendship/adult-network integration to lower suicidal ideation
  and attempts, a cluster-RCT of the Wingman-Connect program for Air Force trainees, a
  social-network-analysis follow-up of that same RCT, and an outcome evaluation of
  adolescent peer-leader suicide-prevention training. Together the excerpts build the case
  that strengthening group cohesion and youth-adult or unit-level social bonds is a viable
  upstream, population-level suicide-prevention strategy, distinct from individual-risk-
  focused approaches.
claims:
  - text: "Across 38 high schools (n=10,291 students), schoolwide suicide ideation rates were higher where there were more peer isolates, fewer friendship ties, and smaller, less dense friendship groups; students with more friendship ties in larger, interconnected groups were less likely to report suicide ideation or attempts."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation"]
    predictors: ["network-structure", "isolation", "sense-of-belonging"]
  - text: "In a cluster-randomized trial, the Wingman-Connect group-cohesion training reduced suicidal ideation and depression symptoms and produced a nearly 50% reduction in occupational impairment (corrective training, negative counseling) among Air Force personnel in technical training."
    evidence: "rct"
    support_strength: "strong"
    outcomes: ["depression", "suicidal-ideation", "stress"]
    predictors: ["team-cohesion", "intervention", "sense-of-belonging"]
  - text: "Social network analysis of the same RCT found Wingman-Connect counteracted the typical drift toward disconnection among Airmen at elevated suicide risk (10% of at-risk controls had zero unit connections by one-month follow-up); at-risk Airmen in the intervention made roughly three times more new valued-connection nominations than others."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["isolation", "sense-of-belonging"]
    predictors: ["intervention", "network-structure"]
population:
  who: "Composite of three distinct samples summarized across the four studies: (1) 10,291 students in 38 U.S. high schools; (2) U.S. Air Force personnel in technical training who received the Wingman-Connect program (cluster-randomized units); (3) adolescent peer leaders and their schools in an earlier suicide-prevention peer-training evaluation."
  where: ["United States"]
  when: "2010-2020 (publication dates of the summarized studies)"
  n: null
  sector: ["education", "military"]
  sample_notes: >
    This document is a set of extracted excerpts/findings from four separate published
    papers (Wyman et al., various years/journals), not an original study; no independent
    sampling was conducted, and per-study n and methodological detail are only partially
    given in the excerpts (e.g., the 10,291-student figure is stated, but Wingman-Connect
    and peer-leader study sample sizes are not restated here).
limitation:
  primary: "The document is a curated set of selective quotations and paraphrases pulled from four separate papers rather than an original analysis or full-text review, so methodological details, effect-size context, and caveats from the source papers are only partially preserved."
  others:
    - "No DOIs, full citations, or consistent authorship are given for the underlying studies within this file, making independent verification dependent on locating the original papers."
    - "Findings from four different populations (adolescents in schools vs. military trainees) are juxtaposed without noting how well suicide-prevention mechanisms generalize across these very different contexts."
risk_of_bias: "unclear"
relevance_to_project: >
  Directly supports the SNH project's upstream, network-level suicide-prevention framing: it
  evidences that group cohesion-building interventions (Wingman-Connect's
  Kinship/Purpose/Guidance/Balance model) and peer-adult network integration measurably
  increase social integration and help-seeking acceptability and reduce suicide risk and
  depression, offering a template for designing cohesion-building interventions for isolated
  remote workers or open-source contributors.
tags:
  topic: ["suicide-prevention", "community-health", "social-support", "isolation", "mental-health"]
  method: ["review-scoping", "secondary-data"]
  population: ["adolescents", "military-personnel"]
source:
  markdown: "Papers_Data/Mental Health/MD/Research Summaries.docx/Research Summaries.docx.md"
  pdf: null
  notes: "no-doi: confirmed none (manual review)"

---

id: "oyserman-2002-rethinking-individualism-and-collectivism-evaluation-of"
title: "Rethinking individualism and collectivism: Evaluation of theoretical assumptions and meta-analyses."
authors:
  - "Oyserman, Daphna"
  - "Coon, Heather M."
  - "Kemmelmeier, Markus"
year: 2002
doi: "10.1037/0033-2909.128.1.3"
venue: {type: "journal", name: "Psychological Bulletin", volume: 128, issue: 1, pages: "3-72"}
citation: "Oyserman et al. (2002). Rethinking individualism and collectivism: Evaluation of theoretical assumptions and meta-analyses.. Psychological Bulletin, 128(1), 3-72. https://doi.org/10.1037/0033-2909.128.1.3"
article_type: "review"
method: {design: "review-systematic", approach: "secondary-data", evidence_level: "moderate", preregistered: false}
gist: >
  A landmark meta-analysis (83 studies) plus narrative review (170 studies) testing whether
  European Americans are actually more individualistic and less collectivistic than other
  groups, as widely assumed in psychology. The authors find real but modest and inconsistent
  differences: European Americans are higher in individualism and lower in collectivism than
  East Asians and some Latin Americans, but are not more individualistic than African
  Americans or Latinos, and are not less collectivistic than Japanese or Koreans -- only
  Chinese samples show large individualism-collectivism gaps. Effects on self-concept and
  relationality are moderate; effects on attribution/cognitive style are large. The paper
  argues that individualism-collectivism scales are often overly broad and unreliable,
  conflating distinct constructs such as duty-to-group versus enjoyment of belonging, and
  that felt belonging/relatedness should be studied separately from collectivism proper.
claims:
  - text: "Across international and within-U.S. meta-analyses (83 studies), European Americans/Canadians were on average more individualistic and less collectivistic than other groups, but effect sizes were generally small; European Americans were not more individualistic than African Americans or Latinos, and were not less collectivistic than Japanese or Koreans."
    evidence: "review-systematic"
    support_strength: "moderate"
    outcomes: ["sense-of-belonging"]
    predictors: ["cultural-individualism-collectivism"]
  - text: "Within the United States, African Americans emerged as the most individualistic ethnic group (more so than European Americans), while Asian Americans and Latino Americans were higher in collectivism than European Americans; only the European American vs. Asian American comparison matched the expected pattern of higher individualism and lower collectivism for European Americans."
    evidence: "review-systematic"
    support_strength: "moderate"
    outcomes: ["sense-of-belonging"]
    predictors: ["cultural-individualism-collectivism"]
  - text: "Among East Asian groups, only people of Chinese origin (PR China, Taiwan, Hong Kong) showed large, robust individualism-collectivism effects versus Americans; Japanese and Koreans showed small or non-significant differences, and effect size depended heavily on scale reliability and content -- roughly half of cross-national scales had Cronbach's alpha below .70, and including 'belonging'/'advice-seeking' items versus 'duty' items changed both the size and direction of group differences."
    evidence: "review-systematic"
    support_strength: "moderate"
    outcomes: ["communication"]
    predictors: ["cultural-individualism-collectivism", "sampling-method"]
population:
  who: "83 studies (over 80% using undergraduate samples) used in cross-national and within-U.S. meta-analyses comparing European Americans/Canadians to other countries and to U.S. ethnic/racial groups (African American, Asian American, Latino American); a further, largely overlapping set of 170 studies (also mostly college students) reviewed narratively for individualism-collectivism's psychological implications."
  where: ["United States", "Canada", "multiple countries in cross-national comparisons, concentrated on Japan, Korea, Hong Kong, and PR China"]
  when: "Literature published 1980 through 1999"
  n: 83
  sector: ["higher-education"]
  sample_notes: >
    Over 80% of meta-analyzed studies used college undergraduates; within-U.S. comparisons
    were limited to European, African, Asian, and Latino Americans (no Native American data
    were found in the literature); cross-national data were heavily concentrated on four
    East Asian countries, with too few studies from Africa, Latin America, or most other
    regions to support stable regional conclusions.
limitation:
  primary: "Roughly half of cross-national individualism/collectivism scales (and most within-U.S. scales) had Cronbach's alpha below .70, and scale content varies idiosyncratically across studies (some include belonging/advice-seeking items, others only duty-to-group items), which the authors show changes both the size and direction of measured cultural differences."
  others:
    - "Over 80% of underlying studies used college undergraduates, limiting generalizability to broader populations."
    - "Cross-national evidence is heavily concentrated on four East Asian countries; data on Africa, Latin/South America, and most of the rest of the world are too sparse for stable conclusions."
    - "Most reviewed studies never directly assessed individualism or collectivism, instead using national origin or ethnicity as a proxy, confounding 'culture' with other country-level factors such as GNP and civil rights."
risk_of_bias: "medium"
relevance_to_project: >
  Cautions the SNH project against treating 'collectivist' or 'individualist' cultural
  framing as a simple predictor of community engagement, belonging, or support-seeking in
  distributed/remote teams and open-source communities -- the paper shows that felt
  belonging and enjoyment of group membership behave differently from duty-bound
  collectivism, which is directly relevant to how SNH operationalizes and validates sense-
  of-belonging and social-support measures across culturally diverse populations.
tags:
  topic: ["community-health", "wellbeing", "measurement", "methodology"]
  method: ["review-systematic", "secondary-data"]
  population: ["college-students", "cross-cultural"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Rethinking Individualism and Collectivism Evaluation of Theoretical Assumptions and Meta-Analyses/Rethinking Individualism and Collectivism Evaluation of Theoretical Assumptions and Meta-Analyses.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Rethinking Individualism and Collectivism Evaluation of Theoretical Assumptions and Meta-Analyses.pdf"
  notes: null

---

id: "ziegel-1995-the-handbook-of-research-synthesis"
title: "The Handbook of Research Synthesis"
authors:
  - "Ziegel, Eric R."
  - "Cooper, H."
  - "Hedges, L."
year: 1995
doi: "10.2307/1269651"
venue: {type: "journal", name: "Technometrics", volume: 37, issue: 2, pages: "242"}
citation: "Ziegel et al. (1995). The Handbook of Research Synthesis. Technometrics, 37(2), 242. https://doi.org/10.2307/1269651"
article_type: "commentary"
method: {design: "theory", approach: "analytical", evidence_level: "speculative", preregistered: false}
gist: >
  This is a short 1995 Technometrics book-review column in which Eric Ziegel briefly
  evaluates The Handbook of Research Synthesis (eds. Cooper & Hedges), bundled alongside
  unrelated reviews of three other statistics/AI books in the same journal section. The
  relevant paragraph describes the handbook as a 32-chapter, 10-section reference organizing
  meta-analysis practice around six decision points and praises its editorial attention to
  consistent notation and terminology. It contains no primary data or findings on social
  network health topics; its only use here is as a pointer to a canonical meta-analysis
  methodology text.
claims:
  - text: "The Handbook of Research Synthesis is structured as 32 chapters across 10 sections, each section built around a 'central decision point' in conducting a research synthesis: problem formulation, literature searching, literature evaluation, statistical description and combination of studies, statistical analysis of effect size, and reporting of results."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["research-synthesis-quality"]
    predictors: ["evidence-synthesis-method"]
  - text: "The reviewer characterizes the handbook as 'the most comprehensive treatment that can be imagined for this topic,' noting the editors enforced consistent mathematical notation, common terminology, and consistent rounding of numerical results across the volume's contributors."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["research-synthesis-quality"]
    predictors: ["evidence-synthesis-method"]
population:
  who: "Not a study of a human population; this is a book review whose subject (The Handbook of Research Synthesis) targets researchers conducting meta-analyses, identified in the foreword as information scientists, psychologists, social policy analysts, and educators."
  where: []
  when: null
  n: null
  sector: ["academic-research"]
  sample_notes: >
    N/A - no primary sample; the reviewed handbook itself draws its 32 chapters'
    contributors from information science, psychology, social policy, and education, plus
    some statisticians.
limitation:
  primary: "The paragraph specific to this handbook is only a few sentences long (the full review spans a single printed page, p. 242, shared across four unrelated book notices) and offers no critical assessment of the handbook's statistical methods, effect-size formulas, or empirical validity beyond structural description and praise."
  others:
    - "The markdown conversion bundles this review together with three unrelated book reviews (an AI/statistics conference volume, a data-sets handbook, and a Tukey collected-works volume), none relevant to SNH."
    - "No excerpted content from inside the Handbook of Research Synthesis itself is provided, only the reviewer's outside summary of its table of contents and editorial policy."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Relevant only as a bibliographic pointer to Cooper & Hedges' Handbook of Research
  Synthesis as a canonical meta-analysis methodology reference the SNH project could consult
  when systematically synthesizing evidence across its own corpus; the review itself
  supplies no SNH-specific evidence, measures, or mechanisms.
tags:
  topic: ["methodology", "measurement"]
  method: ["analytical"]
  population: ["researchers-meta-analysts"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Review - The Handbook of Research Synthesis by Cooper and Hedges - Ziegel Technometrics 1995/Review - The Handbook of Research Synthesis by Cooper and Hedges - Ziegel Technometrics 1995.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Review - The Handbook of Research Synthesis by Cooper and Hedges - Ziegel Technometrics 1995.pdf"
  notes: null

---

id: "rose-2006-sick-individuals-and-sick-populations"
title: "Sick Individuals and Sick Populations"
authors:
  - "Rose, Geoffrey"
year: 2006
doi: "10.1093/oso/9780195180848.003.0003"
venue: {type: "book", name: "Public Health Ethics", volume: null, issue: null, pages: "33-43"}
citation: "Rose (2006). Sick Individuals and Sick Populations. Public Health Ethics, 33-43. https://doi.org/10.1093/oso/9780195180848.003.0003"
article_type: "theory"
method: {design: "theory", approach: "analytical", evidence_level: "reference", preregistered: false}
gist: >
  Rose distinguishes two epidemiological questions -- 'why did this individual get this
  disease' versus 'why does this population have so much of the disease' -- and argues they
  demand different study designs and different prevention strategies. Using examples such as
  UK water hardness and cardiovascular mortality, blood pressure in Kenyan nomads versus
  London civil servants, and Finnish versus Japanese cholesterol distributions, he shows
  that a cause uniformly present within a population cannot be detected by within-population
  case-control or cohort methods, only by comparing populations. He then contrasts the
  'high-risk' prevention strategy, which targets susceptible individuals but has weak
  predictive power and is often behaviourally inappropriate, against the 'population
  strategy,' which shifts the whole risk distribution and yields larger aggregate benefit
  despite offering each individual only a small gain (the 'Prevention Paradox').
claims:
  - text: "A calculation from Framingham data suggests that a 10 mmHg downward shift in the whole population's blood pressure distribution would correspond to roughly a 30% reduction in total attributable cardiovascular mortality, illustrating the larger aggregate payoff of population-wide risk-factor shifts over individually targeted treatment."
    evidence: "theory"
    support_strength: "moderate"
    outcomes: ["population-health"]
    predictors: ["intervention"]
  - text: "Using UK Down's syndrome birth data, mothers under 30 have the lowest individual risk (0.7 per 1000 births) yet, because they are so numerous, account for 51% of all Down's syndrome cases, whereas high-risk mothers aged 40+ generate only about 13% of cases combined -- demonstrating the 'Prevention Paradox' that a large number of people at small risk can produce more disease than a small number at high risk."
    evidence: "theory"
    support_strength: "moderate"
    outcomes: ["population-health"]
    predictors: ["risk-distribution"]
  - text: "In the WHO clofibrate trial, a cholesterol-lowering drug given as a population-level preventive intervention appears to have killed more people than it saved even though the excess fatal complication rate was only about 1 per 1000 per year, showing that small individual risks from new mass interventions can be hard to detect yet decisive for the population risk-benefit balance."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["population-health"]
    predictors: ["intervention"]
population:
  who: "Not a single study population; a theoretical essay illustrating its argument with data borrowed from several previously published studies -- Framingham Study participants, UK Heart Disease Prevention Project screenees, Kenyan nomads, London civil servants, and UK birth records used for Down's syndrome-by-maternal-age rates."
  where: ["UK", "Kenya", "Japan", "Finland", "USA"]
  when: null
  n: null
  sector: []
  sample_notes: >
    No original sample: reiteration of a 1984 lecture (published 1985) that synthesizes and
    re-analyzes figures from other researchers' cited studies rather than presenting new
    primary data.
limitation:
  primary: "This is a theoretical/synthesis essay, not an empirical study -- its illustrative examples and effect sizes are drawn from other researchers' data (Framingham, UK Heart Disease Prevention Project, Alberman's Down's syndrome data) rather than original analysis, so specifics should be verified against their primary sources."
  others:
    - "Focuses entirely on physical-disease epidemiology (blood pressure, cholesterol, cancer); its 'high-risk vs population strategy' framework is extrapolated to social/behavioral health domains like SNH by analogy, not tested there."
    - "Written in 1985 from a UK public-health vantage point; some cited examples (e.g., the clofibrate trial) and behavior-change assumptions predate modern implementation science."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Rose's high-risk-vs-population framework is the classic argument for why SNH interventions
  aimed only at screening and supporting 'at-risk' individuals (e.g., flagging high-burnout
  or high-loneliness people) will systematically miss most future cases, since most burnout,
  isolation, or turnover arises from the large number of moderately exposed people rather
  than the small high-risk tail -- supporting complementary population-level, norm- and
  culture-shifting interventions (e.g., organization-wide workload, autonomy, or connection-
  norm changes) alongside individual-level support.
tags:
  topic: ["methodology", "community-health", "suicide-prevention"]
  method: ["theory"]
  population: ["general-population"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Sick Individuals and Sick Populations/Sick Individuals and Sick Populations.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Sick Individuals and Sick Populations.pdf"
  notes: null

---

id: "fried-2020-systems-all-the-way-down-embracing"
title: "Systems all the way down: embracing complexity in mental health research"
authors:
  - "Fried, Eiko I."
  - "Robinaugh, Donald J."
year: 2020
doi: "10.1186/s12916-020-01668-w"
venue: {type: "journal", name: "BMC Medicine", volume: 18, issue: 1, pages: null}
citation: "Fried et al. (2020). Systems all the way down: embracing complexity in mental health research. BMC Medicine, 18(1). https://doi.org/10.1186/s12916-020-01668-w"
article_type: "commentary"
method: {design: "theory", approach: "analytical", evidence_level: "speculative", preregistered: false}
gist: >
  This editorial introduces a BMC Medicine collection on complexity in mental health
  research, arguing across six inaugural papers that psychopathology emerges from
  multifactorial systems spanning biological, psychological, and social levels rather than
  from single causes, and that these systems show both multifinality and equifinality. It
  summarizes contributions on childhood-trauma mechanisms, neurobiological resilience,
  network analysis of adolescent resilience factors, psychological primitives underlying
  suicidal thoughts, and computational/complex-systems approaches to psychotherapy. It calls
  for mental health research to adopt tools from complexity science (network analysis,
  computational modeling, attractor-state concepts) to explain, predict, and intervene on
  mental disorders.
claims:
  - text: "Synthesizing the six collection papers, the editorial argues mental disorders are massively multifactorial and exhibit both multifinality (the same causal agents can produce different mental health outcomes) and equifinality (diverse causes can produce the same disorder), such that little evidence supports any single factor being necessary or sufficient for a given disorder."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["mental-health"]
    predictors: ["network-structure"]
  - text: "Summarizing Fritz et al.'s network analysis of adolescents ages 14-17 with and without childhood adversity, the editorial reports resilience factors such as family support and self-esteem show weaker interrelations during early adolescence following child adversity, suggesting the positive feedback loop (family support -> less distress -> self-esteem -> family cohesion -> family support) is disrupted."
    evidence: "longitudinal"
    support_strength: "low-to-moderate"
    outcomes: ["mental-health", "wellbeing"]
    predictors: ["social-support"]
  - text: "The editorial highlights proposals that computational modelling and complex-systems concepts (attractor states, early-warning signals, network destabilization) can serve as thinking, didactic, prediction, and treatment-selection tools in psychotherapy, and that a complex-systems approach to psychotherapy is described as both viable and necessary for advancing the field."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["mental-health"]
    predictors: ["intervention"]
population:
  who: "Not an empirical sample; the editorial characterizes six invited papers in a BMC Medicine special collection on complexity in mental health research, spanning childhood-trauma cohorts, adolescent resilience-network studies, and theoretical/computational psychotherapy papers."
  where: []
  when: "2019-2020"
  n: null
  sector: ["healthcare"]
  sample_notes: >
    Editorial with no primary data collection of its own; population details (e.g.,
    adolescents aged 14-17 with/without childhood adversity in Fritz et al.) belong to the
    cited studies and are not independently evaluable for representativeness from this text.
limitation:
  primary: "As an editorial introducing a collection, it presents no independent data or systematic evidence synthesis of its own; its characterizations of the six papers are the editors' summarized interpretations rather than verifiable full-study findings."
  others:
    - "The six summarized papers are heterogeneous in design (narrative review, neurobiology overview, network analysis, theoretical framework, two psychotherapy-focused theory papers), so claims drawn from the editorial mix evidence of very different strength."
    - "Most of the summarized work concerns childhood trauma/resilience or clinical psychotherapy rather than adult workplace or remote-work populations."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Frames mental health as an emergent property of interacting biological, psychological, and
  social systems rather than of single risk factors, supporting the SNH project's rationale
  for modeling network-level social support and isolation dynamics (not just individual
  predictors) and for considering computational/network-analytic tools to model how
  workplace social systems evolve toward burnout or resilience.
tags:
  topic: ["mental-health", "methodology", "community-health"]
  method: ["theory"]
  population: ["adolescents", "clinical-sample"]
source:
  markdown: "Papers_Data/Mental Health/MD/Systems All the Way Down Embracing Complexity in Mental Health Research/Systems All the Way Down Embracing Complexity in Mental Health Research.md"
  pdf: "papers/Mental Health/Systems All the Way Down Embracing Complexity in Mental Health Research.pdf"
  notes: null

---

id: "kendler-2012-the-dappled-nature-of-causes-of"
title: "The dappled nature of causes of psychiatric illness: replacing the organic–functional/hardware–software dichotomy with empirically based pluralism"
authors:
  - "Kendler, K S"
year: 2012
doi: "10.1038/mp.2011.182"
venue: {type: "journal", name: "Molecular Psychiatry", volume: 17, issue: 4, pages: "377-388"}
citation: "Kendler (2012). The dappled nature of causes of psychiatric illness: replacing the organic–functional/hardware–software dichotomy with empirically based pluralism. Molecular Psychiatry, 17(4), 377-388. https://doi.org/10.1038/mp.2011.182"
article_type: "theory"
method: {design: "theory", approach: "analytical", evidence_level: "moderate", preregistered: false}
gist: >
  Kendler argues that psychiatric illness does not sort cleanly into 'organic/hardware'
  versus 'functional/software' problems, as Cartesian dualism and computer-functionalist
  thinking imply. Reviewing 11 categories of causal 'difference-makers' (from molecular
  genetics through culture) for schizophrenia, major depression, and alcohol dependence, he
  shows each disorder's causes are 'dappled' across biological, psychological, and social-
  cultural levels rather than confined to one domain, with these levels mediating and
  moderating one another. He proposes 'empirically based pluralism'-grounded in what
  research actually finds, not a priori theoretical commitment-as the replacement framework,
  distinguishing it from Engel's biopsychosocial model by claiming stronger empirical
  discipline.
claims:
  - text: "Across schizophrenia, major depression, and alcohol dependence, difference-makers are distributed across biological, psychological, and higher-order (social/political/cultural) domains rather than clustering at either a purely 'organic' or 'functional' pole, contradicting the hardware-software prediction."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["mental-health"]
    predictors: ["social-support", "network-structure"]
  - text: "For all three disorders, aggregate genetic effects account for the single largest share of estimated variance in liability (e.g., ~80% heritability for schizophrenia, ~40% for major depression, 50-60% for alcohol dependence), though this partly reflects that genetic effects have been the most thoroughly quantified category."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["mental-health"]
    predictors: ["social-support"]
  - text: "In a study of childhood sexual abuse and major depression, disclosure and response mattered as much as the abuse itself: risk of lifetime MD rose ~50% further if disclosure met a negative response, but fell back near control levels if disclosure led the abuse to stop-illustrating that psychological/social meaning (felt abandonment vs. protection), not only biological insult, functions as a causal difference-maker."
    evidence: "cross-sectional"
    support_strength: "low-to-moderate"
    outcomes: ["mental-health", "depression"]
    predictors: ["social-support", "loneliness"]
population:
  who: "Not an empirical sample; a narrative/expert-review synthesis of the psychiatric genetics, neuroscience, and psychosocial epidemiology literature on schizophrenia, major depression, and alcohol dependence, drawing partly on the author's own twin/family studies."
  where: []
  when: null
  n: null
  sector: ["mental-health"]
  sample_notes: >
    No primary sample; 'population' is the body of published research the author selectively
    reviews and subjectively weights into causal-signature estimates (his own words: 'a
    necessarily subjective exercise').
limitation:
  primary: "The core 'causal signature' percentages allocating variance across 11 categories are explicitly the author's subjective judgment calls, not a systematic quantitative synthesis (e.g., not a formal meta-analysis or variance-decomposition model), so the dappled pattern is illustrative rather than statistically estimated."
  others:
    - "As a conceptual/theoretical essay rather than a systematic review, source selection is not documented with reproducible search or inclusion criteria."
    - "Findings are pitched at the level of disorders in aggregate, and the author acknowledges the same pluralistic pattern may not describe any individual patient's specific etiology."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Provides conceptual grounding for why the SNH project should treat social/relational
  factors (support, disclosure, belonging) as genuine, non-reducible difference-makers in
  mental-health outcomes alongside biological ones-useful for arguing against dismissing
  social interventions as merely 'downstream' of biology, and for framing
  burnout/isolation/loneliness as one tier in a multi-level causal system rather than a
  single dominant cause.
tags:
  topic: ["mental-health", "suicide-prevention"]
  method: ["review-scoping"]
  population: ["clinical-mental-health"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/The Dappled Nature of Causes of Psychiatric Illness - Replacing the Hardware-Software Dichotomy with Empirically Based Pluralism/The Dappled Nature of Causes of Psychiatric Illness - Replacing the Hardware-Software Dichotomy with Empirically Based Pluralism.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/The Dappled Nature of Causes of Psychiatric Illness - Replacing the Hardware-Software Dichotomy with Empirically Based Pluralism.pdf"
  notes: null

---

id: "list-2022-the-five-vital-signs-of-a"
title: "The Five Vital Signs of a Scalable Idea and How to Avoid a Voltage Drop"
authors:
  - "List, John A."
year: 2022
doi: null
venue: {type: "other", name: "Behavioral Scientist", volume: null, issue: null, pages: null}
citation: "List (2022). The Five Vital Signs of a Scalable Idea and How to Avoid a Voltage Drop. Behavioral Scientist."
article_type: "commentary"
method: {design: "theory", approach: "analytical", evidence_level: "weak", preregistered: false}
gist: >
  Economist John List, drawing on his book The Voltage Effect, argues that interventions
  which work in small pilots often lose effectiveness ('voltage drop') when scaled, and
  proposes five diagnostic checks a promising idea must pass: ruling out false positives via
  replication, checking representativeness of the target population, checking
  representativeness of the situational drivers of success, anticipating spillovers and
  general-equilibrium effects, and accounting for supply-side cost trajectories. For the SNH
  design problem it is a methodological caution against assuming a small pilot isolation- or
  burnout-intervention will generalize to a whole organization or community without first
  checking who it works for, why, and at what cost.
claims:
  - text: "A preschool curriculum with a parental-support component raised test scores more for Hispanic families than for white or Black families in the same population, traced to Hispanic households being more likely to be multigenerational, giving children access to grandparents who could help with learning when parents were unavailable."
    evidence: "case-study"
    support_strength: "low"
    outcomes: ["performance"]
    predictors: ["social-support", "sampling-method"]
  - text: "Children who were not enrolled in the preschool program nonetheless showed significantly better developmental outcomes, an unintended positive spillover the author attributes to peer play with enrolled children."
    evidence: "case-study"
    support_strength: "low"
    outcomes: ["performance"]
    predictors: ["network-structure", "peer-mentoring"]
  - text: "At Uber, raising driver pay through tipping or higher rate cards triggered supply-side adjustments (existing drivers worked more hours, new drivers entered the market), producing a new equilibrium in which average driver wages did not change even though the per-driver rate had increased."
    evidence: "case-study"
    support_strength: "low"
    outcomes: ["retention"]
    predictors: ["workload", "intervention"]
population:
  who: "No formal study population; the piece uses illustrative examples drawn from the author's own field-experiment research (an early-childhood education curriculum piloted in a Chicago suburb / Chicago Heights) and his tenure as chief economist at Uber."
  where: ["United States"]
  when: null
  n: null
  sector: ["education", "gig-economy"]
  sample_notes: >
    Anecdotal essay adapted from a trade book; no sample sizes, methods, or statistics are
    reported for the underlying studies referenced, and no citations are given for
    independent verification.
limitation:
  primary: "This is an opinion/summary essay adapted from the author's popular-science book; it presents illustrative anecdotes about scaling interventions rather than reporting methods, samples, or statistical results for the studies it references."
  others:
    - "No citations to the underlying studies are provided, precluding verification of the specific numeric claims."
    - "Examples are drawn selectively from the author's own research and consulting work, raising risk of favorable/selective reporting."
    - "The framework (five 'vital signs') is presented as a general heuristic, not validated against a systematic sample of scaling attempts."
risk_of_bias: "high"
relevance_to_project: >
  Provides a scaling-diagnostics heuristic (replicate before rolling out, check who and
  where an effect holds, anticipate peer spillovers and market-level equilibrium
  adjustments, and budget for cost trajectories) that is directly applicable to piloting SNH
  interventions such as isolation, loneliness, or burnout programs before deploying them
  across a whole remote-work organization or open-source community.
tags:
  topic: ["methodology", "measurement", "intervention"]
  method: ["theory", "case-study"]
  population: ["general-population"]
source:
  markdown: "Papers_Data/Mental Health/MD/The Five Vital Signs of a Scalable Idea and How to Avoid a Voltage Drop/The Five Vital Signs of a Scalable Idea and How to Avoid a Voltage Drop.md"
  pdf: "papers/Mental Health/The Five Vital Signs of a Scalable Idea and How to Avoid a Voltage Drop.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "swinburn-2011-the-global-obesity-pandemic-shaped-by"
title: "The global obesity pandemic: shaped by global drivers and local environments"
authors:
  - "Swinburn, Boyd A"
  - "Sacks, Gary"
  - "Hall, Kevin D"
  - "McPherson, Klim"
  - "Finegood, Diane T"
  - "Moodie, Marjory L"
  - "Gortmaker, Steven L"
year: 2011
doi: "10.1016/s0140-6736(11)60813-1"
venue: {type: "journal", name: "The Lancet", volume: 378, issue: 9793, pages: "804-814"}
citation: "Swinburn et al. (2011). The global obesity pandemic: shaped by global drivers and local environments. The Lancet, 378(9793), 804-814. https://doi.org/10.1016/s0140-6736(11)60813-1"
article_type: "review"
method: {design: "review-scoping", approach: "secondary-data", evidence_level: "moderate", preregistered: false}
gist: >
  This Lancet Series opener argues that the near-simultaneous global rise in obesity since
  the 1970s-80s is driven mainly by changes in the global food system (cheaper, more
  processed, more heavily marketed, more accessible food) producing passive overconsumption,
  while local environmental and individual factors (transport systems, food culture, body-
  size norms, genetics) explain the wide variation in obesity prevalence between and within
  populations. The authors propose a systemic drivers-versus-environmental-moderators
  framework and argue no country has ever reversed its obesity epidemic through public
  health measures alone, making policy action on the food supply side (not individual
  behavior change) the priority. It is a narrative synthesis and conceptual framework paper
  rather than a primary data study.
claims:
  - text: "Increases in food energy supply were more than sufficient to explain the rise in obesity in the USA since the 1970s and most of the weight increase in the UK since the 1980s, based on food-supply and energy-balance modelling studies."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["obesity"]
    predictors: ["food-environment"]
  - text: "Obesity prevalence patterns differ predictably by national income: in low- and middle-income countries obesity first appears among wealthy, urban, middle-aged adults (especially women) and later shifts to lower socioeconomic and rural groups as GDP rises, whereas in high-income countries it affects both sexes and all ages but is disproportionately concentrated in disadvantaged groups."
    evidence: "review-scoping"
    support_strength: "moderate"
    outcomes: ["obesity", "health-inequality"]
    predictors: ["socioeconomic-status", "urbanization"]
  - text: "Unlike tobacco use, injuries, and infectious disease, no country has yet served as a public-health exemplar in reversing its obesity epidemic, and independent of overall national wealth, higher income inequality is associated with higher obesity prevalence."
    evidence: "review-scoping"
    support_strength: "low-to-moderate"
    outcomes: ["obesity", "health-inequality"]
    predictors: ["organizational-culture", "network-structure"]
population:
  who: "Global adult and child populations across income levels; synthesis of international BMI surveillance data, national surveys, and published epidemiological/modelling studies (not a primary sampled cohort)"
  where: ["Global", "multiple high-, middle-, and low-income countries (USA, UK, Brazil, China, Australia, Pacific Islands, etc.)"]
  when: "Data and estimates primarily from 1970s-2011; obesity estimates as of 2008"
  n: null
  sector: ["public-health", "policy"]
  sample_notes: >
    Narrative synthesis drawing on secondary epidemiological data sources (WHO,
    IASO/International Obesity Taskforce, national surveys) and prior modelling papers
    rather than a defined study sample; authors note data representativeness is limited by
    absence of comparable, regularly repeated national surveys in many countries.
limitation:
  primary: "This is a narrative (non-systematic) review and conceptual framework paper, not a study with its own primary data collection, so causal claims about drivers rest on synthesis of heterogeneous prior studies rather than controlled analysis."
  others:
    - "The proposed obesogenic-drivers framework and 'energy balance flipping point' hypothesis are explicitly described by the authors as simplified and needing further testing beyond US food-supply data."
    - "Global monitoring systems for population weight/nutrition are described by the authors themselves as inadequate in almost all countries, limiting the precision of the prevalence trends discussed."
risk_of_bias: "medium"
relevance_to_project: >
  This paper is about obesity, not social connection, but its core analytic move -
  distinguishing distal systemic/environmental 'drivers' from local moderating conditions,
  and arguing that individual-behavior-change programs cannot reverse a population-level
  epidemic without addressing upstream systemic drivers - is a useful structural analogy for
  SNH's own prevention framing: it supports treating remote-work isolation or maintainer
  burnout as products of systemic (e.g. organizational, platform, economic) drivers
  requiring environment-level intervention rather than purely individual coping strategies.
tags:
  topic: ["community-health", "methodology"]
  method: ["review-scoping"]
  population: ["global-population"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/The Global Obesity Pandemic Shaped by Global Drivers and Local Environments/The Global Obesity Pandemic Shaped by Global Drivers and Local Environments.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/The Global Obesity Pandemic Shaped by Global Drivers and Local Environments.pdf"
  notes: null

---

id: "wilcox-2008-the-impact-of-two-universal-randomized"
title: "The impact of two universal randomized first- and second-grade classroom interventions on young adult suicide ideation and attempts"
authors:
  - "Wilcox, Holly C."
  - "Kellam, Sheppard G."
  - "Brown, C. Hendricks"
  - "Poduska, Jeanne M."
  - "Ialongo, Nicholas S."
  - "Wang, Wei"
  - "Anthony, James C."
year: 2008
doi: "10.1016/j.drugalcdep.2008.01.005"
venue: {type: "journal", name: "Drug and Alcohol Dependence", volume: 95, issue: null, pages: "S60-S73"}
citation: "Wilcox et al. (2008). The impact of two universal randomized first- and second-grade classroom interventions on young adult suicide ideation and attempts. Drug and Alcohol Dependence, 95, S60-S73. https://doi.org/10.1016/j.drugalcdep.2008.01.005"
article_type: "empirical"
method: {design: "rct", approach: "experiment", evidence_level: "moderate", preregistered: false}
gist: >
  This paper reports a school- and classroom-randomized trial testing whether two first- and
  second-grade classroom interventions -- the Good Behavior Game (GBG, a behavior-management
  strategy) and Mastery Learning (ML, a reading-achievement strategy) -- reduce suicide
  ideation and suicide attempts assessed 15+ years later in young adulthood. In Cohort 1
  (Baltimore City schools, first graders in 1985-86), GBG assignment was associated with
  roughly half the risk of suicide ideation and suicide attempt compared to controls, robust
  across covariate-adjusted models, while ML showed no significant effect on either outcome.
  The GBG's protective effect was substantially weaker and non-significant in a replication
  cohort (1986-87) implemented with less teacher mentoring and monitoring, suggesting the
  intervention must be delivered with fidelity to work.
claims:
  - text: "In Cohort 1, participants assigned to GBG classrooms were about half as likely to have experienced suicide ideation by young adulthood as controls (RR = 0.5, p = 0.024 unadjusted; adjusted RR = 0.4-0.5 across covariate models, best-fitting model RR = 0.5, 95% CI 0.2-0.9, p = 0.015); ML showed no significant effect on ideation (p = 0.211)."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation", "mental-health"]
    predictors: ["intervention", "sense-of-belonging"]
  - text: "GBG assignment was also associated with roughly half the risk of suicide attempt in Cohort 1 (overall summary RR = 0.5, 95% CI 0.3-0.9, p = 0.041), though the association lost statistical significance in some covariate-adjusted models (Model 3 RR = 0.6, p = 0.130); ML showed no significant impact on attempts."
    evidence: "rct"
    support_strength: "low-to-moderate"
    outcomes: ["suicidal-ideation", "mental-health"]
    predictors: ["intervention"]
  - text: "The GBG's protective effect on suicidality was greatly attenuated and non-significant in the Cohort 2 replication (SI: GBG 9% vs. control 12%, RR = 0.8, p = 0.408; SA: RR = 1.0, p = 0.965), attributed to reduced teacher mentoring/monitoring during implementation; caregiver suicide ideation/mental illness was a consistent, strong predictor of offspring suicidality across both cohorts (e.g., RR = 4.3, 95% CI 2.5-7.2, p < 0.001)."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation"]
    predictors: ["intervention", "social-support"]
population:
  who: "Two cohorts of first-grade children entering 19 elementary schools (41 classrooms) in the Baltimore City Public School System (Cohort 1: 1985-86 entry, n=1196 enrolled, 858 assessed in young adulthood; Cohort 2: 1986-87 entry, 837 assessed), followed up as young adults (mean age ~21-22) 15+ years later."
  where: ["United States"]
  when: "1985-2002 (baseline 1985-1987; young adult follow-up interviews 1999-2002)"
  n: 1918
  sector: ["education", "public-health"]
  sample_notes: >
    Cohort 1: 66% African-American, remainder mostly non-Hispanic White; classrooms
    randomized within schools with balancing on gender/kindergarten experience/behavior. 83%
    of the original sample was reassessed as young adults (including 154 in incarceration
    facilities); ~10% could not be traced or refused; 1.8% had died. Cohort 2 was
    implemented with less fidelity (less teacher mentoring/monitoring), limiting direct
    comparability to Cohort 1.
limitation:
  primary: "Findings are specific to this population/time period and setting (low-income, majority African-American urban school district); generalizability requires replication, and the protective GBG effect was not replicated in a same-district second cohort implemented with less fidelity."
  others:
    - "Suicidality outcomes relied on retrospective self-report of a single yes/no item each for lifetime ideation and attempt, collected once in young adulthood, with no independent verification."
    - "Caregiver mental illness/suicidality covariates were collected retrospectively from the youths themselves, raising possible mis-specification/bias in adjusted models."
    - "Mediation analyses (substance use, conduct problems, academic self-competence, peer deviance, etc.) found no evidence that any tested variable mediated the GBG effect, leaving the causal mechanism unresolved."
risk_of_bias: "low"
relevance_to_project: >
  Provides a rare randomized, decades-long causal evidence chain from an early classroom-
  level social/behavioral intervention (norm-setting, team-based peer accountability) to
  reduced suicidality in adulthood, directly supporting the SNH project's interest in
  upstream, structural interventions (versus individual-level fixes) for
  loneliness/isolation-adjacent mental health outcomes; the fidelity-dependence finding
  (strong Cohort 1 effect, weak Cohort 2 replication without mentoring/monitoring) is a
  caution for any SNH intervention design that its impact depends on rigorous implementation
  support, not just the intervention's existence.
tags:
  topic: ["mental-health", "suicide-prevention", "community-health"]
  method: ["rct", "longitudinal"]
  population: ["children", "young-adults"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/The Impact of Two Universal Randomized First and Second Grade Classroom Interventions on Young Adult Suicide Ideation and Attempts/The Impact of Two Universal Randomized First and Second Grade Classroom Interventions on Young Adult Suicide Ideation and Attempts.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/The Impact of Two Universal Randomized First and Second Grade Classroom Interventions on Young Adult Suicide Ideation and Attempts.pdf"
  notes: null

---

id: "van-2010-the-interpersonal-theory-of-suicide"
title: "The interpersonal theory of suicide."
authors:
  - "Van Orden, Kimberly A."
  - "Witte, Tracy K."
  - "Cukrowicz, Kelly C."
  - "Braithwaite, Scott R."
  - "Selby, Edward A."
  - "Joiner, Thomas E."
year: 2010
doi: "10.1037/a0018697"
venue: {type: "journal", name: "Psychological Review", volume: 117, issue: 2, pages: "575-600"}
citation: "Van Orden et al. (2010). The interpersonal theory of suicide.. Psychological Review, 117(2), 575-600. https://doi.org/10.1037/a0018697"
article_type: "theory"
method: {design: "theory", approach: "analytical", evidence_level: "low-to-moderate", preregistered: false}
gist: >
  Van Orden, Witte, Cukrowicz, Braithwaite, Selby, and Joiner propose the interpersonal
  theory of suicide: the most lethal suicidal desire arises from the simultaneous,
  perceived-as-permanent presence of thwarted belongingness and perceived burdensomeness,
  while the capability to act on that desire is acquired separately through habituation to
  pain and fear from repeated painful or provocative experiences (e.g., prior attempts,
  self-harm, combat exposure). The paper reorganizes decades of suicide risk-factor findings
  (social isolation, family conflict, unemployment, physical illness, prior attempts) as
  observable indicators of these three latent constructs and states four falsifiable
  hypotheses linking them to passive ideation, active desire, intent, and lethal/near-lethal
  attempts. It cites the authors' own interaction studies showing suicidal desire and
  attempts are best predicted by the joint presence of thwarted belongingness and
  burdensomeness (plus hopelessness), and by their combination with acquired capability,
  rather than by any single risk factor.
claims:
  - text: "Social isolation (few social supports, living alone, loneliness, loss of a spouse) is described as among the strongest and most reliable predictors of suicidal ideation, attempts, and death across age, nationality, and clinical severity, with dozens of empirical studies (catalogued in the paper's risk-factor table) supporting the association."
    evidence: "review-narrative"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation"]
    predictors: ["isolation", "loneliness", "social-support"]
  - text: "In two of the authors' own studies (undergraduates and an ethnically diverse community sample of young adults), the most severe suicidal ideation occurred specifically among people scoring high on BOTH thwarted belongingness and perceived burdensomeness simultaneously, not among those elevated on only one construct, with effects holding above and beyond depression, age, and gender."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["suicidal-ideation"]
    predictors: ["sense-of-belonging", "perceived-burdensomeness", "hopelessness"]
  - text: "Among young adults in an acute suicidal crisis, a three-way interaction of thwarted belongingness, perceived burdensomeness, and acquired capability (indexed by number of past suicide attempts) predicted whether the current crisis involved an actual attempt versus ideation alone, controlling for depression, hopelessness, and borderline personality disorder features."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["suicide-attempt"]
    predictors: ["sense-of-belonging", "perceived-burdensomeness", "acquired-capability"]
population:
  who: "Not a primary data-collection study: a theoretical synthesis of the suicide risk-factor literature, illustrated with supporting evidence from the authors' own prior studies (e.g., undergraduates, methadone-maintenance patients, psychiatric outpatients, and community samples of young adults in suicidal crisis)."
  where: ["United States"]
  when: null
  n: null
  sector: []
  sample_notes: >
    No new sample was collected; the paper synthesizes dozens of cited risk-factor studies
    (Table 1) plus several of the authors' own hypothesis-testing studies, mostly cross-
    sectional, clinical, or undergraduate convenience samples.
limitation:
  primary: "As a theory paper, it presents no new primary data on its central causal claims; supporting evidence for the theory's own hypotheses comes almost entirely from a small number of cross-sectional, correlational studies conducted by the authors' own research group, which cannot establish the proposed causal/temporal ordering."
  others:
    - "Key thresholds the theory relies on (e.g., 'complete' thwarted belongingness, 'global' perceived burdensomeness) are conceptually defined but not operationalized or tested at those extremes."
    - "The paper itself notes that a well-known related indicator, hopelessness (Beck Hopelessness Scale), has poor specificity (.42) despite high sensitivity (.80), meaning most people flagged as at-risk on this construct-adjacent measure do not go on to attempt suicide."
    - "Independent replication outside the authors' own lab is limited at the time of writing."
risk_of_bias: "medium"
relevance_to_project: >
  This is the foundational theory behind thwarted belongingness (loneliness + absence of
  reciprocally caring relationships) and perceived burdensomeness as measurable constructs;
  it gives the SNH project a validated conceptual and measurement framework (e.g., the
  Interpersonal Needs Questionnaire) for distinguishing 'feeling disconnected' from 'feeling
  like a burden' when assessing isolation risk in remote workers or community members,
  rather than treating isolation as a single undifferentiated construct.
tags:
  topic: ["suicide-prevention", "isolation", "loneliness", "mental-health", "social-support", "measurement"]
  method: ["theory", "narrative-review"]
  population: ["clinical-sample", "community-sample", "adults"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/The Interpersonal Theory of Suicide/The Interpersonal Theory of Suicide.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/The Interpersonal Theory of Suicide.pdf"
  notes: null

---

id: "bastien-2001-validation-of-the-insomnia-severity-index"
title: "Validation of the Insomnia Severity Index as an outcome measure for insomnia research"
authors:
  - "Bastien, C"
year: 2001
doi: "10.1016/s1389-9457(00)00065-4"
venue: {type: "journal", name: "Sleep Medicine", volume: 2, issue: 4, pages: "297-307"}
citation: "Bastien (2001). Validation of the Insomnia Severity Index as an outcome measure for insomnia research. Sleep Medicine, 2(4), 297-307. https://doi.org/10.1016/s1389-9457(00)00065-4"
article_type: "empirical"
method: {design: "psychometric-validation", approach: "survey", evidence_level: "moderate", preregistered: false}
gist: >
  Reports two validation studies of the Insomnia Severity Index (ISI), a 7-item self-report
  scale for insomnia severity. In a 145-patient sleep-clinic sample, the ISI showed adequate
  internal consistency (alpha = 0.74) and modest concurrent validity against sleep-diary
  measures. In a 78-patient RCT sample of older adults treated for late-life insomnia, the
  ISI detected large pre- to post-treatment change (patient version 15.4 to 8.9), converged
  with clinician and significant-other ratings, and yielded a stable three-factor structure
  (Impact, Severity, Satisfaction) explaining 72% of variance.
claims:
  - text: "In Study 1 (n=145 sleep-clinic patients), the ISI had internal consistency of alpha = 0.74 (item-total correlations 0.36-0.67) and correlated modestly with sleep-diary indices (SOL r=0.38, WASO r=0.35, EMA r=0.35, sleep efficiency r=-0.19, all p<0.01)."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["mental-health"]
    predictors: ["intervention"]
  - text: "In Study 2 (n=78 older insomnia patients in an RCT of CBT and pharmacotherapy), ISI total scores dropped from baseline to post-treatment on both patient (15.4 to 8.9) and clinician (17.7 to 7.7) versions, and gains were retained through 24-month follow-up, demonstrating sensitivity to treatment-related change."
    evidence: "rct"
    support_strength: "moderate"
    outcomes: ["mental-health"]
    predictors: ["intervention"]
  - text: "A principal component analysis (varimax rotation) yielded a stable three-factor structure -- Impact, Severity, and Satisfaction -- jointly explaining 72% of total variance, supporting the content validity of the scale's diagnostic coverage."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["mental-health"]
    predictors: []
population:
  who: "Study 1: 145 adult clinical patients presenting with insomnia at a sleep disorders centre (mean age 41.4). Study 2: 78 older adults (mean age 65) with primary insomnia enrolled in a randomized trial of cognitive-behavioral therapy vs. pharmacotherapy for late-life insomnia."
  where: ["Canada"]
  when: null
  n: 223
  sector: ["healthcare"]
  sample_notes: >
    Both samples are clinical/treatment-seeking populations recruited through a university
    sleep disorders centre in Quebec, not community or general-population samples; Study 2
    further restricted to older adults meeting strict DSM-III-R/ICSD primary-insomnia
    criteria, limiting generalizability.
limitation:
  primary: "Both validation samples are clinical/treatment-seeking patients at a single specialty sleep centre, so reliability/validity estimates may not generalize to community, workplace, or non-clinical insomnia populations."
  others:
    - "Correlations between the ISI and objective polysomnographic measures were often small (some non-significant at baseline), indicating the scale captures perceived rather than objectively measured sleep disturbance."
    - "The three-factor structure came from an exploratory factor analysis on a small item set (7 items), which the authors themselves caution should be interpreted cautiously."
risk_of_bias: "medium"
relevance_to_project: >
  Establishes the ISI as a brief, validated, easy-to-administer self-report instrument for
  insomnia severity and treatment-sensitive change, which is directly usable as a
  standardized sleep/wellbeing outcome measure in SNH studies examining how remote-work
  stress, burnout, or social isolation relate to sleep disruption.
tags:
  topic: ["mental-health", "wellbeing", "measurement"]
  method: ["survey"]
  population: ["clinical-sample"]
source:
  markdown: "Papers_Data/Mental Health/01 Mental Health - Extended/MD/Validation of the Insomnia Severity Index as an Outcome Measure for Insomnia Research/Validation of the Insomnia Severity Index as an Outcome Measure for Insomnia Research.md"
  pdf: "papers/Mental Health/01 Mental Health - Extended/Validation of the Insomnia Severity Index as an Outcome Measure for Insomnia Research.pdf"
  notes: null

---

id: "mcfillin-2023-why-mental-health-education-prevention-is"
title: "Why Mental Health Education & Prevention is Harmful"
authors:
  - "McFillin, Roger"
year: 2023
doi: null
venue: {type: "other", name: "Radically Genuine (Substack)", volume: null, issue: null, pages: null}
citation: "McFillin (2023). Why Mental Health Education & Prevention is Harmful. Radically Genuine (Substack)."
article_type: "commentary"
method: {design: "theory", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  A Substack opinion piece by a clinical psychologist arguing that school-based mental-
  health screening and psychoeducation programs are iatrogenic: they pathologize normal
  childhood struggles, propagate an unsupported 'chemical imbalance' narrative, and push
  overdiagnosis and unnecessary medication. It cites a single RCT-style comparison (WISE
  Teens, Australia) in which a social-emotional-skills program was associated with worse
  depression/anxiety outcomes than standard health classes as its central evidentiary
  anchor, and argues prevention should instead rest with families, community, and faith
  traditions rather than schools or clinicians.
claims:
  - text: "Citing a study of 1,071 Australian secondary-school students (2017-2018) published in Behaviour Research and Therapy, the piece reports that students in the WISE Teens social-emotional-skills program showed higher depression, increased anxiety, greater emotion-dysregulation difficulty, and more strained parent relationships than students in a standard health curriculum, with clinical-level depression in about 1 of 8 WISE Teens participants versus 1 of 13 controls."
    evidence: "rct"
    support_strength: "low-to-moderate"
    outcomes: ["depression", "anxiety", "mental-health"]
    predictors: ["intervention"]
  - text: "The author argues that psychiatric diagnoses (e.g., Major Depressive Disorder, ADHD) function as unvalidated labels rather than disease constructs, and that teaching children to frame ordinary struggles (loss, loneliness, financial hardship) in diagnostic terms increases self-stigmatization and hopelessness rather than clarifying their experience."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["mental-health", "wellbeing"]
    predictors: ["diagnostic-labeling"]
  - text: "The piece asserts that common adolescent depression-screening tools produce high false-positive rates, citing a claim that the TeenScreen program's creator acknowledged an 84% chance of wrongly flagging teens as suicide-risk, and estimating that an '80%-accurate' screening tool applied to roughly 74 million US children under 18 would falsely label millions."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["mental-health", "depression"]
    predictors: ["intervention"]
population:
  who: "General opinion commentary about US school-based mental-health screening and psychoeducation policy for children/adolescents, anchored by one cited controlled comparison of 1,071 Australian secondary-school students (2017-2018) in the WISE Teens program versus standard health class."
  where: ["United States", "Australia"]
  when: "2017-2018 (cited study); published 2023"
  n: null
  sector: ["education", "mental-health-policy"]
  sample_notes: >
    This is an opinion blog post with no original sample of its own; the only quantitative
    sample referenced is the cited WISE Teens trial (n=1,071 Australian teens, 2017-2018),
    described secondhand rather than independently analyzed. Statistics on TeenScreen and
    PHQ-9-A false-positive rates are asserted without citation and could not be verified in
    this corpus copy.
limitation:
  primary: "This is an ideologically framed advocacy blog post (Substack), not a systematic review or empirical study; it selectively cites a single study and uncited statistics to support a predetermined anti-medicalization, anti-screening thesis, including unrelated political claims (e.g., 'cultural Marxism')."
  others:
    - "Most factual assertions (PHQ-9 origin, TeenScreen false-positive rate, pharmaceutical-industry statistics) lack citations and are unverifiable in this corpus copy."
    - "The WISE Teens finding is summarized secondhand rather than critically appraised (e.g., no discussion of effect sizes, confidence intervals, or study limitations)."
    - "No systematic search or balancing of pro-screening evidence is presented; the piece is one-sided by design."
risk_of_bias: "high"
relevance_to_project: >
  Offers a skeptical counter-narrative to screening- and psychoeducation-based mental-health
  interventions that the SNH project should weigh when designing prevention or early-
  detection features: it flags a real cited finding (WISE Teens) suggesting school-based
  psychoeducation programs can sometimes worsen depression/anxiety, which is a useful
  cautionary data point even though the surrounding argument is largely opinion rather than
  evidence-based.
tags:
  topic: ["mental-health", "suicide-prevention", "wellbeing", "measurement"]
  method: ["theory"]
  population: ["adolescents", "school-based", "general-population"]
source:
  markdown: "Papers_Data/Mental Health/MD/Why Mental Health Education & Prevention is Harmful/Why Mental Health Education & Prevention is Harmful.md"
  pdf: "papers/Mental Health/Why Mental Health Education & Prevention is Harmful.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "mcdonald-2024-why-your-aces-score-doesn-t"
title: "Why Your ACEs Score Doesn't Mean As Much As You Might Think"
authors:
  - "McDonald, MaryCatherine"
year: 2024
doi: null
venue: {type: "other", name: "Psychology Today", volume: null, issue: null, pages: null}
citation: "McDonald (2024). Why Your ACEs Score Doesn't Mean As Much As You Might Think. Psychology Today."
article_type: "commentary"
method: {design: "theory", approach: "analytical", evidence_level: "speculative", preregistered: false}
gist: >
  A Psychology Today opinion piece by trauma researcher MaryCatherine McDonald argues that
  the widely used ACEs (Adverse Childhood Experiences) framework oversimplifies trauma by
  reducing it to a checklist of ten events collapsed into a single score, when whether an
  event becomes traumatic actually depends on an individual's nervous system and protective
  factors such as social support. The piece critiques the original 1998 Felitti et al. ACE
  study's demographic narrowness (71% white, middle-class sample) and its correlational
  design, and calls for a holistic, strengths-based, trauma-informed approach that also
  incorporates Positive Childhood Experiences (PCEs) research. For SNH it functions as a
  caution against over-relying on simple deficit-count instruments without accounting for
  individually variable buffering factors.
claims:
  - text: "The foundational ACE study (Felitti et al., 1998) sampled a predominantly white (71 percent) and middle-class population, which the author argues should raise questions about the framework's applicability to diverse cultural and socioeconomic contexts."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["mental-health"]
    predictors: ["sampling-method"]
  - text: "An events-based, ten-item checklist approach to defining trauma risks misclassification in both directions: it can overlook adversities outside the list, and it can mislabel events (e.g., parental divorce) as inherently traumatic even when protective factors like a robust social support network prevent lasting harm, because trauma response is determined by the individual nervous system, not the event itself."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["mental-health"]
    predictors: ["social-support"]
  - text: "Correlations between ACEs and negative health/social outcomes do not establish causation; resilience, social support systems, environmental factors, and access to resources all shape how individuals respond to adversity, and a 2019 Johns Hopkins study on Positive Childhood Experiences (Bethell et al.) found protective, mitigating effects present across ACE levels."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["mental-health", "wellbeing"]
    predictors: ["social-support", "intervention"]
population:
  who: "General readership; the piece's main empirical referent is the sample from the original Kaiser Permanente/CDC Adverse Childhood Experiences (ACE) study."
  where: ["United States"]
  when: "mid-1990s (original ACE study, as referenced)"
  n: null
  sector: ["general-population"]
  sample_notes: >
    No new sample was collected by this commentary. It references the original ACE study
    (Felitti et al., 1998; ~17,000 Kaiser Permanente HMO members, 71% white, middle-class)
    and briefly cites a 2019 Johns Hopkins Positive Childhood Experiences study (Bethell et
    al.) without describing that study's sample in detail.
limitation:
  primary: "This is a non-empirical opinion/commentary piece by a single author that reports no new data and no systematic review; its critiques of the ACEs literature and its alternative-framework recommendations are asserted rather than substantiated with a broad evidence base."
  others:
    - "Only two sources are cited in the references (Felitti et al. 1998 and Bethell et al. 2019), so the scope of literature underlying the critique is narrow."
    - "Published on a public-facing site (Psychology Today) without peer review."
risk_of_bias: "high"
relevance_to_project: >
  Directly relevant to how the SNH project should design and interpret risk-screening
  instruments: it warns against reducing complex psychosocial risk (e.g., isolation,
  burnout) to a single deficit-count score, and underscores that protective factors like
  social support can neutralize otherwise-adverse experiences, supporting a multi-factor
  rather than checklist approach to measurement.
tags:
  topic: ["mental-health", "measurement", "methodology", "wellbeing"]
  method: ["theory"]
  population: ["general-population"]
source:
  markdown: "Papers_Data/Mental Health/MD/Why Your ACEs Score Doesnt Mean As Much As You Might Think/Why Your ACEs Score Doesnt Mean As Much As You Might Think.md"
  pdf: "papers/Mental Health/Why Your ACEs Score Doesnt Mean As Much As You Might Think.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "world-2023-world-health-statistics-2023-monitoring-health"
title: "World Health Statistics 2023: Monitoring Health for the SDGs, Sustainable Development Goals"
authors:
  - "World Health Organization"
year: 2023
doi: null
venue: {type: "report", name: "World Health Organization", volume: null, issue: null, pages: null}
citation: "World Health Organization (2023). World Health Statistics 2023: Monitoring Health for the SDGs, Sustainable Development Goals. World Health Organization."
article_type: "review"
method: {design: "global-statistical-compendium", approach: "secondary-data", evidence_level: "reference", preregistered: false}
gist: >
  This is WHO's annual global health statistics report, compiling country-level indicators
  toward the health-related Sustainable Development Goals (SDGs) and WHO's 13th General
  Programme of Work. It covers mortality and disease trends (maternal/child mortality, NCDs,
  infectious disease, injuries and violence, environmental risks) and universal health
  coverage, with a dedicated section on suicide mortality trends and a briefer discussion of
  the global mental-disorder treatment gap. It is a reference compendium of population
  health statistics rather than a study of workplace or remote-work social dynamics.
claims:
  - text: "The global suicide mortality rate fell 29% between 2000 and 2019, from 13.0 to 9.2 deaths per 100,000 population; rates declined in all WHO regions except the Region of the Americas, where they rose 28%, while the European Region had both the largest decline (42%) and the highest 2019 rate (12.8 per 100,000)."
    evidence: "Global Health Estimates mortality data (2000-2019) compiled and reported by WHO"
    support_strength: "strong"
    outcomes: ["suicidal-ideation"]
    predictors: []
  - text: "Suicide accounted for 16% of all injury deaths globally in 2019 and more than 1 in 100 (1.3%) of all deaths; men and boys accounted for 69% of suicide deaths, and suicide was the third leading cause of death among girls and young women aged 15-29."
    evidence: "WHO Global Health Estimates injury and mortality data, 2019"
    support_strength: "strong"
    outcomes: ["suicidal-ideation"]
    predictors: []
  - text: "Only about one third of people with depression and 29% of people with psychosis globally receive formal mental health care, and mental, neurological and substance-use disorders accounted for 10% of the global disease burden (DALYs) and 25% of years lived with disability in 2019."
    evidence: "Cited secondary sources (WHO Mental Health Atlas 2020 and Global Burden of Disease 2019) synthesized in the report"
    support_strength: "moderate"
    outcomes: ["mental-health", "depression"]
    predictors: ["help-seeking"]
population:
  who: "Global population, all countries and WHO regions, disaggregated by sex and age group"
  where: ["Global"]
  when: "Primarily 2000-2021 (mortality/SDG indicator trends); some 2019 disease-burden estimates"
  n: null
  sector: ["public-health", "population-health"]
  sample_notes: >
    Country-reported vital registration and modelled estimates aggregated by WHO across all
    member states; not a primary study, no individual-level sample.
limitation:
  primary: "This is a statistical compendium synthesizing modelled national/regional estimates from many underlying sources, not primary research; individual estimates carry wide uncertainty intervals and depend on the quality of country reporting systems, which varies greatly especially in low- and middle-income countries."
  others:
    - "Contains almost nothing specific to remote work, workplace social dynamics, or online/community social network health, limiting direct relevance to the project beyond baseline mental-health/suicide epidemiology."
    - "Mental health and suicide content is a small fraction of a much larger report covering unrelated topics (maternal mortality, NCDs, infectious disease, climate change, health systems)."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Provides authoritative baseline global statistics on suicide mortality trends and the
  mental-health treatment gap that can contextualize (but not directly evidence) claims
  about isolation, loneliness, and mental health outcomes relevant to remote worker and
  community social-network health.
tags:
  topic: ["mental-health", "suicide-prevention"]
  method: ["secondary-data"]
  population: ["general-population"]
source:
  markdown: "Papers_Data/Mental Health/MD/World Health Statistics 2023/World Health Statistics 2023.md"
  pdf: "papers/Mental Health/World Health Statistics 2023.pdf"
  notes: "no-doi: confirmed none (manual review)"
