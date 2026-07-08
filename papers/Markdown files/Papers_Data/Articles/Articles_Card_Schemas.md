# Card Schemas - Articles

<!-- GENERATED FILE - do not edit. Source of truth is each paper's
     MD/<paper>/card_schema.md. Regenerate with:
     python3 tools/audit/build_combined_cards.py -->

id: "capra-2008-a-framework-for-evaluating-managerial-styles"
title: "A Framework for Evaluating Managerial Styles in Open Source Projects"
authors:
  - "Capra, Eugenio"
  - "Wasserman, Anthony I."
year: 2008
doi: "10.1007/978-0-387-09684-1_1"
venue: {type: "book", name: "IFIP – The International Federation for Information Processing", volume: null, issue: null, pages: "1-14"}
citation: "Capra et al. (2008). A Framework for Evaluating Managerial Styles in Open Source Projects. IFIP – The International Federation for Information Processing, 1-14. https://doi.org/10.1007/978-0-387-09684-1_1"
article_type: "empirical"
method: {design: "mixed-methods", approach: "interview", evidence_level: "low-to-moderate", preregistered: false}
gist: >
  The paper develops the Software Project Governance Framework (SPGF), which scores software
  projects along four dimensions -- contribution, project leadership, working practices, and
  testing -- to position them on a continuum from fully closed to fully open governance.
  Built from interviews with 25 project managers and validated against more than 70
  commercial and community open-source projects, the framework is illustrated with case
  studies of OpenOffice, MySQL, and SugarCRM showing how corporate-led open-source projects
  can still adopt fully distributed, virtual working practices. It contributes a structured
  way to characterize how geographically dispersed, community-governed teams organize
  communication, decision-making, and quality control.
claims:
  - text: "Across the validation sample of 70+ projects, working practices were the most 'open' dimension: 57% of projects scored the maximum (4) for being widely dispersed and communicating entirely through virtual tools with rare or no physical meetings, versus only 15% scoring maximum openness on testing."
    evidence: "mixed-methods"
    support_strength: "low-to-moderate"
    outcomes: ["collaboration", "communication"]
    predictors: ["network-structure", "organizational-culture"]
  - text: "MySQL, though centrally controlled by a company (scoring 1 on contribution and project leadership), scored 4 on working practices: developers were located in 26 countries, worked from home, met only once or twice a year, and coordinated asynchronously via IRC, shared task lists, and email to bridge time zones."
    evidence: "case-study"
    support_strength: "low"
    outcomes: ["collaboration", "communication"]
    predictors: ["remote-work-intensity", "organizational-culture"]
  - text: "Survey data across the sample showed roughly 50% of code in community open-source projects is developed by hired (paid) rather than volunteer developers, and physical face-to-face meetings occur in only about 35% of projects, indicating that most governance and coordination happens through virtual/asynchronous channels regardless of a project's formal openness."
    evidence: "mixed-methods"
    support_strength: "low-to-moderate"
    outcomes: ["collaboration"]
    predictors: ["remote-work-intensity", "network-structure"]
population:
  who: "Project managers, community managers, QA managers, VPs of engineering, committers, and project leaders from more than 70 commercial and community-based software projects (open and closed source), plus 25 project managers interviewed in the initial framework-development phase"
  where: []
  when: null
  n: 70
  sector: ["open-source-software", "software-industry"]
  sample_notes: >
    Convenience sample of mature, well-known projects drawn from SourceForge, Apache,
    Tigris, and Java.net meeting minimum size criteria (at least 2 administrators and 2
    contributors); explicitly skewed toward large, established projects rather than small
    teams, so findings may not generalize to nascent or small-scale open-source communities.
limitation:
  primary: "The framework is qualitative and ordinal by design (scores 1-4 per dimension), explicitly not intended for absolute cross-project comparison, and its dimension scores rest on the authors' interpretive judgment from interview data rather than independently verifiable metrics."
  others:
    - "Sample selection favored large, mature, well-known projects, introducing selection bias away from smaller or struggling open-source communities."
    - "Case studies (OpenOffice, MySQL, SugarCRM) are illustrative rather than representative, and scoring rationale relies on the authors' own coding of interview responses."
    - "No statistical testing or correlation analysis is reported between SPGF dimensions and outcomes like project success or code quality; the paper explicitly frames this as future work."
risk_of_bias: "medium"
relevance_to_project: >
  Provides an empirically grounded, four-dimension taxonomy (contribution, leadership,
  working practices, testing) for characterizing how distributed open-source teams organize
  communication and governance, useful for SNH work on measuring network structure and
  collaboration norms in maintainer/contributor communities. The finding that even
  corporate-controlled projects (e.g., MySQL) can be fully virtual and asynchronous is
  directly relevant to designing for remote, geographically dispersed collaboration without
  assuming volunteer-led governance.
tags:
  topic: ["open-source", "remote-work", "collaboration", "community-health", "methodology"]
  method: ["mixed-methods", "interview", "case-study"]
  population: ["open-source-contributors", "software-developers"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/A Framework for Evaluating Managerial Styles in Open Source Projects/A Framework for Evaluating Managerial Styles in Open Source Projects.md"
  pdf: "papers/Articles/01 Articles - Extended/A Framework for Evaluating Managerial Styles in Open Source Projects.pdf"
  notes: null

---

id: "mensching-2024-a-microcosm-of-the-interactions-in"
title: "A Microcosm of the Interactions in Open Source Projects"
authors:
  - "Mensching, Rob"
year: 2024
doi: null
venue: {type: "other", name: "robmensching.com", volume: null, issue: null, pages: null}
citation: "Mensching (2024). A Microcosm of the Interactions in Open Source Projects. robmensching.com."
article_type: "commentary"
method: {design: "case-study", approach: "analytical", evidence_level: "speculative", preregistered: false}
gist: >
  A blog post by an open-source maintainer that reconstructs and annotates the actual 2022
  mailing-list thread preceding the xz/liblzma backdoor, showing the original maintainer
  disclosing burnout and mental-health strain while community members pressed demands
  instead of offering help. The only participant who stepped in with practical assistance
  was the eventual attacker, who used that goodwill to accumulate maintainer trust. The
  piece argues this exchange is a representative 'microcosm' of how open-source projects
  treat solo maintainers as an inexhaustible, unsupported resource.
claims:
  - text: "The maintainer explicitly attributed his reduced activity to 'longterm mental health issues' and burnout ('my ability to care has been fairly limited'), disclosed directly on the public mailing list in response to pressure from users."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "mental-health"]
    predictors: ["isolation", "workload"]
  - text: "Across the thread, community members repeatedly demanded the maintainer hand off or accelerate transition of the project rather than offering to contribute code or maintenance help themselves, illustrating an absence of reciprocal social support."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["social-support", "isolation"]
    predictors: ["social-support", "community-engagement"]
  - text: "The only individual who offered concrete help during this period was 'Jia Tan,' later identified as the attacker who inserted the xz/liblzma backdoor; the offer of help itself was the mechanism by which the attacker acquired the trust and access needed to become a co-maintainer."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["collaboration"]
    predictors: ["peer-mentoring", "network-structure"]
population:
  who: "One open-source project maintainer (xz/liblzma) and the small set of mailing-list participants (including the eventual attacker) in a single 2022 email thread"
  where: []
  when: "2022 (email thread dates); blog post published March 2024"
  n: null
  sector: ["open-source"]
  sample_notes: >
    Single anecdotal case (N=1 thread), reconstructed from a publicly archived mailing-list
    thread; not a systematic sample and not generalizable by design.
limitation:
  primary: "This is a single anecdotal case study built from one archived email thread and the author's opinionated annotation, not a systematic or empirical analysis of open-source maintainer support patterns."
  others:
    - "Written with full hindsight knowledge of the xz backdoor attack, which likely shapes a retrospective narrative onto ambiguous exchanges."
    - "Relies entirely on a secondary source (an archived email thread) rather than direct interviews or investigation of participants' intentions."
    - "No comparison cases or baseline of 'typical' maintainer-community interactions are offered to support the claim that this thread is representative."
risk_of_bias: "high"
relevance_to_project: >
  Provides a vivid, real-world illustration of how untreated maintainer burnout and absent
  community social support can create both wellbeing harm and a concrete security failure
  mode, directly motivating SNH project interest in maintainer support/intervention
  mechanisms and early detection of isolation and burnout signals in open-source
  communities.
tags:
  topic: ["open-source", "maintainer-burnout", "isolation", "social-support", "community-health"]
  method: ["case-study"]
  population: ["open-source-maintainers", "online-community"]
source:
  markdown: "Papers_Data/Articles/MD/A Microcosm of the Interactions in Open Source Projects/A Microcosm of the Interactions in Open Source Projects.md"
  pdf: "papers/Articles/A Microcosm of the Interactions in Open Source Projects.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "mcdonald-2024-annual-intel-open-source-community-survey"
title: "Annual Intel Open Source Community Survey Results"
authors:
  - "McDonald, Nikki"
year: 2024
doi: null
venue: {type: "other", name: "Intel Open Ecosystem", volume: null, issue: null, pages: null}
citation: "McDonald (2024). Annual Intel Open Source Community Survey Results. Intel Open Ecosystem."
article_type: "empirical"
method: {design: "cross-sectional", approach: "survey", evidence_level: "weak", preregistered: false}
gist: >
  Reports results of Intel's second annual survey of 666 open source community members (Dec
  2023-Jan 2024), finding maintainer burnout as the top-cited challenge (45%), followed by
  documentation/onboarding (41%) and sustainability (37%). Also documents a decline in self-
  identified female respondents (15% to 7% year over year), continued strong engagement
  despite burnout (91% contributed vs 84% prior year), and growing interest in open source's
  role in AI innovation (82% rate it highly important). The piece is a corporate blog
  summary of survey findings rather than a peer-reviewed study, with no methodology detail
  on sampling or recruitment beyond an n and a date range.
claims:
  - text: "Maintainer burnout was the top-cited challenge among open source community survey respondents, selected by 45% (n=666), narrowly ahead of documentation/onboarding difficulties (41%) and sustainability concerns (37%)."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["burnout"]
    predictors: ["open-source-maintenance", "workload"]
  - text: "Self-identified female respondents dropped sharply year over year, from 15% to 7%, while male respondents made up 79% of the sample, underscoring a persistent and worsening gender diversity gap in open source participation."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["sense-of-belonging"]
    predictors: ["inclusiveness"]
  - text: "Despite widely reported burnout, contribution activity increased: 91% of respondents said they had contributed to open source projects in the past year versus 84% the previous year, with about 4 in 10 contributing at least weekly."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["job-engagement", "retention"]
    predictors: ["open-source-maintenance", "community-engagement"]
population:
  who: "666 self-selected respondents to Intel's annual open source community survey, majority male (79%), late 30s, one-third US-based and two-thirds international"
  where: ["United States", "international (unspecified)"]
  when: "December 2023-January 2024"
  n: 666
  sector: ["open-source", "technology"]
  sample_notes: >
    Self-selected survey audience reached via Intel's open source community channels; no
    sampling frame, response rate, or representativeness analysis reported; some sub-
    questions (e.g. conference attendance) had much smaller n (~200).
limitation:
  primary: "No methodological detail is given on sampling frame, recruitment channel, or response rate, so results likely reflect a self-selected, Intel-affiliated audience rather than the broader open source population."
  others:
    - "Corporate blog format with no statistical testing, confidence intervals, or comparison of subgroup differences beyond simple percentages."
    - "Written by Intel staff with an evident promotional interest in favorable framing of Intel's open source involvement."
    - "Year-over-year comparisons (e.g. gender shift, contribution rate) may reflect sample composition changes rather than true population trends."
risk_of_bias: "high"
relevance_to_project: >
  Provides a large-sample (though non-random) data point that maintainer burnout is the
  single most commonly cited top challenge among open source contributors, directly
  supporting the SNH project's focus on maintainer burnout as a target outcome, and flags a
  widening gender-diversity gap as a related community-health signal worth tracking.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "community-health"]
  method: ["survey", "cross-sectional"]
  population: ["open-source-maintainers", "software-developers"]
source:
  markdown: "Papers_Data/Articles/MD/Annual Intel Open Source Community Survey Results/Annual Intel Open Source Community Survey Results.md"
  pdf: "papers/Articles/Annual Intel Open Source Community Survey Results.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "guba-1981-criteria-for-assessing-the-trustworthiness-of"
title: "Criteria for assessing the trustworthiness of naturalistic inquiries"
authors:
  - "Guba, Egon G."
year: 1981
doi: "10.1007/bf02766777"
venue: {type: "journal", name: "ECTJ", volume: 29, issue: 2, pages: null}
citation: "Guba (1981). Criteria for assessing the trustworthiness of naturalistic inquiries. ECTJ, 29(2). https://doi.org/10.1007/bf02766777"
article_type: "methods"
method: {design: "theory", approach: "analytical", evidence_level: "reference", preregistered: false}
gist: >
  Guba argues that naturalistic (qualitative) inquiry needs its own criteria for judging
  trustworthiness rather than being held to the rationalistic paradigm's internal validity,
  external validity, reliability, and objectivity. He proposes four parallel naturalistic
  criteria -- credibility, transferability, dependability, and confirmability -- and lays
  out concrete techniques (prolonged engagement, triangulation, member checks, thick
  description, audit trails, and external dependability/confirmability audits) for
  establishing each. The paper became a foundational, widely cited reference for evaluating
  rigor in qualitative social-science research.
claims:
  - text: "Guba proposes that trustworthiness in naturalistic inquiry should be judged by four criteria that parallel but are distinct from rationalistic ones: credibility (analog of internal validity), transferability (analog of external validity/generalizability), dependability (analog of reliability), and confirmability (analog of objectivity)."
    evidence: "theory"
    support_strength: "moderate"
    outcomes: ["research-trustworthiness"]
    predictors: ["inquiry-paradigm"]
  - text: "The paper identifies triangulation and member checks as the 'sine qua non' minimum requirements for establishing credibility, alongside prolonged engagement at a site, persistent observation, peer debriefing, and collection of referential adequacy materials during the study."
    evidence: "theory"
    support_strength: "moderate"
    outcomes: ["research-trustworthiness"]
    predictors: ["triangulation", "peer-debriefing"]
  - text: "For dependability and confirmability, Guba recommends establishing an 'audit trail' during the study and, afterward, commissioning external dependability and confirmability audits (modeled on a financial audit) that examine the inquiry process and verify that every interpretation is supported by documented data."
    evidence: "theory"
    support_strength: "moderate"
    outcomes: ["research-trustworthiness"]
    predictors: ["audit-trail"]
population:
  who: "No empirical sample; this is a methodological/conceptual essay addressed to naturalistic (qualitative) inquiry researchers, journal editors, referees, and dissertation committees."
  where: []
  when: null
  n: null
  sector: []
  sample_notes: >
    This is a conceptual/methodological ERIC/ECTJ Annual Review Paper (1981), not an
    empirical study, so there is no sample, recruitment, or response rate. It draws on the
    author's (and Yvonna Lincoln's) prior and forthcoming work on naturalistic inquiry
    methodology.
limitation:
  primary: "The criteria are asserted rather than empirically validated -- the paper explicitly frames them as 'textbook answers' that only increase the probability of trustworthiness, and it offers no decision rules for how much triangulation, audit, or member-checking is sufficient."
  others:
    - "Reflects one author's (and Lincoln's) specific school of thought rather than a systematic review of competing qualitative rigor frameworks current at the time."
    - "Terminology and framing (e.g., 'naturalistic' vs. 'rationalistic' paradigm) are dated relative to how qualitative methodology is discussed in contemporary literature, though the four criteria themselves remain in wide use."
risk_of_bias: "not-applicable"
relevance_to_project: >
  SNH research on isolation, belonging, and burnout often relies on qualitative methods --
  interviews, case studies, ethnographic observation in remote/open-source communities --
  and this paper supplies the standard vocabulary (credibility, transferability,
  dependability, confirmability) and concrete techniques (triangulation, member checks,
  audit trails, thick description) the project should use to evaluate the rigor of
  qualitative SNH studies it cites or designs.
tags:
  topic: ["methodology", "measurement"]
  method: ["theory", "qualitative"]
  population: ["academic-researchers"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/Criteria for Assessing the Trustworthiness of Naturalistic Inquiries/Criteria for Assessing the Trustworthiness of Naturalistic Inquiries.md"
  pdf: "papers/Articles/01 Articles - Extended/Criteria for Assessing the Trustworthiness of Naturalistic Inquiries.pdf"
  notes: null

---

id: "oliver-2021-dealing-with-burnout-in-open-source"
title: "Dealing with burnout in open source"
authors:
  - "Oliver, Kiran"
year: 2021
doi: null
venue: {type: "other", name: "Opensource.com", volume: null, issue: null, pages: null}
citation: "Oliver (2021). Dealing with burnout in open source. Opensource.com."
article_type: "commentary"
method: {design: "theory", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  This opensource.com article by Kiran Oliver defines burnout and argues that it is
  widespread in tech (citing a survey figure of over 60% of industry professionals reporting
  burnout), then offers practical, experience-based advice for managers and individual
  contributors to prevent and respond to burnout in open source teams and communities. It
  emphasizes that neurodivergent contributors (autistic, ADHD, dyslexic, dyspraxic) may
  experience burnout differently and can be misread as slacking off, and it stresses privacy
  and compassion when someone discloses burnout.
claims:
  - text: "The author cites a 2020 industry survey finding that over 60% of tech industry professionals report having experienced burnout."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["burnout"]
    predictors: ["technostress"]
  - text: "In open source communities, burnout manifests behaviorally as not responding to pull requests, leaving issues open for extended periods, missing meetings or roadmap deadlines, and general forgetfulness, alongside emotional fatigue, anxiety, and stress."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "anxiety", "maintainer-burnout"]
    predictors: ["workload", "community-engagement"]
  - text: "Burnout in neurodivergent employees (e.g., autism, ADD/ADHD) can present as autistic burnout, which is described as often harder to recognize and can be misinterpreted by others as poor performance rather than as burnout."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "mental-health"]
    predictors: ["inclusiveness", "psychological-safety"]
population:
  who: "General audience of open source maintainers, contributors, and managers; no formal study sample, author draws on personal experience and a conference talk audience's shared experiences"
  where: []
  when: "2021"
  n: null
  sector: ["open-source", "technology"]
  sample_notes: >
    Opinion/advice blog post; not an empirical study. Anecdotal basis includes audience
    feedback from the author's 2021 Upstream/Tidelift Maintainer Week talk on burnout; no
    systematic data collection or sampling.
limitation:
  primary: "The piece is a short opinion/advice blog post with no original data collection, methodology, or citations to peer-reviewed research beyond one secondary survey statistic, so its claims are not empirically validated."
  others:
    - "Recommendations are generic best-practice suggestions (flexible time off, async meetings, automation) without evidence of effectiveness for preventing or reducing burnout."
    - "No definition of burnout is operationalized or measured; claims about autistic burnout are asserted without citation to primary research within the piece itself."
risk_of_bias: "high"
relevance_to_project: >
  Provides a practitioner-level, community-facing framing of maintainer/contributor burnout
  symptoms (unresponsiveness to PRs, missed deadlines, emotional fatigue) that the SNH
  project can use to identify observable behavioral proxies for burnout risk in open source
  communities, and flags neurodivergent-inclusive design as a consideration for any burnout-
  detection or support intervention.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "mental-health", "psychological-safety"]
  method: ["theory"]
  population: ["open-source-contributors"]
source:
  markdown: "Papers_Data/Articles/MD/Dealing with Burnout in Open Source/Dealing with Burnout in Open Source.md"
  pdf: "papers/Articles/Dealing with Burnout in Open Source.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "case-2022-developers-are-burned-out-quitting-their"
title: "Developers are burned out, quitting their jobs and creating a crisis for recruiters"
authors:
  - "Case, Tony"
year: 2022
doi: null
venue: {type: "other", name: "WorkLife (worklife.news)", volume: null, issue: null, pages: null}
citation: "Case (2022). Developers are burned out, quitting their jobs and creating a crisis for recruiters. WorkLife (worklife.news)."
article_type: "commentary"
method: {design: "theory", approach: "interview", evidence_level: "weak", preregistered: false}
gist: >
  This WorkLife.news trade article reports that software developers are burning out and
  leaving jobs in large numbers, citing two vendor survey reports (LaunchDarkly and EDB) and
  quoting five engineering executives on causes and fixes. The executives point to
  distributed-team communication breakdowns, expanded developer responsibilities (QA,
  security, license compliance), and lack of autonomy or onboarding support as drivers of
  burnout and attrition, and describe practices like asynchronous communication, deep-focus
  time blocks, and periodic in-person team bonding as mitigations.
claims:
  - text: "A LaunchDarkly report found that nearly 7 in 10 developers (67%) have left a job (or know someone who has) due to pressure around minimizing deployment errors, and 61% said their companies' cumbersome development processes are barriers to innovation."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["turnover", "burnout", "productivity"]
    predictors: ["workload", "organizational-culture", "technostress"]
  - text: "An EDB survey found that just under half (46%) of developers said they were very satisfied in their current roles, even as they continued to weigh other job options amid a possible recession."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["job-satisfaction", "turnover"]
    predictors: ["organizational-culture", "workload"]
  - text: "Engineering leaders interviewed attributed developer burnout in fully distributed teams primarily to poor intra-team communication and unclear vision/mission, and separately to insufficient structure and support for early- and mid-career hires, arguing this forces companies to over-hire scarce senior developers."
    evidence: "qualitative"
    support_strength: "speculative"
    outcomes: ["burnout", "turnover", "communication"]
    predictors: ["team-cohesion", "remote-work-intensity", "leadership-style", "autonomy"]
population:
  who: "Software developers and engineering leaders in the tech industry, as characterized in two vendor-commissioned surveys and quotes from five named engineering executives (Sonatype, ClickUp, Jobsity, Kong, Netlify)"
  where: ["USA"]
  when: "2022"
  n: null
  sector: ["tech", "open-source"]
  sample_notes: >
    This is a journalism piece, not a primary study: it summarizes findings from two
    external vendor surveys (LaunchDarkly report; EDB 'Open Source Talent Survey 2022')
    without giving their sample sizes, response rates, or methodology, and supplements them
    with opinion quotes from five engineering executives with no disclosed selection method.
limitation:
  primary: "Trade-journalism piece that reports secondhand statistics from two vendor-commissioned surveys without any methodological detail (sample size, response rate, instrument), so the cited percentages cannot be independently assessed for rigor."
  others:
    - "Causal claims about burnout drivers (remote/distributed communication, lack of autonomy) come from unstructured executive opinion quotes, not from any study design."
    - "Executives quoted have a commercial interest in promoting their own companies' tools or practices (e.g. async communication, deep-focus blocks), which is a source of bias."
risk_of_bias: "high"
relevance_to_project: >
  Captures practitioner-level framing of developer and open-source-maintainer burnout
  drivers -- distributed-team communication gaps, expanded on-call/security
  responsibilities, low autonomy, and weak onboarding support -- plus proposed mitigations
  (async communication, protected deep-focus time, periodic in-person bonding) that the SNH
  project can use as candidate intervention ideas to test against stronger evidence, not as
  evidence itself.
tags:
  topic: ["burnout", "remote-work", "open-source", "maintainer-burnout", "job-satisfaction"]
  method: ["qualitative", "cross-sectional"]
  population: ["software-developers", "tech", "open-source", "remote-workers"]
source:
  markdown: "Papers_Data/Articles/MD/Developers Are Burned Out Quitting Their Jobs and Creating a Crisis for Recruiters/Developers Are Burned Out Quitting Their Jobs and Creating a Crisis for Recruiters.md"
  pdf: "papers/Articles/Developers Are Burned Out Quitting Their Jobs and Creating a Crisis for Recruiters.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "crowston-2004-effective-work-practices-for-software-engineering"
title: "Effective Work Practices for Software Engineering: Free/Libre Open Source Software Development"
authors:
  - "Crowston, Kevin"
  - "Annabi, Hala"
  - "Howison, James"
  - "Masango, Chengetai"
year: 2004
doi: null
venue: {type: "conference", name: "WISER'04 Workshop on Interdisciplinary Software Engineering Research, Newport Beach, California (ACM)", volume: null, issue: null, pages: null}
citation: "Crowston et al. (2004). Effective Work Practices for Software Engineering: Free/Libre Open Source Software Development. WISER'04 Workshop on Interdisciplinary Software Engineering Research, Newport Beach, California (ACM)."
article_type: "theory"
method: {design: "theory", approach: "analytical", evidence_level: "speculative", preregistered: false}
gist: >
  This conference paper builds a theoretical model of FLOSS (Free/Libre Open Source
  Software) team effectiveness by extending Hackman's input-process-output model of work-
  team effectiveness with coordination theory (managing task/resource/actor dependencies)
  and Weick and Roberts' collective mind theory (contribution, representation,
  subordination). Drawing on the FLOSS and distributed-work literatures, the authors
  synthesize prior findings (e.g., the core/co-developer/active-user/passive-user 'onion'
  structure, effort penalties of distance) into a set of testable propositions and lay out a
  data-collection plan (mailing-list archives, CVS logs, interviews, observation) for future
  empirical work. It contributes a theoretical scaffold rather than new empirical results.
claims:
  - text: "FLOSS development teams are repeatedly described in the literature as having a hierarchical, onion-like structure: a small, highly interactive core of developers who write most of the code and control design, surrounded by a larger, more loosely coupled group of co-developers, then active users who report bugs/features, then passive users; core developers face a significant barrier to entry because they must have deep understanding of the software and its processes."
    evidence: "review-scoping"
    support_strength: "low"
    outcomes: ["collaboration"]
    predictors: ["network-structure", "community-engagement"]
  - text: "Distributed/FLOSS teams generally require more on-task effort to be effective than co-located teams because participants are distant and less familiar with each other's work, and this additional required effort has been linked in prior empirical studies (Herbsleb et al. 2001; Mockus et al. 2000) to delays in software release compared to traditional face-to-face teams."
    evidence: "review-scoping"
    support_strength: "low-to-moderate"
    outcomes: ["productivity", "collaboration"]
    predictors: ["remote-work-intensity", "workload"]
  - text: "FLOSS software quality and development speed are attributed in the reviewed literature to two mechanisms: developers being users of their own software (eliminating much requirements ambiguity) and open access to source code letting users become co-developers, which the literature credits with letting hundreds of contributors handle mundane work (e.g., testing, estimated to consume over 50% of cost in non-FLOSS projects) and fix bugs/evolve features quickly."
    evidence: "review-scoping"
    support_strength: "low"
    outcomes: ["productivity", "collaboration"]
    predictors: ["open-source-maintenance", "community-engagement"]
population:
  who: "Not a primary study of a sample; the paper synthesizes prior descriptive/case-study literature on FLOSS projects (e.g., Linux, Apache, Mozilla, GNOME) and proposes a future research design targeting FLOSS developers, teams, and project artifacts."
  where: []
  when: null
  n: null
  sector: ["open-source"]
  sample_notes: >
    No new empirical data was collected for this paper; it is a conceptual/propositional
    piece. The 'proposed data collection' section describes planned future sources (project
    demographics, mailing-list and bug-tracker archives, CVS logs, developer interviews,
    conference observation, virtual ethnography) that had not yet been executed or analyzed
    at time of writing.
limitation:
  primary: "The theoretical model and all of its propositions are untested at time of publication; the paper is a research proposal/framework, not a report of empirical findings, so none of its claims about team effectiveness have been validated against data."
  others:
    - "Much of the underlying FLOSS literature it synthesizes is written by developers/consultants with partisan or promotional interests, and well-documented case studies are scarce and skew toward reporting successes rather than failures."
    - "The widely-cited 'onion' team-structure model it relies on is based on only a few case studies and, as the authors themselves note, 'has not been extensively tested.'"
risk_of_bias: "not-applicable"
relevance_to_project: >
  Offers the SNH project a ready-made theoretical scaffold — core/co-developer/active-
  user/passive-user structure, coordination-theory dependency management, and collective-
  mind (contribution/representation/subordination) constructs — for operationalizing
  community engagement, participation-role structure, and coordination mechanisms as
  predictors of collaboration and burnout in open-source and remote-team settings, and for
  designing the kind of trace-data-plus-interview measurement plan (mailing lists, commit
  logs, interviews) the project itself would need.
tags:
  topic: ["open-source", "collaboration", "community-health", "methodology"]
  method: ["theory"]
  population: ["open-source-developers", "distributed-teams"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/Effective Work Practices for Software Engineering Free Libre Open Source Software Development/Effective Work Practices for Software Engineering Free Libre Open Source Software Development.md"
  pdf: "papers/Articles/01 Articles - Extended/Effective Work Practices for Software Engineering Free Libre Open Source Software Development.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "anon-2021-how-i-recognize-and-prevent-burnout"
title: "How I Recognize And Prevent Burnout In Open Source"
authors:
year: 2021
doi: null
venue: {type: "other", name: "Opensource.com (republished by aster.cloud)", volume: null, issue: null, pages: null}
citation: "Opensource.com (republished by aster.cloud) (2021). How I Recognize And Prevent Burnout In Open Source. Opensource.com (republished by aster.cloud)."
article_type: "commentary"
method: {design: "case-study", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  A first-person practitioner essay in which the author describes his own early-warning
  signs of burnout—dreading everyday tasks, withdrawing from social contact at work and at
  home, and becoming irritable with family and friends—and the small preventive habits he
  uses to counter it, such as mantras for presence, short social breaks, brief daily
  exercise, and disciplined boundary-setting around vacation and family time. It closes by
  urging readers, especially in remote work settings, to check on colleagues who seem
  overwhelmed rather than let them suffer burnout alone.
claims:
  - text: "The author identifies social withdrawal—avoiding contact with others in both work and non-work settings—and increased snappishness or conflict with family and friends as his own personal early-warning signs that burnout is approaching."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "isolation"]
    predictors: ["isolation", "workload"]
  - text: "He reports that regular small preventive practices—social lunches with friends/former colleagues, five to ten minutes of daily exercise, refocusing mantras, and explicit boundary-setting around vacation and family time—help him avoid reaching a burnout state, a practice he notes became harder to sustain once the pandemic disrupted in-person social breaks."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "work-life-balance"]
    predictors: ["boundary-management", "social-support"]
  - text: "The essay argues burnout has social spillover: when one person suffers, it affects the people around them, so coworkers should proactively check in on and follow up with overwhelmed colleagues, or alert their manager, rather than leaving them to cope alone—particularly in remote work environments."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "wellbeing"]
    predictors: ["social-support", "peer-mentoring"]
population:
  who: "The author's own first-person experience; intended audience is open-source contributors and remote/tech workers generally, not a studied sample."
  where: []
  when: "2021"
  n: null
  sector: ["open-source"]
  sample_notes: >
    Purely anecdotal single-author narrative; no participants, sampling, or data
    collection—this is a personal reflective essay, not a study.
limitation:
  primary: "Entirely anecdotal, first-person opinion piece with no systematic data, sample, or evidence beyond the author's own recollected experience."
  others:
    - "No citation of research literature; the recommended strategies are personal habits rather than tested interventions."
    - "This conversion appears to be missing its opening section (replaced by extracted images), so some introductory context is unavailable."
risk_of_bias: "not-applicable"
relevance_to_project: >
  Provides a practitioner-level account of self-recognized burnout warning signs (social
  withdrawal, friction with family/friends) and lightweight prevention tactics (short
  breaks, exercise, boundary-setting) that can inform design of maintainer/remote-worker
  burnout early-warning prompts and peer check-in features, and reinforces the project's
  emphasis on proactive social support in remote settings.
tags:
  topic: ["burnout", "open-source", "remote-work", "wellbeing", "work-life-balance"]
  method: ["case-study"]
  population: ["open-source-contributors", "remote-workers"]
source:
  markdown: "Papers_Data/Articles/MD/How I Recognize And Prevent Burnout In Open Source/How I Recognize And Prevent Burnout In Open Source.md"
  pdf: "papers/Articles/How I Recognize And Prevent Burnout In Open Source.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "finley-2021-how-open-source-maintainers-keep-contributorsand"
title: "How open source maintainers keep contributors—and themselves—happy"
authors:
  - "Finley, Klint"
year: 2021
doi: null
venue: {type: "other", name: "The ReadME Project (GitHub)", volume: null, issue: null, pages: null}
citation: "Finley (2021). How open source maintainers keep contributors—and themselves—happy. The ReadME Project (GitHub)."
article_type: "commentary"
method: {design: "case-study", approach: "other", evidence_level: "weak", preregistered: false}
gist: >
  This GitHub ReadME Project article reports practitioner advice from talks at the 2021
  Global Maintainer Summit on sustaining open-source contributor communities. Maintainers
  from projects like Kubernetes, Rust, Python, Homebrew, Prometheus, Home Assistant, and
  NgRX describe practices for attracting and retaining contributors: staying visibly active,
  responding quickly, offering recognition and escalating responsibility, automating triage
  (linters, bots, stale-issue closers), setting clear project scope, and saying no to
  proposals kindly and promptly. It frames contributor-relations work as central to
  maintainer sustainability and burnout prevention, arguing that scaling community
  management, not just code, is the key challenge facing popular projects.
claims:
  - text: "Multiple maintainers (Kubernetes' Brendan Burns, Tern's Rose Judge) emphasized that slow response times to issues and pull requests discourage future participation from both new and existing contributors."
    evidence: "case-study"
    support_strength: "weak"
    outcomes: ["community-engagement", "retention"]
    predictors: ["leadership-style", "organizational-culture"]
  - text: "Automation of contribution triage (linters, auto-formatters, and custom bots such as Python's 'Bedevere' and 'Miss-islington') reduced maintainer workload and interpersonal friction, e.g. Homebrew's shift to automated code review eliminated maintainers being 'accused of being pedantic' over style disputes."
    evidence: "case-study"
    support_strength: "weak"
    outcomes: ["burnout", "collaboration"]
    predictors: ["workload", "open-source-maintenance"]
  - text: "Maintainers reported that avoiding scope creep and defining a clear project vision (e.g. NgRX's design documents) made it easier to decline contributions without guilt, and that framing rejections as directed at the proposal rather than the person preserved contributor goodwill."
    evidence: "case-study"
    support_strength: "weak"
    outcomes: ["burnout", "collaboration", "retention"]
    predictors: ["leadership-style", "boundary-management"]
population:
  who: "Maintainers and community leads of prominent open-source projects (Kubernetes, Rust, Python, Homebrew, Prometheus, Home Assistant, NgRX, Tern, FOSSASIA) speaking at GitHub's Global Maintainer Summit, June 8-9 2021"
  where: ["Global (open-source community, virtual/GitHub-hosted summit)"]
  when: "2021"
  n: null
  sector: ["open-source"]
  sample_notes: >
    Not a study; a journalistic summary of conference talks by a small, self-selected set of
    prominent maintainers. No systematic sampling, no quantitative data on how
    representative these practices are of maintainers broadly.
limitation:
  primary: "This is journalism synthesizing anecdotal advice from conference speakers, not original research; no data collection, sample, or empirical test of which practices actually improve contributor retention or maintainer wellbeing."
  others:
    - "Advice is drawn from a handful of high-profile, well-resourced projects (Kubernetes, Rust, Python) and may not generalize to smaller or resource-poor projects."
    - "The markdown conversion has severe character corruption (missing letters throughout, e.g. 'th' for 'the'), degrading readability though the substantive content remains inferable."
risk_of_bias: "high"
relevance_to_project: >
  Provides practitioner-level, ground-truth vocabulary and candidate mechanisms (response
  latency, automation of triage, scope-setting, rejection framing) linking maintainer
  burnout and contributor retention in open-source communities -- useful as a source of
  hypotheses to test empirically and as evidence that maintainer burden and 'saying no' are
  recognized, felt problems in the community the SNH project targets.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "community-health"]
  method: ["case-study"]
  population: ["open-source"]
source:
  markdown: "Papers_Data/Articles/MD/How Open Source Maintainers Keep Contributors and Themselves Happy/How Open Source Maintainers Keep Contributors and Themselves Happy.md"
  pdf: "papers/Articles/How Open Source Maintainers Keep Contributors and Themselves Happy.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "overney-2020-how-to-not-get-rich-an"
title: "How to Not Get Rich: An Empirical Study of Donations in Open Source"
authors:
  - "Overney, Cassandra"
  - "Meinicke, Jens"
  - "Kästner, Christian"
  - "Vasilescu, Bogdan"
year: 2020
doi: null
venue: {type: "conference", name: "Proceedings of the 42nd International Conference on Software Engineering (ICSE '20)", volume: null, issue: null, pages: null}
citation: "Overney et al. (2020). How to Not Get Rich: An Empirical Study of Donations in Open Source. Proceedings of the 42nd International Conference on Software Engineering (ICSE '20)."
article_type: "empirical"
method: {design: "mixed-methods", approach: "secondary-data", evidence_level: "moderate", preregistered: false}
gist: >
  This mixed-methods study mines GitHub and npm repositories to characterize the emerging
  phenomenon of open-source donations: how many projects ask for them, which platforms they
  use, what characteristics predict asking for and receiving funds, why developers say they
  want the money, and whether donations actually move the needle on project activity. It
  finds donation requests are rare (well under 1% of repositories), donations are often
  framed by maintainers as a last-ditch appeal tied to unsustainable workload, and receiving
  donations shows little to no measurable association with subsequent engineering activity,
  while projects that ask but fail to receive funding tend to decline further.
claims:
  - text: "25,885 of 77,934,441 GitHub repositories (0.04%) and 1,145 of 537,640 npm packages (0.2%) explicitly requested donations as of May 23, 2019, most commonly via PayPal and Patreon, with adoption rising steadily since about 2012."
    evidence: "cross-sectional"
    support_strength: "strong"
    outcomes: ["open-source-funding"]
    predictors: ["open-source-maintenance"]
  - text: "In qualitative analysis of 109 donation-request texts, 48% cited engineering activities (including paying a developer's salary) as the funding goal, with some maintainers explicitly framing appeals as a 'cry for help' before abandoning an unsustainable project (e.g., 'Before I give up ... completely I wanted to give this one last try')."
    evidence: "qualitative"
    support_strength: "low-to-moderate"
    outcomes: ["burnout", "help-seeking"]
    predictors: ["workload", "open-source-maintenance"]
  - text: "Interrupted time-series models on 337 projects found no significant short-term change in commit activity after a project's first donation (β=0.03, n.s.), only a weak positive association between total earnings and commit volume (~35% more commits per e-fold increase in funding), and a decline in activity among projects that asked for but never received donations."
    evidence: "longitudinal"
    support_strength: "low-to-moderate"
    outcomes: ["productivity", "retention"]
    predictors: ["intervention", "open-source-maintenance"]
population:
  who: "Open-source software projects hosted on GitHub (and the subset also published on npm) that publicly request donations via detectable platforms (PayPal, Patreon, OpenCollective, Kickstarter, etc.); deeper qualitative sub-samples of README files, donation-platform profile pages, and OpenCollective transaction ledgers were also analyzed."
  where: []
  when: "Snapshot as of May 23, 2019, with longitudinal repository history extending back to roughly 2012"
  n: 25885
  sector: ["software-development", "open-source"]
  sample_notes: >
    Population sizes vary by research question: full census across 77.9M GitHub repos /
    537,640 npm packages (RQ1-2); 25,885 GitHub / 1,145 npm donation-seeking repos plus
    matched non-donation controls for regression modeling (RQ3-4); a purposive qualitative
    sample of 109 repositories for coding donation expectations (RQ5); 337 projects meeting
    activity-window requirements for interrupted time-series modeling (RQ6); and 60 hand-
    coded plus 540 auto-classified OpenCollective projects for spending analysis (RQ7).
    Authors deliberately excluded surveys/interviews with maintainers for ethical reasons
    (avoiding burdening a population already flagged as stressed/burned out), relying only
    on public artifacts.
limitation:
  primary: "The study relies entirely on public repository artifacts (README files, donation-platform pages, GHTorrent metadata) and explicitly avoided surveys or interviews with developers, so it cannot capture private/undetectable donation channels (e.g., Bitcoin, informal sponsorship) or developers' actual psychological state, motivations, or stress levels—only what they chose to disclose publicly."
  others:
    - "The interrupted time-series outcome models are correlational and rely on only two coarse proxy measures (commit counts, issue-resolution speed) for a small subsample of well-funded projects, and explicitly could not measure hypothesized outcomes like reduced developer stress or burnout."
    - "Findings are restricted to projects using automatically detectable donation platforms on GitHub as of a single May 2019 snapshot and may not generalize to non-GitHub-hosted projects or undisclosed funding arrangements."
    - "Self-reported donation goals in README/profile text may not honestly reflect maintainers' true intentions due to self-censorship of less socially acceptable motives (acknowledged by the authors)."
risk_of_bias: "medium"
relevance_to_project: >
  Provides empirical grounding for the SNH project's interest in maintainer burnout and
  sustainability: it documents how rare donation-based funding actually is (0.04% of GitHub
  repos), how often donation appeals are explicitly framed as a workload-driven 'cry for
  help' rather than routine fundraising, and shows that receiving donations does little to
  measurably relieve activity/workload strain—evidence that money alone is an insufficient
  intervention for open-source maintainer wellbeing and that other social-support mechanisms
  deserve attention.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "community-health", "methodology"]
  method: ["mixed-methods", "secondary-data", "regression-modeling"]
  population: ["open-source-maintainers", "github-repositories"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/How to Not Get Rich An Empirical Study of Donations in Open Source/How to Not Get Rich An Empirical Study of Donations in Open Source.md"
  pdf: "papers/Articles/01 Articles - Extended/How to Not Get Rich An Empirical Study of Donations in Open Source.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "larabel-2024-intel-survey-finds-maintainer-burnout-documentation"
title: "Intel Survey Finds Maintainer Burnout & Documentation Top Open-Source Challenges"
authors:
  - "Larabel, Michael"
year: 2024
doi: null
venue: {type: "other", name: "Phoronix", volume: null, issue: null, pages: null}
citation: "Larabel (2024). Intel Survey Finds Maintainer Burnout & Documentation Top Open-Source Challenges. Phoronix."
article_type: "commentary"
method: {design: "cross-sectional", approach: "survey", evidence_level: "weak", preregistered: false}
gist: >
  This Phoronix news article relays results from Intel's 2023 Open Source Community Survey,
  emailed to participants rather than published, reporting that maintainer burnout (45%) was
  the single most-cited challenge facing open-source projects, ahead of
  documentation/onboarding (41%) and sustainability (37%). It also reports that license
  acceptability, maintainer responsiveness, and a welcoming community were the attributes
  respondents valued most in an open-source project, and that most respondents view AI-
  related open source as important.
claims:
  - text: "Among top open-source challenges reported by Intel's 2023 survey respondents: maintainer burnout 45%, documentation and onboarding 41%, maintaining sustainability 37%, and building community engagement 32%."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["burnout"]
    predictors: ["workload", "community-engagement", "organizational-culture"]
  - text: "The most important attributes of an open-source project to survey respondents were an acceptable license, followed by maintainer responsiveness, activity volume, a welcoming community, and established policies/documentation."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["sense-of-belonging"]
    predictors: ["inclusiveness", "leadership-style"]
  - text: "82% of respondents found open source's role in AI either extremely or very important, and 30% said they contribute to open-source projects more than once per week."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["job-engagement"]
    predictors: ["community-engagement"]
population:
  who: "Self-selected participants in Intel's 2023 Open Source Community Survey, described as open-source developers/contributors"
  where: []
  when: "2023"
  n: null
  sector: ["open-source"]
  sample_notes: >
    Sample size, response rate, sampling method, and survey instrument are not disclosed in
    this journalistic write-up; results were emailed to participants by Intel and had not
    been publicly posted at the time of writing, so figures cannot be independently
    verified.
limitation:
  primary: "This is a journalist's secondary summary of an unpublished Intel survey with no disclosed sample size, response rate, or methodology, so reported percentages cannot be assessed for rigor or representativeness."
  others:
    - "No demographic, seniority, or project-type breakdown of respondents is given."
    - "Findings are self-report perceptions of challenges, not measured burnout or outcome data."
risk_of_bias: "high"
relevance_to_project: >
  Offers directly on-topic prevalence context for the SNH project's central concern by
  ranking maintainer burnout as the single most-cited open-source challenge (45%), ahead of
  documentation and sustainability, though its unverified methodology limits it to
  motivating context rather than rigorous evidence.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "community-health"]
  method: ["survey"]
  population: ["open-source-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/Intel Survey Finds Maintainer Burnout and Documentation Top Open-Source Challenges/Intel Survey Finds Maintainer Burnout and Documentation Top Open-Source Challenges.md"
  pdf: "papers/Articles/Intel Survey Finds Maintainer Burnout and Documentation Top Open-Source Challenges.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "anon-nd-release-assurance-why-innovative-software-delivery"
title: "Release Assurance: Why Innovative Software Delivery Starts with Trust and Psychological Safety"
authors:
year: null
doi: null
venue: {type: "report", name: "LaunchDarkly", volume: null, issue: null, pages: null}
citation: "LaunchDarkly (None). Release Assurance: Why Innovative Software Delivery Starts with Trust and Psychological Safety. LaunchDarkly."
article_type: "empirical"
method: {design: "cross-sectional", approach: "survey", evidence_level: "low", preregistered: false}
gist: >
  This vendor-commissioned survey report from LaunchDarkly (a feature-flag/release-
  management company) surveys 500 software developers and finds that psychological safety
  and leadership support around release risk are strongly tied to job satisfaction and
  retention. It reports that 67% of developers have quit or know a colleague who quit over
  pressure to minimize deployment mistakes, that job satisfaction is far higher when
  leadership prioritizes developer outcomes, and that confidence in a team's ability to
  safely release code is linked to felt empowerment to innovate.
claims:
  - text: "67% of developers say they themselves have quit a job (36%) or know someone who has (35%, overlapping categories) due to pressure to minimize deployment mistakes/rollbacks; among those who describe their release process as an obstacle to innovation, 74% report this quitting behavior, rising to 78% at companies where developer outcomes are a low priority."
    evidence: "cross-sectional"
    support_strength: "low"
    outcomes: ["turnover", "retention"]
    predictors: ["psychological-safety", "leadership-style", "organizational-culture"]
  - text: "92% of developers report being very (53%) or somewhat (39%) satisfied with their job; satisfaction is sharply higher (86%) at companies where leadership treats improving developer outcomes as a top/large priority versus only 14% satisfied where it is not a priority."
    evidence: "cross-sectional"
    support_strength: "low"
    outcomes: ["job-satisfaction"]
    predictors: ["leadership-style", "psychological-safety"]
  - text: "93% of developers agree that gaining confidence in their team's ability to safely release code makes them feel empowered to innovate more (52% strongly agree), and 56% say smaller, more frequent deployments would increase their confidence versus larger, less frequent ones."
    evidence: "cross-sectional"
    support_strength: "low"
    outcomes: ["job-engagement", "productivity"]
    predictors: ["psychological-safety", "workload"]
population:
  who: "500 software developers across a range of industries and job titles, surveyed for a LaunchDarkly-commissioned industry report"
  where: []
  when: null
  n: 500
  sector: ["technology", "software"]
  sample_notes: >
    Vendor-commissioned market-research survey; sampling frame, recruitment method, country
    mix, and survey instrument are not disclosed in the report, so representativeness cannot
    be assessed.
limitation:
  primary: "This is a vendor marketing/lead-generation report (published by LaunchDarkly, a release-management tool vendor) with no disclosed sampling methodology, response rate, or peer review, so findings should be treated as directional industry-survey data rather than rigorous research."
  others:
    - "All findings are self-reported cross-sectional percentages with no statistical testing, confidence intervals, or controls for confounds."
    - "Turnover figures rely on retrospective recall ('have you or someone you know ever quit'), which is prone to recall and social-desirability bias."
    - "No demographic, geographic, or company-size breakdown is given, limiting generalizability."
risk_of_bias: "high"
relevance_to_project: >
  Offers industry (non-academic) survey evidence that developers' perceived psychological
  safety around risk-taking and release process is linked to job satisfaction and self-
  reported turnover, which is relevant to the SNH project's interest in how organizational
  trust/leadership support functions as a predictor of burnout-adjacent turnover and
  retention in tech workplaces — though the vendor-sponsored, undisclosed-methodology nature
  means it should be cited as weak/corroborating evidence only, not as a primary source.
tags:
  topic: ["psychological-safety", "job-satisfaction", "productivity", "technostress"]
  method: ["survey"]
  population: ["software-developers", "industry-survey"]
source:
  markdown: "Papers_Data/Articles/MD/LaunchDarkly Release Assurance Why Innovative Software Delivery Starts with Trust and Psychological Safety/LaunchDarkly Release Assurance Why Innovative Software Delivery Starts with Trust and Psychological Safety.md"
  pdf: "papers/Articles/LaunchDarkly Release Assurance Why Innovative Software Delivery Starts with Trust and Psychological Safety.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "bekahhw-nd-maintainer-month-enhancing-support-for-open"
title: "Maintainer Month: Enhancing Support for Open Source Maintainers"
authors:
  - "BekahHW"
year: null
doi: null
venue: {type: "other", name: "OpenSauced Blog", volume: null, issue: null, pages: null}
citation: "BekahHW (None). Maintainer Month: Enhancing Support for Open Source Maintainers. OpenSauced Blog."
article_type: "commentary"
method: {design: "theory", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  This OpenSauced blog post argues that open source maintainers carry a high 'cognitive
  load' from code work, triage, documentation, and community mediation, and that this load —
  compounded by unpaid volunteer labor and unsustainable funding models — drives burnout and
  project abandonment. It proposes practical mitigations: streamlining issue triage,
  delegating to trusted community members with defined roles and onboarding, encouraging
  asynchronous communication norms, investing in documentation, and offering maintainers
  training and mentorship. It closes with a call to recognize and fund maintainers year-
  round rather than only during a designated 'Maintainer Month'.
claims:
  - text: "A 2021 Tidelift survey is cited as showing that a significant portion of open source maintainers feel undervalued, which the author links to risk of burnout and mental health issues."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["burnout", "mental-health"]
    predictors: ["organizational-culture", "open-source-maintenance"]
  - text: "The post asserts that high cognitive load from managing code, communication, and community responsibilities reduces maintainer efficiency and creativity and contributes to burnout, implying that reducing task and communication burden could improve maintainer sustainability."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["burnout", "productivity"]
    predictors: ["workload", "open-source-maintenance"]
  - text: "The author states that connecting maintainers to a community of peers and providing mentorship and training reduces the feeling of isolation that often accompanies the maintainer role."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["isolation", "sense-of-belonging"]
    predictors: ["peer-mentoring", "community-engagement"]
population:
  who: "Open source project maintainers generally, discussed rhetorically by an OpenSauced Developer Experience Lead; no primary sample studied"
  where: []
  when: null
  n: null
  sector: ["open-source"]
  sample_notes: >
    No original data collection; the piece cites a third-party 2021 Tidelift survey and
    other bloggers' reflections without reporting methods, sample size, or response rate.
limitation:
  primary: "The piece is an opinion/advocacy blog post with no original empirical data, methodology, or citations beyond informal links to other blogs and a secondhand reference to a survey."
  others:
    - "Recommendations (asynchronous work, delegation, documentation) are asserted as effective without any evaluation or outcome data."
    - "Author has an organizational stake (OpenSauced, a maintainer-tooling company) promoting its own blog content and products, a potential conflict of interest."
risk_of_bias: "high"
relevance_to_project: >
  Offers a practitioner-level taxonomy of maintainer cognitive load and burnout drivers
  (communication overload, volunteer attrition, unclear roles) plus concrete SNH-relevant
  interventions — role delegation, onboarding/mentorship, async norms, and documentation
  investment — that map onto community-engagement and peer-mentoring design levers for
  reducing maintainer isolation and burnout, though none are empirically validated here.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "isolation", "community-health"]
  method: ["theory"]
  population: ["open-source-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/Maintainer Month Enhancing Support for Open Source Maintainers/Maintainer Month Enhancing Support for Open Source Maintainers.md"
  pdf: "papers/Articles/Maintainer Month Enhancing Support for Open Source Maintainers.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "abbycabs-nd-maintaining-balance-for-open-source-maintainers"
title: "Maintaining Balance for Open Source Maintainers"
authors:
  - "abbycabs (GitHub)"
year: null
doi: null
venue: {type: "other", name: "opensource.guide (GitHub)", volume: null, issue: null, pages: null}
citation: "abbycabs (GitHub) (None). Maintaining Balance for Open Source Maintainers. opensource.guide (GitHub)."
article_type: "commentary"
method: {design: "qualitative", approach: "other", evidence_level: "weak", preregistered: false}
gist: >
  This GitHub-published guide distills themes from a workshop with 40 members of the GitHub
  Maintainer Community about burnout and 'personal ecology' (pacing and boundary-setting to
  sustain energy over time). It identifies recurring burnout drivers among open source
  maintainers -- lack of positive feedback, difficulty saying no, working alone,
  insufficient time/resources, and conflicting stakeholder demands -- and compiles practices
  maintainers said helped, such as delegating, building community support, setting explicit
  boundaries, seeking funding, and automating routine work.
claims:
  - text: "Workshop participants identified five recurring drivers of maintainer burnout: lack of positive feedback (users mostly surface complaints, not praise), difficulty saying no to added responsibilities, working alone/isolation, insufficient time or resources (especially for volunteer maintainers), and conflicting demands from users, contributors, and employers."
    evidence: "qualitative"
    support_strength: "weak"
    outcomes: ["burnout", "isolation"]
    predictors: ["workload", "isolation"]
  - text: "Maintainers reported that leaning on the community for delegation and having multiple points of contact for a project reduced burnout risk by allowing them to take breaks without the project stalling, and that explicit boundary-setting (e.g., stating limited review hours or PR criteria in the README) helped manage contributor and user expectations."
    evidence: "qualitative"
    support_strength: "weak"
    outcomes: ["burnout", "job-engagement"]
    predictors: ["social-support", "boundary-management"]
  - text: "Being a maintainer was described as isolating even when working alongside co-maintainers, a problem participants said had worsened in recent years due to reduced in-person convening of distributed teams; some maintainers reported using wearable technology to monitor sleep quality and heart-rate variability as early indicators of stress."
    evidence: "qualitative"
    support_strength: "weak"
    outcomes: ["loneliness", "stress"]
    predictors: ["isolation", "remote-work-intensity"]
population:
  who: "40 self-selected members of the GitHub-run Maintainer Community who took part in a workshop on burnout, self-care, and 'personal ecology' for open source maintainers"
  where: []
  when: null
  n: 40
  sector: ["open-source"]
  sample_notes: >
    Convenience/self-selected sample of maintainers already engaged with GitHub's Maintainer
    Community; no demographic, project-size, or geographic breakdown is reported, and no
    data collection or coding methodology is described -- findings are presented as thematic
    takeaways from a facilitated discussion rather than analyzed qualitative data.
limitation:
  primary: "Findings come from an undocumented, informally facilitated workshop with a small self-selected convenience sample (n=40), with no stated data collection, coding, or analysis method, so themes should be read as anecdotal practitioner consensus rather than rigorous qualitative research."
  others:
    - "No participant demographics, project characteristics, or maintainer tenure/role details are reported."
    - "Published as a practical how-to guide that blends workshop themes with general advice and links to external resources, without separating reported findings from the authors' own recommendations."
risk_of_bias: "high"
relevance_to_project: >
  Directly names loneliness/working-alone and unmanaged demands as maintainer-burnout
  drivers and points to community support and explicit boundary-setting as mitigations,
  informing SNH design choices around peer-support mechanisms and boundary/workload-
  management features for open-source maintainer health.
tags:
  topic: ["open-source", "burnout", "maintainer-burnout", "loneliness", "community-health"]
  method: ["qualitative"]
  population: ["open-source-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/Maintaining Balance for Open Source Maintainers/Maintaining Balance for Open Source Maintainers.md"
  pdf: "papers/Articles/Maintaining Balance for Open Source Maintainers.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "chan-2020-meet-the-developer-group-trying-to"
title: "Meet the Developer Group Trying to Break the Mental Health Stigma in Tech"
authors:
  - "Chan, Rosalie"
year: 2020
doi: null
venue: {type: "other", name: "Business Insider", volume: null, issue: null, pages: null}
citation: "Chan (2020). Meet the Developer Group Trying to Break the Mental Health Stigma in Tech. Business Insider."
article_type: "commentary"
method: {design: "case-study", approach: "interview", evidence_level: "weak", preregistered: false}
gist: >
  This Business Insider profile covers Open Sourcing Mental Illness (OSMI), a nonprofit
  founded by developer Ed Finkler in 2013 to destigmatize mental health struggles in the
  tech industry. It cites OSMI's annual survey finding that 51% of tech professionals report
  having been diagnosed with a mental health condition (versus roughly one in five U.S.
  adults per NAMI), and quotes OSMI advisory board psychologist Jen Akullian on how 'move
  fast and break things' culture, solo/remote work, high self-expectations, and the absence
  of HR support at many startups leave tech workers isolated and reluctant to seek help. It
  closes by noting some employers and tech conferences are beginning to add mental health
  programming.
claims:
  - text: "OSMI's annual survey of the tech/IT industry found 51% of respondents report having been diagnosed with a mental health condition, compared to roughly one in five U.S. adults nationally per NAMI data cited in the article."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["mental-health", "depression", "anxiety"]
    predictors: ["workload", "technostress"]
  - text: "Tech workers are often isolated by working alone or remotely, and many startups lack an HR department, so employees experiencing mental health issues frequently 'don't know where to go' for support and tend to keep problems to themselves."
    evidence: "qualitative"
    support_strength: "speculative"
    outcomes: ["isolation", "help-seeking", "mental-health"]
    predictors: ["isolation", "organizational-culture"]
  - text: "Unaddressed mental health strain in tech can escalate to burnout and to people quitting their jobs or careers, according to OSMI's advisory board psychologist."
    evidence: "qualitative"
    support_strength: "speculative"
    outcomes: ["burnout", "turnover", "mental-health"]
    predictors: ["workload", "organizational-culture"]
population:
  who: "Tech/software industry professionals surveyed annually by the OSMI nonprofit; article also draws on interviews with OSMI founder Ed Finkler and advisory board psychologist Jen Akullian"
  where: []
  when: null
  n: null
  sector: ["technology"]
  sample_notes: >
    This news article does not report OSMI survey methodology, sample size, sampling frame,
    or response rate; the cited 51% figure and NAMI comparison come from a third-party
    survey summarized secondhand, not from a study this article itself conducted.
limitation:
  primary: "This is a journalistic profile, not a peer-reviewed or methodologically documented study; the headline statistic (51% of tech professionals diagnosed with a mental health condition) is cited from an advocacy organization's self-administered survey without sample size, recruitment method, or response rate reported."
  others:
    - "Quotes are drawn from a small number of interested parties (the organization's founder and an advisory board member), with no independent or critical sourcing."
    - "No comparison group methodology is given for the NAMI 'one in five U.S. adults' statistic used as a benchmark."
risk_of_bias: "high"
relevance_to_project: >
  Provides an oft-cited anecdotal prevalence figure (51% of tech professionals reporting a
  mental health diagnosis) and a first-person account of why isolation, solo/remote work,
  and lack of organizational support structures suppress help-seeking in tech workplaces --
  directly relevant to SNH's framing of isolation and stigma as barriers to help-seeking and
  to designing peer-support or advisory interventions modeled on OSMI's approach.
tags:
  topic: ["mental-health", "burnout", "isolation", "help-seeking", "psychological-safety"]
  method: ["survey", "interview"]
  population: ["software-developers"]
source:
  markdown: "Papers_Data/Articles/MD/Meet the Developer Group Trying to Break the Mental Health Stigma in Tech/Meet the Developer Group Trying to Break the Mental Health Stigma in Tech.md"
  pdf: "papers/Articles/Meet the Developer Group Trying to Break the Mental Health Stigma in Tech.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "fu-2024-mental-health-in-open-source"
title: "Mental Health in Open Source"
authors:
  - "Fu, Anthony"
year: 2024
doi: null
venue: {type: "other", name: "antfu.me (personal blog)", volume: null, issue: null, pages: null}
citation: "Fu (2024). Mental Health in Open Source. antfu.me (personal blog)."
article_type: "commentary"
method: {design: "case-study", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  A personal blog post by a prolific open-source maintainer (creator/co-maintainer of Vite,
  UnoCSS, Slidev, Vitest, VueUse) reflecting on four years of near-burnout while sustaining
  a high-velocity, high-quality, wide-scope maintenance workload across many popular
  projects. He attributes his ability to keep going to community/co-maintainer support,
  deliberate lowering of self-expectations, and boundary-setting around notifications,
  framing sustainable maintainer mental health as a continuous, individual process of
  adaptation rather than a solvable problem.
claims:
  - text: "The author describes a structurally unbalanced maintainer-to-user ratio in open source: it is very hard to recruit new collaborators or team members, while user growth is essentially frictionless because the software is free, concentrating workload and pressure on a small number of maintainers."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "stress"]
    predictors: ["workload", "network-structure", "community-engagement"]
  - text: "The author reports that deliberately lowering self-expectations, accepting that maintainers are not obligated to fix every issue, and switching from passive push notifications to proactively checking issues on his own schedule allowed him to recover from low points/near-burnout episodes within roughly a week."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "wellbeing"]
    predictors: ["boundary-management", "autonomy", "workload"]
  - text: "The author states he was only able to simultaneously sustain high velocity, high quality, and a wide scope of projects (seemingly defying the classic project-management 'iron triangle') because of substantial help from co-maintainers and the surrounding community, and that without that support he 'should have reached my limit a long while ago.'"
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "collaboration"]
    predictors: ["community-engagement", "team-cohesion", "peer-mentoring"]
population:
  who: "Single autobiographical account of one prolific open-source maintainer (Anthony Fu), reflecting on ~4 years maintaining multiple high-traffic JavaScript/Vue-ecosystem projects (Vite, UnoCSS, Slidev, Vitest, VueUse, Nuxt DevTools, etc.)"
  where: []
  when: "2024 (published Mar 16, 2024; reflects on 2020-2024)"
  n: 1
  sector: ["open-source"]
  sample_notes: >
    First-person personal blog post / diary-style reflection, n=1 self-report with no
    systematic data collection, sampling, or external validation; highly subjective and
    specific to the author's own projects and circumstances.
limitation:
  primary: "This is a single-author personal essay/blog post, not a research study: it presents one maintainer's anecdotal self-report with no systematic data collection, comparison group, or validated measures, so findings cannot be generalized beyond the author's own experience."
  others:
    - "No validated burnout, stress, or wellbeing instruments were used; assessments are entirely retrospective and introspective."
    - "The author explicitly flags his own opinions as 'heavily biased.'"
    - "Survivorship bias: the account is written by a maintainer who explicitly says he has not (yet) burned out or quit."
risk_of_bias: "high"
relevance_to_project: >
  Provides a rich first-person case exemplar of open-source maintainer burnout mechanisms
  directly relevant to SNH's maintainer-burnout work: the structural maintainer-to-user
  imbalance as a chronic stressor, notification/attention boundary-management as a burnout
  mitigation tactic, and community/co-maintainer support as the key buffer enabling
  sustained high-velocity contribution. Useful for motivating design interventions (e.g.,
  notification controls, peer-support or co-maintainer structures) rather than as
  generalizable evidence.
tags:
  topic: ["maintainer-burnout", "open-source", "burnout", "wellbeing", "community-health"]
  method: ["case-study"]
  population: ["open-source-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/Mental Health in Open Source/Mental Health in Open Source.md"
  pdf: "papers/Articles/Mental Health in Open Source.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "coates-2024-mental-health-of-developers-in-the"
title: "Mental Health of Developers in the Open Source Landscape"
authors:
  - "Coates, Tim"
year: 2024
doi: null
venue: {type: "other", name: "Tim Coates Insights (blog)", volume: null, issue: null, pages: null}
citation: "Coates (2024). Mental Health of Developers in the Open Source Landscape. Tim Coates Insights (blog)."
article_type: "commentary"
method: {design: "theory", approach: "analytical", evidence_level: "speculative", preregistered: false}
gist: >
  This blog post argues that open-source software (OSS) development, while collaborative and
  innovation-driving, exposes developers to distinct mental-health stressors: skill
  mismatches when assigned unfamiliar codebases, performance anxiety from public community
  scrutiny, and burnout from uncompensated volunteer maintenance labor. Drawing on other
  developers' and maintainers' personal blog posts (Antfu, Rob Mensching, Vadim Kravcenko)
  rather than original data, it also links remote work and long solo coding hours to social
  isolation, loneliness, anxiety, and depression, and closes with practitioner-style
  recommendations (training, documentation platforms, appreciation culture, realistic
  deadlines, EAP access) for employers and OSS communities.
claims:
  - text: "Open-source maintainers frequently experience burnout from uncompensated volunteer labor sustaining popular projects, compounded by performance anxiety from having their contributions publicly scrutinized by the community."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["burnout", "anxiety"]
    predictors: ["workload", "open-source-maintenance"]
  - text: "A mismatch between a developer's existing skillset and the codebase of an open-source project they are assigned to work with (e.g., a C/C++ developer debugging a PHP-based tool) is described as a recurring source of frustration for both contributors and reviewing maintainers."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["stress"]
    predictors: ["workload", "open-source-maintenance"]
  - text: "Remote work and extended solo coding time are described as contributing to social isolation, loneliness, anxiety, and depression among developers, alongside imposter syndrome driven by chronic self-doubt despite demonstrable skill."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["isolation", "loneliness", "anxiety", "depression"]
    predictors: ["remote-work-intensity", "work-life-balance"]
population:
  who: "Software developers generally, with emphasis on open-source project contributors and maintainers; characterized entirely through the author's synthesis of other individual bloggers' first-person accounts and secondary journalism, not a primary study sample."
  where: []
  when: null
  n: null
  sector: ["software-development", "open-source"]
  sample_notes: >
    No primary data collection, survey, or systematic literature search was conducted;
    evidence consists of anecdotes from named individual bloggers (Antfu, Rob Mensching,
    Vadim Kravcenko), an anonymous developer quote, general references to Reddit discussion,
    and citations to informal tech-industry articles (TechCrunch, Information Age,
    SurveyPoint.ai).
limitation:
  primary: "The piece is an opinion/synthesis blog post that cites other bloggers' anecdotes, an anonymous quote, and informal journalism rather than peer-reviewed empirical research on developer mental health, so its claims cannot be treated as validated findings."
  others:
    - "No original data collection, sampling, or systematic evidence search underlies the claims."
    - "Sources cited are themselves informal personal blogs of uncertain rigor and representativeness."
    - "No effect sizes, prevalence estimates, or comparison groups are reported anywhere in the piece."
risk_of_bias: "high"
relevance_to_project: >
  Surfaces practitioner-level candidate predictors of OSS-maintainer burnout and isolation
  (uncompensated labor, skill mismatch, public scrutiny, remote-work solo hours) that the
  SNH project can treat as hypotheses to test with real data, and catalogs informally-
  proposed mitigations (appreciation culture, contribution guidelines, EAP access, realistic
  deadlines) as intervention ideas worth formal evaluation rather than as established
  evidence.
tags:
  topic: ["open-source", "maintainer-burnout", "mental-health", "isolation", "remote-work"]
  method: ["analytical"]
  population: ["software-developers", "open-source-contributors", "remote-workers"]
source:
  markdown: "Papers_Data/Articles/MD/Mental Health of Developers in the Open Source Landscape/Mental Health of Developers in the Open Source Landscape.md"
  pdf: "papers/Articles/Mental Health of Developers in the Open Source Landscape.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "anon-2021-open-source-and-mental-health-r"
title: "Open Source and Mental Health (r/Redox discussion thread)"
authors:
year: 2021
doi: null
venue: {type: "other", name: "Reddit r/Redox", volume: null, issue: null, pages: null}
citation: "Reddit r/Redox (2021). Open Source and Mental Health (r/Redox discussion thread). Reddit r/Redox."
article_type: "commentary"
method: {design: "qualitative", approach: "other", evidence_level: "weak", preregistered: false}
gist: >
  Community discussion thread (r/Redox, June 2021) responding to Jeremy Soller's post about
  the death, believed suicide, of 18-year-old Redox OS contributor jD91mZM2. Comments show
  how an open-source community processes a member's death in public: grief and self-
  forgiveness framing, calls to reduce help-seeking stigma, safe-messaging correction ('died
  by suicide'), and a prominent Rust author's first-person account of how his influential
  critical writing contributed to another maintainer's burnout and now threatens his own
  sustainability in open source.
claims:
  - text: "A widely-read Rust ecosystem author (Shnatsel) states he knows 'for certain' his articles (10k-50k views each) significantly contributed to the burnout of at least one prolific open-source maintainer, that the emotional fallout stopped his own writing for over a year, and that unpriced 'people costs' leave him questioning whether open source is sustainable for him."
    evidence: "qualitative"
    support_strength: "weak"
    outcomes: ["burnout", "retention"]
    predictors: ["community-engagement", "organizational-culture"]
  - text: "Commenters counsel the grieving maintainer against self-blame, arguing suicide is a cumulative process where 'sometimes having someone reach out isn't enough' — a community-articulated limit on what check-in practices can promise."
    evidence: "qualitative"
    support_strength: "speculative"
    outcomes: ["suicidal-ideation", "mental-health"]
    predictors: ["social-support"]
  - text: "The thread itself performs several protective practices discussed in the SNH literature: public de-stigmatization of help-seeking, safe-messaging language correction, and peer disclosure of personal mental-health management strategies."
    evidence: "qualitative"
    support_strength: "speculative"
    outcomes: ["help-seeking", "sense-of-belonging"]
    predictors: ["community-engagement", "inclusiveness"]
population:
  who: "Redox OS / Rust open-source community members commenting publicly"
  where: []
  when: "June 2021"
  n: 12
  sector: ["open-source", "tech"]
  sample_notes: >
    Self-selected public commenters on a link post; captured 2026-07-08 from the live thread
    after the original archive turned out to be a login-wall page; a few deleted comments
    and two collapsed replies not captured.
limitation:
  primary: "Self-selected anonymous forum comments with no verifiability; grief context shapes what is said publicly."
  others:
    - "Original 2026 capture was lost; thread identified later as the best candidate, so provenance to the corpus's original intent is uncertain."
    - "Small visible sample; deleted comments unrecoverable."
risk_of_bias: "high"
relevance_to_project: >
  Primary-source community reaction to a contributor suicide: documents both the demand for
  check-in practices and the community's own caution about their limits (informing
  checkin_protocol.md in the social-network-health repo), plus a rare first-person account
  of critic-side burnout dynamics in open source.
tags:
  topic: ["open-source", "mental-health", "suicide-prevention", "community-health", "maintainer-burnout"]
  method: ["qualitative"]
  population: ["open-source", "tech"]
source:
  markdown: "Papers_Data/Articles/MD/Open Source and Mental Health Reddit Discussion Redox Community/Open Source and Mental Health Reddit Discussion Redox Community.md"
  pdf: null
  notes: "no-doi: web article / no registered DOI found"

---

id: "soller-2021-open-source-and-mental-health"
title: "Open Source and Mental Health"
authors:
  - "Soller, Jeremy"
year: 2021
doi: null
venue: {type: "other", name: "Redox OS", volume: null, issue: null, pages: null}
citation: "Soller (2021). Open Source and Mental Health. Redox OS."
article_type: "commentary"
method: {design: "case-study", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  The founder of the Redox OS operating system project writes a first-person reflection
  after a prolific young contributor's apparent suicide, arguing that open source
  communities systematically neglect the mental health of their contributors in favor of
  valuing code output. He describes his own history of ADHD, depression, and isolation, and
  argues that chronic stressors (poor project environment, social isolation, purely task-
  focused interaction) combine with acute triggers to produce mental health crises among
  maintainers and contributors, and calls for the community to check in on each other's
  wellbeing rather than only their code.
claims:
  - text: "The author reports that a prolific 18-year-old Redox OS contributor died, apparently by suicide, after a period of being unresponsive and 'offline,' with the author's last contact having been a purely technical exchange one month prior."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["suicidal-ideation", "isolation"]
    predictors: ["isolation", "social-support"]
  - text: "The author asserts, without citing formal data, that ADHD, autism, bipolar disorder, depression, and other disorders are 'incredibly common' among open source contributors, and that a resulting lack of soft skills isolates open source communities from mainstream social norms."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["mental-health", "isolation"]
    predictors: ["community-engagement", "organizational-culture"]
  - text: "The author frames mental health crises as arising from a combination of chronic stressors (e.g., a sustained poor home/work/project environment) and acute triggering events (e.g., an argument), and argues open source projects have largely failed to investigate or mitigate the human/mental-health cost of contribution, sometimes leading to burnout and departure and sometimes to suicide."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "turnover", "mental-health"]
    predictors: ["organizational-culture", "workload", "isolation"]
population:
  who: "Single first-person case narrative by the Redox OS project founder, referencing one deceased contributor and the author's own mental health history; no systematic sample."
  where: []
  when: "2021"
  n: null
  sector: ["open-source"]
  sample_notes: >
    Not a study; an anecdotal blog post/eulogy with n=1 documented case (the deceased
    contributor) plus the author's autobiographical account. No methodology, no comparison
    group, no formal data collection.
limitation:
  primary: "This is a personal blog post/eulogy, not research: it presents anecdote and the author's own theorizing about suicide and mental illness as if established fact, with no citations, data, or methodology."
  others:
    - "Claims about the prevalence of psychiatric conditions among open source contributors and about the neuroscience of suicide are asserted without evidence."
    - "Single-case retrospective account is highly susceptible to hindsight bias and cannot support causal claims about what contributed to the death."
risk_of_bias: "high"
relevance_to_project: >
  Provides a maintainer-voice, ground-level illustration of the SNH project's core concern
  -- that open source communities can be organized around code output at the expense of
  contributor social/emotional wellbeing -- and is a useful qualitative anecdote motivating
  measures of isolation, check-in practices, and maintainer burnout, though it cannot be
  used as evidentiary support for prevalence or causal claims.
tags:
  topic: ["open-source", "mental-health", "suicide-prevention", "maintainer-burnout", "isolation", "community-health"]
  method: ["case-study"]
  population: ["open-source-contributors"]
source:
  markdown: "Papers_Data/Articles/MD/Open Source and Mental Health Redox OS/Open Source and Mental Health Redox OS.md"
  pdf: "papers/Articles/Open Source and Mental Health Redox OS.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "speed-2025-open-source-maintainers-are-really-feeling"
title: "Open source maintainers are really feeling the squeeze"
authors:
  - "Speed, Richard"
year: 2025
doi: null
venue: {type: "other", name: "The Register", volume: null, issue: null, pages: null}
citation: "Speed (2025). Open source maintainers are really feeling the squeeze. The Register."
article_type: "commentary"
method: {design: "case-study", approach: "interview", evidence_level: "weak", preregistered: false}
gist: >
  This Register news article surveys the state of open source maintainer burnout as of early
  2025, built around quotes from the State Of Open Conference (SOO), the abrupt resignation
  of Asahi Linux lead Hector Martin, and interviews with maintainers (Jamie Tanna) and
  researchers (Google's Sophia Vargas, Kubernetes maintainers Kat Cosgrove and Jeremy
  Rickard). It cites external survey data showing widespread maintainer overload and abuse
  from entitled users, and argues that pay alone will not fix the problem — many projects
  need more contributors for non-code labor (mentorship, triage, community management) as
  much as money.
claims:
  - text: "The 2024 Tidelift State of the Open Source Maintainer survey found that roughly 60% of maintainers had either quit or were considering quitting, cited as evidence of chronic under-support relative to the growing enterprise appetite for open source software."
    evidence: "cross-sectional"
    support_strength: "low"
    outcomes: ["turnover", "burnout"]
    predictors: ["workload", "organizational-culture"]
  - text: "In an informal survey of Kubernetes project contributors (explicitly described by the researchers as too small to be statistically significant), 70% of respondents who observed abuse directed at maintainers said they had considered whether to keep contributing to the project."
    evidence: "cross-sectional"
    support_strength: "speculative"
    outcomes: ["turnover", "community-engagement"]
    predictors: ["organizational-culture", "psychological-safety"]
  - text: "Analysis referenced from the Linux Foundation/Harvard Census II report indicates that even widely used, 'critical infrastructure' open source projects are typically maintained by very few people, often with a single person doing most of the work, concentrating burnout and continuity risk."
    evidence: "cross-sectional"
    support_strength: "low-to-moderate"
    outcomes: ["burnout", "turnover"]
    predictors: ["open-source-maintenance", "workload"]
population:
  who: "Open source maintainers and contributors discussed via conference talks and interviews (e.g., Jamie Tanna of oapi-codegen, Hector Martin of Asahi Linux, Kubernetes maintainers Kat Cosgrove and Jeremy Rickard), plus survey populations cited secondhand (Tidelift maintainer respondents, Linux Foundation Census II project contributors)."
  where: []
  when: "2024-2025"
  n: null
  sector: ["technology", "open-source"]
  sample_notes: >
    This is a journalistic article, not a primary study: it synthesizes conference quotes,
    individual interviews, and citations to external survey reports rather than presenting
    its own sampled data; underlying survey sample sizes and response rates are not given in
    the article.
limitation:
  primary: "The article is journalism, not primary research — it aggregates quotes and secondhand citations of other organizations' surveys/reports without presenting original methodology, sampling, or data."
  others:
    - "The Kubernetes maintainer survey it cites is explicitly flagged by its own researchers as too small to be statistically significant."
    - "No details on response rates, sampling frames, or measurement instruments are provided for the Tidelift or Linux Foundation figures it references."
risk_of_bias: "high"
relevance_to_project: >
  Gives the SNH project current, quotable texture on maintainer burnout mechanisms — abusive
  user interactions, chronic under-resourcing, and concentration of workload on very few
  contributors ('bus factor') — and flags two primary sources worth pulling directly (2024
  Tidelift maintainer survey; Linux Foundation/Harvard Census II) for harder evidence on
  open-source maintainer turnover and burnout.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "community-health"]
  method: ["qualitative", "secondary-data"]
  population: ["open-source-maintainers", "open-source-contributors"]
source:
  markdown: "Papers_Data/Articles/MD/Open Source Maintainers Are Really Feeling the Squeeze/Open Source Maintainers Are Really Feeling the Squeeze.md"
  pdf: "papers/Articles/Open Source Maintainers Are Really Feeling the Squeeze.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "mcquaid-2018-open-source-maintainers-owe-you-nothing"
title: "Open Source Maintainers Owe You Nothing"
authors:
  - "McQuaid, Mike"
year: 2018
doi: null
venue: {type: "other", name: "mikemcquaid.com", volume: null, issue: null, pages: null}
citation: "McQuaid (2018). Open Source Maintainers Owe You Nothing. mikemcquaid.com."
article_type: "commentary"
method: {design: "theory", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  A veteran open-source maintainer (Homebrew, 8+ years) argues that most open-source
  licenses (MIT, BSD, GPLv3, MPL, Apache) explicitly disclaim warranty and liability, and
  that maintainer burnout stems from users and maintainers alike adopting an unwritten
  customer-service relationship the license never promised. The essay's proposed fix is a
  mindset/behavior change: maintainers should feel free to disengage from unenjoyable work
  and set boundaries, contributors should defer to maintainers, and users should treat
  contributions as gifts rather than entitlements.
claims:
  - text: "Nearly all major open-source licenses (MIT, BSD 2-Clause, GPLv3, MPLv2.0, Apache v2.0, Unlicense) explicitly disclaim warranty and limit liability, meaning maintainers have no formal legal obligation to fix bugs, respond to issues, or support any particular use case."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["burnout"]
    predictors: ["organizational-culture"]
  - text: "The author identifies the mismatch between the license's zero-obligation terms and the de facto 'business/customer-like' relationship that develops in practice (maintainers apologizing and rushing fixes, users expecting support) as one of the biggest drivers of maintainer burnout."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["burnout", "job-engagement"]
    predictors: ["organizational-culture", "workload"]
  - text: "The author claims many maintainers begin contributing for enjoyment but continue out of a felt sense of obligation, and that this shift from intrinsic motivation to obligation-driven unpaid labor is what 'grinds them down' over time and can lead to project abandonment."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["burnout"]
    predictors: ["organizational-culture", "boundary-management"]
population:
  who: "Personal essay by Mike McQuaid, an individual open-source maintainer (Homebrew) reflecting on his own ~10 years of open-source community experience; not an empirical study of a sample."
  where: []
  when: "2018"
  n: null
  sector: ["open-source"]
  sample_notes: >
    Single-author opinion/experience essay; no data collection, sample, or systematic
    evidence base beyond the author's personal observations and license text analysis.
limitation:
  primary: "This is a first-person opinion essay with no empirical data, sample, or citations to research; all claims about burnout causes and fixes are the author's personal interpretation."
  others:
    - "Generalizes from one maintainer's experience (Homebrew) to open-source maintainers broadly."
    - "Proposed solution (boundary-setting, 'owe nothing' framing) is asserted rather than tested against outcomes like retention or wellbeing."
risk_of_bias: "high"
relevance_to_project: >
  Provides a maintainer-voiced account of a specific mechanism behind open-source maintainer
  burnout -- the gap between license-defined zero-obligation and the informal customer-
  service expectations that build up in practice -- and a boundary-setting/expectation-
  management intervention idea relevant to designing supports for maintainer wellbeing and
  community norms.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "community-health"]
  method: ["theory"]
  population: ["open-source"]
source:
  markdown: "Papers_Data/Articles/MD/Open Source Maintainers Owe You Nothing/Open Source Maintainers Owe You Nothing.md"
  pdf: "papers/Articles/Open Source Maintainers Owe You Nothing.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "salkever-2023-open-source-maintainers-exploring-the-people"
title: "Open Source Maintainers: Exploring the people, practices, and constraints facing the world's most critical open source software projects"
authors:
  - "Salkever, Alex"
year: 2023
doi: null
venue: {type: "report", name: "Linux Foundation Research", volume: null, issue: null, pages: null}
citation: "Salkever (2023). Open Source Maintainers: Exploring the people, practices, and constraints facing the world's most critical open source software projects. Linux Foundation Research."
article_type: "empirical"
method: {design: "qualitative", approach: "interview", evidence_level: "low-to-moderate", preregistered: false}
gist: >
  Based on 32 hour-long interviews with 'super maintainers' of critical open source projects
  (e.g., Linux, Kubernetes, PostgreSQL, Git, NumPy, PyTorch, Storybook), this Linux
  Foundation report documents how maintainers balance contributor onboarding, governance,
  documentation, funding, diversity, and burnout. It finds that contributor experience is
  widely perceived to degrade as projects mature, that most maintainers are salaried to work
  on their projects yet feel under-recognized, and that maintainers rely on informal, self-
  devised boundary-setting and automation practices to avoid burnout. The report synthesizes
  these interviews into a set of practitioner best-practices rather than testing hypotheses.
claims:
  - text: "75% of the 32 interviewed super-maintainers served as both maintainers and code contributors (25% maintainer-only, none contributor-only), spending an average of 70% of their working time on the open source project; only one of the projects examined had just a single maintainer."
    evidence: "qualitative"
    support_strength: "low"
    outcomes: ["collaboration"]
    predictors: ["workload"]
  - text: "Multiple long-tenured maintainers (e.g., PostgreSQL's Andres Freund) reported that new-contributor experience has deteriorated over time as project maturity, PR volume, and code complexity increased, leading to slower, shallower maintainer responses than early contributors received, despite deliberate efforts to preserve a welcoming onboarding experience."
    evidence: "qualitative"
    support_strength: "low"
    outcomes: ["retention"]
    predictors: ["workload", "community-engagement"]
  - text: "Maintainers described burnout as driven by the public, always-on, consensus-heavy nature of open source governance (illustrated by Jupyter's 2022 shift from rough consensus to a modular Executive Committee/Steering Council structure after consensus-driven decision-making contributed to leader burnout), and reported preventing it via explicit work-hour/communication boundaries, workflow automation, accepting the work is never 'finished,' and taking breaks."
    evidence: "qualitative"
    support_strength: "low"
    outcomes: ["burnout"]
    predictors: ["boundary-management", "leadership-style"]
population:
  who: "32 purposively selected 'super maintainers' and core contributors of open source projects identified by LF Research's Census II work as among the ~200 most critical/widely-depended-upon OSS projects (e.g., Linux, Kubernetes, containerd, PostgreSQL, Git, cURL, NumPy, PyTorch, Jupyter, Storybook, Salt, Webpack, Babel, React)."
  where: []
  when: "interviews conducted prior to publication in July 2023; exact interview window not stated"
  n: 32
  sector: ["open-source"]
  sample_notes: >
    Purposive, non-random sample skewed toward well-resourced, full-time-employed
    maintainers (all but two had full-time employer support) of long-lived, high-visibility
    projects backed by large tech companies (Amazon, Microsoft, IBM, Meta, VMware, Red Hat);
    maintainers drawn from 'a half dozen countries', 6 of 32 female; three interviewees
    discussed past (not current) maintainer roles. Not representative of the broader
    population of smaller or unaffiliated OSS maintainers.
limitation:
  primary: "Small, purposive, non-random sample of 32 highly visible 'super maintainers' from large, well-funded, corporate-backed projects limits generalizability to typical, smaller, or unaffiliated open source maintainers, who the report itself notes face different funding and burnout pressures."
  others:
    - "No formal qualitative coding methodology, inter-rater reliability, or preregistration is described; findings are presented as narrative synthesis of interview themes and illustrative quotes rather than systematically coded/quantified results."
    - "Produced and funded by the Linux Foundation itself, which may bias framing toward practices favorable to foundation-affiliated and corporate-sponsored open source models."
    - "Reported percentages (e.g., 75% dual role, 38% employer support) come from a self-selected group of 32 and are presented without confidence intervals or statistical testing."
risk_of_bias: "medium"
relevance_to_project: >
  Provides concrete, named burnout-prevention practices (boundary-setting, automation,
  distributing governance/decision-making, employer financial support) and a documented case
  (Jupyter's consensus-to-council governance shift) linking maintainer burnout to
  organizational structure, which the SNH project can draw on when designing interventions
  or measures for maintainer-burnout and community-engagement in open-source/tech
  communities.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "community-health"]
  method: ["qualitative"]
  population: ["open-source-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/Open Source Maintainers Report 2023 Linux Foundation Research/Open Source Maintainers Report 2023 Linux Foundation Research.md"
  pdf: "papers/Articles/Open Source Maintainers Report 2023 Linux Foundation Research.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "zhu-2019-open-source-of-anxiety"
title: "(Open) source of anxiety"
authors:
  - "Zhu, Henry"
year: 2019
doi: null
venue: {type: "other", name: "Increment", volume: null, issue: null, pages: null}
citation: "Zhu (2019). (Open) source of anxiety. Increment."
article_type: "commentary"
method: {design: "case-study", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  A first-person essay by Henry Zhu, a maintainer of the Babel JavaScript compiler and
  former maintainer of JSCS, recounts how open-source maintainer work eroded his boundaries
  and mental health, producing chronic anxiety and physical symptoms like insomnia, eczema,
  and backaches. He argues the mismatch between a huge, largely invisible user base and a
  tiny, under-resourced maintainer team is structural, and calls for transparency mechanisms
  (workload visibility, queue systems) and built-in rest cycles ('digital seasons') to make
  maintenance sustainable.
claims:
  - text: "The author describes experiencing sustained anxiety and physical symptoms (insomnia, eczema flare-ups, backaches) that he attributes directly to unbounded, always-on maintainer responsibilities and the inability to set boundaries around communication and availability."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "anxiety", "mental-health"]
    predictors: ["workload", "boundary-management", "open-source-maintenance"]
  - text: "Babel, the compiler he maintains, was kept running by six people with only the author working on it full time, yet at the time of writing had over 1.7 million dependent repositories on GitHub and had surpassed 8.5 million weekly npm downloads for v7 alone -- a case illustration of the gap between infrastructure scale and maintainer capacity."
    evidence: "case-study"
    support_strength: "weak"
    outcomes: ["burnout", "sustainability"]
    predictors: ["workload", "open-source-maintenance"]
  - text: "The author argues that maintainer overload is worsened by lack of transparency about workload and queues, and by open-source culture having no equivalent of seasonal or ritual rest; he proposes visibility tools (e.g., a take-a-number style queue) and community-defined boundary practices as remedies."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "communication"]
    predictors: ["boundary-management", "organizational-culture"]
population:
  who: "Single open-source maintainer (Babel, formerly JSCS) reflecting on his own personal experience; no other participants studied"
  where: []
  when: null
  n: 1
  sector: ["open-source", "software"]
  sample_notes: >
    First-person autobiographical essay, not a research study; no sampling, recruitment, or
    data collection procedures -- observations are drawn solely from the author's own
    retrospective account.
limitation:
  primary: "This is a single first-person, retrospective personal essay rather than a research study, so its observations reflect one individual's experience and cannot be generalized to maintainers broadly."
  others:
    - "No systematic data collection, measurement instruments, or comparison group"
    - "Published as an opinion/personal essay in a magazine (Increment), not peer-reviewed"
risk_of_bias: "high"
relevance_to_project: >
  Offers vivid first-person qualitative evidence of the mechanisms behind maintainer burnout
  in open-source communities -- blurred work/life boundaries, invisibility of non-coding
  labor, and severe mismatch between dependent user base and maintainer headcount --
  directly informing the SNH project's understanding of maintainer-burnout risk factors and
  possible boundary-management or workload-transparency interventions.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "mental-health", "wellbeing"]
  method: ["qualitative", "case-study"]
  population: ["open-source-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/Open Source of Anxiety/Open Source of Anxiety.md"
  pdf: "papers/Articles/Open Source of Anxiety.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "steinmacher-2019-overcoming-social-barriers-when-contributing-to"
title: "Overcoming Social Barriers When Contributing to Open Source Software Projects"
authors:
  - "Steinmacher, Igor"
  - "Gerosa, Marco"
  - "Conte, Tayana U."
  - "Redmiles, David F."
year: 2019
doi: "10.1007/s10606-018-9335-z"
venue: {type: "journal", name: "Computer Supported Cooperative Work (CSCW)", volume: 28, issue: "1-2", pages: "247-290"}
citation: "Steinmacher et al. (2019). Overcoming Social Barriers When Contributing to Open Source Software Projects. Computer Supported Cooperative Work (CSCW), 28(1-2), 247-290. https://doi.org/10.1007/s10606-018-9335-z"
article_type: "empirical"
method: {design: "mixed-methods", approach: "interview", evidence_level: "moderate", preregistered: false}
gist: >
  Through a systematic literature review, practitioner surveys, and semi-structured
  interviews with 35 developers across 13 OSS projects, the authors build a model of 58
  onboarding barriers, 13 of them social (e.g., not receiving an answer, impolite replies,
  difficulty finding a mentor, shyness, cultural/language differences). They then design and
  evaluate FLOSScoach, an onboarding portal built from the model, in a two-iteration diary
  study with 43 undergraduate contributors, finding it reduced newcomers' need to interact
  with the community and helped those who did reach out communicate more effectively.
claims:
  - text: "13 social barriers were identified and organized into categories (reception issues, newcomers' communication behavior, finding a mentor, language/cultural differences); reception problems such as 'not receiving an answer' and 'delayed answers' were the most frequently and consistently evidenced across the SLR, surveys, and interviews."
    evidence: "qualitative"
    support_strength: "moderate"
    outcomes: ["retention", "communication", "isolation"]
    predictors: ["social-support", "community-engagement", "sampling-method"]
  - text: "In the FLOSScoach diary study, 15 of 43 tracked participants attempted to interact with the community at all, and every participant who did receive a community response reported it was welcoming and helpful, while three participants who received no answer described frustration ('demotivated', 'anesthetized'); the portal group completed the assignment at a higher rate (24/31, 77%) than the control group (19/34, 56%)."
    evidence: "mixed-methods"
    support_strength: "low-to-moderate"
    outcomes: ["communication", "collaboration", "retention"]
    predictors: ["intervention", "social-support"]
  - text: "Projects hosted on social-coding platforms (GitHub/GitLab) showed fewer mentions of social barriers such as difficulty finding a mentor than projects on their own forges or SourceForge, and older/larger projects tended to present more reported barriers, though difficulty finding a mentor and reception issues recurred across nearly all project types regardless of size, age, or language."
    evidence: "qualitative"
    support_strength: "weak"
    outcomes: ["collaboration", "retention"]
    predictors: ["network-structure", "peer-mentoring", "organizational-culture"]
population:
  who: "OSS project newcomers, dropouts, and experienced/core members from real-world community-based projects (Phase I: 9 students, 24 survey respondents, 35 interviewees across 13-19 projects incl. LibreOffice, OpenOffice, JabRef, Firefox, Moodle); Phase II: 43 analyzed undergraduate CS students recruited from two Brazilian universities to attempt real OSS contributions with or without the FLOSScoach portal"
  where: ["Brazil", "multiple countries of interviewed OSS contributors (France, Germany, Canada, Hungary, Australia, Turkey, Mexico, India, US, UK, Greece, China)"]
  when: "2013-2015"
  n: 43
  sector: ["open-source"]
  sample_notes: >
    Phase I combined convenience-sample survey respondents (9 mailing lists), snowball-
    recruited interviewees, and a 21-study SLR; self-selection and social-desirability bias
    likely among volunteer respondents. Phase II used undergraduate students (mostly with
    little/no industry experience) as proxies for OSS newcomers, which limits
    generalizability to real-world volunteer contributors; only 44 of 65 initial diary
    participants met inclusion criteria (>=3 entries, code contribution).
limitation:
  primary: "Phase II generalizability is limited because participants were undergraduate students completing a course assignment (not self-motivated volunteer contributors), and the diary-based, small-sample design (43 analyzed, split across control/portal groups) supports qualitative insight rather than statistically powered causal claims about the portal's effect."
  others:
    - "Data collected 2013-2015, before GitHub/social-coding norms became dominant in OSS, so barrier prevalence may not reflect current platforms."
    - "SLR and interview coding involved subjective qualitative interpretation, mitigated only by multi-researcher discussion, not independent inter-rater reliability statistics."
    - "Self-selection and social-desirability bias likely in open-invitation survey/interview recruitment."
risk_of_bias: "medium"
relevance_to_project: >
  Directly informs SNH's model of what drives isolation vs. belonging in open-source
  communities: it operationalizes concrete, actionable social barriers (unanswered messages,
  unkind tone, absent mentors, shyness/fear, language/cultural friction) and shows that a
  lightweight structural intervention (an onboarding portal with guidance and message
  templates) measurably reduced newcomers' need for and anxiety around social contact, which
  is a directly transferable design pattern for reducing maintainer/contributor isolation
  and improving retention.
tags:
  topic: ["open-source", "community-health", "isolation", "social-support", "collaboration"]
  method: ["mixed-methods", "qualitative", "review-systematic"]
  population: ["open-source-contributors", "students"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/Overcoming Social Barriers When Contributing to Open Source Software Projects/Overcoming Social Barriers When Contributing to Open Source Software Projects.md"
  pdf: "papers/Articles/01 Articles - Extended/Overcoming Social Barriers When Contributing to Open Source Software Projects.pdf"
  notes: null

---

id: "riehle-2014-paid-vs-volunteer-work-in-open"
title: "Paid vs. Volunteer Work in Open Source"
authors:
  - "Riehle, Dirk"
  - "Riemer, Philipp"
  - "Kolassa, Carsten"
  - "Schmidt, Michael"
year: 2014
doi: "10.1109/hicss.2014.407"
venue: {type: "conference", name: "2014 47th Hawaii International Conference on System Sciences", volume: null, issue: null, pages: "3286-3295"}
citation: "Riehle et al. (2014). Paid vs. Volunteer Work in Open Source. 2014 47th Hawaii International Conference on System Sciences, 3286-3295. https://doi.org/10.1109/hicss.2014.407"
article_type: "empirical"
method: {design: "longitudinal", approach: "secondary-data", evidence_level: "moderate", preregistered: false}
gist: >
  Analyzing commit timestamps from the Linux kernel (2005-2011) and a 2008 snapshot of over
  5,000 Ohloh open-source projects (2000-2007), the authors use a conservative working-hours
  proxy (Mon-Fri, 9am-5pm local time = paid work) to estimate that roughly 50% of all open-
  source contribution has been paid corporate work for years, with the paid share flat over
  time in the broad Ohloh sample but rising then plateauing for Linux. They propose the
  ratio of paid to volunteer contributors as a practical indicator project leaders can use
  to gauge community health, noting small projects are often fully company-paid while large,
  healthy public projects sustain a 10-20% paid-developer mix alongside volunteers.
claims:
  - text: "About 50% of all open-source commits occurred during working hours: 45.00% of Linux kernel author contributions and 51.36% of committer integrations were made Mon-Fri 9am-5pm, versus 47.3% (known committers) and 55.4% (extended committers) for the 5,117-project Ohloh sample."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["collaboration"]
    predictors: ["open-source-maintenance", "organizational-culture"]
  - text: "The share of working-time (paid) contribution to the broad Ohloh project sample stayed statistically flat from 2000-2007 (F-test rejects any trend at 98% confidence) despite near-exponential growth in overall project activity, while the Linux kernel showed a clear upward trend in paid work from 2007-2010 that then plateaued."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["collaboration"]
    predictors: ["open-source-maintenance"]
  - text: "Using a conservative 95%+ working-hours threshold to classify 'paid developers,' at least 23.15% of Linux kernel authors and 11.28% of committers, and 17.97% of Ohloh extended committers, were paid; many of the smallest OSS projects were fully company-paid, while large healthy public projects (e.g. GNOME, Eclipse, KDE) maintained a 10-20% paid-developer share alongside volunteers."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["retention", "turnover"]
    predictors: ["open-source-maintenance", "organizational-culture"]
population:
  who: "Software developers/committers contributing to the Linux kernel and to a large cross-section of active open-source projects; unit of analysis is commit-level timestamps, not surveyed individuals."
  where: ["Global (contributor timezones inferred); activity strongly dominated by Western/Christian-calendar countries"]
  when: "Linux kernel: 2005-2011 commit history; Ohloh projects: 2000-2007 commit history from a 2008 database snapshot"
  n: 5117
  sector: ["open-source"]
  sample_notes: >
    Ohloh sample of 5,117 'active' projects (~30% of an estimated 18,000 active OSS projects
    circa 2007) drawn from an 8.7M-commit, 9,192-project snapshot; only 45,870 distinct
    committers, of whom just 580 (1.3%, but 8% of commits) had hand-identified timezones
    ('known committers'), with the rest timezone-imputed via a least-squares heuristic
    ('extended committers'). Paid-work status is inferred purely from commit timing, not
    verified employment records, and a bias check (t-test across activity-ranked committer
    bins) failed to reject the no-bias null but could not rule bias out.
limitation:
  primary: "Paid vs. volunteer status is inferred indirectly from whether a commit timestamp falls in a Mon-Fri 9am-5pm window, not from actual employment or compensation data, so misclassification (enthusiast paid developers working off-hours, or volunteers with flexible daytime schedules) is likely and the authors themselves call the paid-developer estimate a conservative lower bound."
  others:
    - "Ohloh data is an aging 2008 snapshot (activity through 2007) and no comparably detailed public dataset was available to update it at time of writing."
    - "The working-hours definition encodes a Western Mon-Fri workweek assumption; the analysis notes cultures with Saturday workweeks show little open-source activity, but this could still misclassify contributors elsewhere."
    - "Ohloh could not distinguish authors from committers (unlike Git-based Linux data), and timezone assignment for the majority of committers is a statistical estimate rather than a direct observation."
risk_of_bias: "medium"
relevance_to_project: >
  Offers a concrete, low-cost behavioral metric (paid/volunteer contributor ratio, derivable
  from commit timestamps) that the SNH project could adapt as an indicator of open-source
  community health and sustainability risk, complementing self-report measures of maintainer
  burnout; the finding that healthy large projects sustain ~10-20% paid contributors
  alongside volunteers gives a reference range for evaluating whether a project's
  paid/volunteer balance signals health versus over-reliance on either group.
tags:
  topic: ["open-source", "community-health", "maintainer-burnout", "methodology"]
  method: ["secondary-data", "longitudinal"]
  population: ["open-source-contributors"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/Paid vs Volunteer Work in Open Source/Paid vs Volunteer Work in Open Source.md"
  pdf: "papers/Articles/01 Articles - Extended/Paid vs Volunteer Work in Open Source.pdf"
  notes: null

---

id: "lerner-2002-some-simple-economics-of-open-source"
title: "Some Simple Economics of Open Source"
authors:
  - "Lerner, Josh"
  - "Tirole, Jean"
year: 2002
doi: "10.1111/1467-6451.00174"
venue: {type: "journal", name: "The Journal of Industrial Economics", volume: 50, issue: 2, pages: "197-234"}
citation: "Lerner et al. (2002). Some Simple Economics of Open Source. The Journal of Industrial Economics, 50(2), 197-234. https://doi.org/10.1111/1467-6451.00174"
article_type: "theory"
method: {design: "case-study", approach: "analytical", evidence_level: "low", preregistered: false}
gist: >
  This 2002 paper by Lerner and Tirole uses labor-economics 'career concerns' theory and
  industrial-organization theory to explain why programmers contribute unpaid labor to open-
  source projects (Apache, Linux, Perl, Sendmail), arguing that the visibility of individual
  code contributions functions as a signal of talent that yields delayed career and
  reputational payoffs. Drawing on four project case studies (interviews plus secondary
  contributor-distribution data), the authors show open-source participation is highly
  unequal, with a small 'elite' core producing most of the code, and that early, prominent
  contributors frequently converted this signaling capital into commercial leadership roles.
  It offers an economic account of why decentralized volunteer communities sustain
  themselves and which governance features (modularity, credible leadership, transparent
  decision rules) prevent them from fragmenting or 'forking'.
claims:
  - text: "Contribution to open-source code is extremely concentrated: in an analysis of 25 million lines of code across 3,149 projects (~13,000 contributors), more than three-quarters of contributors made only one contribution and only 1 in 25 had more than five, yet the top decile of contributors accounted for 72% of all code contributed and the top two deciles for 81%."
    evidence: "secondary-data"
    support_strength: "low-to-moderate"
    outcomes: ["collaboration"]
    predictors: ["network-structure", "community-engagement", "open-source-maintenance"]
  - text: "Apache's own developer community shows the same elitist pattern: the top 15 developers on the core Apache developers mailing list contributed 83% to 91% of changes, whereas bug/problem reports (a lower-effort form of participation) were distributed far less unequally."
    evidence: "case-study"
    support_strength: "low"
    outcomes: ["collaboration"]
    predictors: ["open-source-maintenance", "network-structure"]
  - text: "Prominent early open-source contributors frequently converted reputation built through visible, individually-attributable contributions into subsequent commercial roles (e.g., founding or leading venture-backed companies such as Sendmail Inc., Collab.Net, Sun Microsystems, Cygnus Solutions), consistent with a signaling/career-concerns account of participation motives rather than pure altruism."
    evidence: "case-study"
    support_strength: "weak"
    outcomes: ["retention", "job-engagement"]
    predictors: ["community-engagement", "open-source-maintenance", "leadership-style"]
population:
  who: "Four purposively selected, high-profile open source software projects (Apache, Linux, Perl, Sendmail) and their founders/lead maintainers, studied via document review and interviews, plus secondary quantitative data on broader open-source contributor populations (e.g., a ~13,000-contributor, 3,149-project analysis and a study of Linux mailing-list posters)."
  where: ["United States", "Europe"]
  when: "Case interviews and analysis conducted circa 1999-2000; secondary datasets from 1999-2000; published 2002"
  n: null
  sector: ["open-source", "software-industry"]
  sample_notes: >
    Non-random, small sample of four projects chosen because they were already
    successful/prominent; the authors explicitly caution these are 'observations based on a
    small sample of successful projects' and that determining what causes success versus
    failure in an informal setting is difficult. Secondary contributor-distribution figures
    come from working papers with response-rate/representativeness not independently
    verifiable in this text.
limitation:
  primary: "The evidence base is four purposively selected, already-successful open source projects examined qualitatively, not a representative or random sample with variation in outcomes, so the proposed economic mechanisms (signaling, career concerns) are illustrated rather than causally tested."
  others:
    - "The paper is explicitly exploratory/agenda-setting theory-building, declining to construct formal statistical models or test hypotheses on large samples."
    - "Key contribution-inequality statistics are drawn from unpublished working papers (Ghosh & Prakash 2000; Dempsey et al. 1999) whose methodology is not independently verifiable here."
    - "Written in 2000-2002, prior to major shifts in OSS tooling, governance (e.g., GitHub-era platforms), and corporate open-source practice, limiting contemporary generalizability."
risk_of_bias: "high"
relevance_to_project: >
  The paper's signaling/career-concerns framework (visibility of contribution, peer
  recognition, 'ego gratification' as a delayed reward) offers a candidate mechanism for why
  remote and open-source contributors sustain unpaid or discretionary engagement, directly
  relevant to designing recognition and visibility features that support community health.
  Its finding of extreme core-periphery contribution inequality (a small elite doing most of
  the work) is directly relevant to understanding and mitigating maintainer burnout risk
  concentration in open-source communities.
tags:
  topic: ["open-source", "maintainer-burnout", "community-health", "collaboration"]
  method: ["case-study", "secondary-data"]
  population: ["open-source-contributors", "software-industry"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/Some Simple Economics of Open Source/Some Simple Economics of Open Source.md"
  pdf: "papers/Articles/01 Articles - Extended/Some Simple Economics of Open Source.pdf"
  notes: null

---

id: "cotton-2015-stronger-than-fear-mental-health-in"
title: "Stronger than fear: Mental health in the open"
authors:
  - "Cotton, Ben"
year: 2015
doi: null
venue: {type: "other", name: "Opensource.com", volume: null, issue: null, pages: null}
citation: "Cotton (2015). Stronger than fear: Mental health in the open. Opensource.com."
article_type: "commentary"
method: {design: "case-study", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  This opensource.com feature profiles Ed Finkler, an open-source developer who in 2013
  founded the Open Sourcing Mental Illness (OSMI) campaign after realizing developers, like
  everyone else, struggle silently with mental health issues. The article describes how
  Finkler's personal conference talks prompted attendees to disclose their own struggles,
  how OSMI's 2015 fundraiser quickly funded professional development of a Creative-Commons-
  licensed workplace mental-health guide, and explicitly notes that little formal research
  exists on how developer work influences (and is influenced by) mental health.
claims:
  - text: "Finkler founded the OSMI campaign in 2013 after his personal conference talks about his own mental illness repeatedly prompted attendees to disclose their own mental health struggles, indicating unmet need for open discussion in developer communities."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["mental-health", "isolation"]
    predictors: ["community-engagement"]
  - text: "The article states roughly 20% of the U.S. population has a mental health disorder at any given time, but notes little research has specifically examined how developers' work influences, and is influenced by, their mental health."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["mental-health"]
    predictors: ["open-source-maintenance"]
  - text: "OSMI's 2015 Indiegogo fundraiser met its $5,000 goal within two hours, with proceeds funding conference travel and a mental-health-professional-authored guide for making tech workplaces safer, released under a Creative Commons license."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["mental-health"]
    predictors: ["community-engagement", "intervention"]
population:
  who: "Single case profile of open-source community mental-health advocate Ed Finkler and the OSMI (Open Sourcing Mental Illness) campaign he founded, based on an interview; no primary research sample."
  where: ["United States"]
  when: "2013-2015"
  n: null
  sector: ["open-source"]
  sample_notes: >
    Journalistic feature/interview piece; single informant (Finkler) plus a few reader
    comments; no systematic sampling or data collection.
limitation:
  primary: "The piece is a journalistic profile and interview, not a research study — it reports one advocate's anecdotal experience and opinions rather than systematic data on developer mental health."
  others:
    - "The '20% of U.S. population has a mental health disorder' statistic is asserted without citation or methodology."
    - "Single-informant perspective with no independent verification of claims made about OSMI's reach or impact."
risk_of_bias: "high"
relevance_to_project: >
  Documents an early (2013-2015) grassroots effort in the open-source community to surface
  and destigmatize developer mental health struggles, and explicitly flags the absence of
  research on how open-source/developer work affects mental health — directly motivating the
  SNH project's evidence-building agenda for maintainer and remote-worker wellbeing.
tags:
  topic: ["open-source", "mental-health", "maintainer-burnout", "community-health"]
  method: ["case-study"]
  population: ["open-source-contributors", "software-developers"]
source:
  markdown: "Papers_Data/Articles/MD/Stronger than Fear Mental Health in the Open/Stronger than Fear Mental Health in the Open.md"
  pdf: "papers/Articles/Stronger than Fear Mental Health in the Open.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "kettanaito-2022-the-dark-side-of-open-source"
title: "The Dark Side of Open Source"
authors:
  - "Kettanaito"
year: 2022
doi: null
venue: {type: "other", name: "kettanaito.com (personal blog)", volume: null, issue: null, pages: null}
citation: "Kettanaito (2022). The Dark Side of Open Source. kettanaito.com (personal blog)."
article_type: "commentary"
method: {design: "case-study", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  Personal essay by a self-described open-source library author describing the hidden costs
  of maintaining a popular OSS project: the near-total absence of sustainable financial
  support for maintainers, the pull toward turning projects into commercial products, and
  burnout from blurred boundaries between open-source work and personal life. The author
  argues maintainers should plan an exit/maintenance strategy early and impose strict daily
  time limits on OSS work to protect mental health and relationships.
claims:
  - text: "The author reports experiencing burnout and anxiety while sustaining a popular open-source project without adequate boundaries or compensation, including panic-like reactions to notifications of new issues being reported on his projects."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "anxiety", "mental-health"]
    predictors: ["workload", "boundary-management"]
  - text: "The author argues that voluntary financial sponsorship almost never sustains open-source maintainers, claiming that in the JavaScript ecosystem nearly all 'successful' projects survive only by being acquihired, corporatized, or converted into paid products rather than by donations."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "retention"]
    predictors: ["open-source-maintenance", "organizational-culture"]
  - text: "The author recommends maintainers set explicit daily time limits on open-source contribution (e.g., a fixed window after work) and consciously protect personal and family time, describing this boundary-setting as the key preventive measure against overwork-driven burnout."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "work-life-balance"]
    predictors: ["boundary-management", "autonomy"]
population:
  who: "The author himself, a solo open-source JavaScript library author/maintainer, writing a first-person reflective account generalizing to open-source maintainers broadly"
  where: []
  when: null
  n: 1
  sector: ["open-source"]
  sample_notes: >
    N=1 personal narrative essay; no systematic sample, survey, or data collection.
    Reflections are drawn entirely from the author's own experience as a JavaScript open-
    source library maintainer, published as a blog post dated 13 June 2022.
limitation:
  primary: "Entirely anecdotal, first-person opinion piece with no data collection, sample, or empirical methodology; claims are unverifiable generalizations drawn from one maintainer's personal experience."
  others:
    - "No citations or references to existing research on open-source sustainability or maintainer burnout"
    - "Focused narrowly on the JavaScript/npm open-source ecosystem, limiting generalizability to other open-source communities or sectors"
risk_of_bias: "high"
relevance_to_project: >
  Offers first-person qualitative testimony of the mechanisms the SNH project associates
  with maintainer burnout, uncompensated workload, blurred work/life boundaries, and anxiety
  triggered by user issue reports, and proposes a concrete self-help intervention (explicit
  time-boxing of open-source work) that could inform design recommendations for sustaining
  open-source maintainer wellbeing.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "work-life-balance", "mental-health"]
  method: ["case-study"]
  population: ["open-source-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/The Dark Side of Open Source/The Dark Side of Open Source.md"
  pdf: "papers/Articles/The Dark Side of Open Source.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "smith-2024-the-developer-crisis-mental-health-burnout"
title: "The Developer Crisis: Mental Health, Burnout, and Retention"
authors:
  - "Smith, Craig"
year: 2024
doi: null
venue: {type: "other", name: "The New Stack", volume: null, issue: null, pages: null}
citation: "Smith (2024). The Developer Crisis: Mental Health, Burnout, and Retention. The New Stack."
article_type: "commentary"
method: {design: "theory", approach: "secondary-data", evidence_level: "weak", preregistered: false}
gist: >
  A trade-publication opinion piece arguing that UK software companies risk losing
  developers to burnout and turnover unless they address unpaid overtime, meeting overload,
  rigid training programs, and tedious backend work. It strings together burnout, quit-
  intention, and productivity statistics from third-party surveys (JetBrains, Stack
  Overflow, McKinsey, standout-cv, ITPro) to make the case for flexible schedules, feedback
  loops, and tooling investment, but conducts no original research of its own.
claims:
  - text: "67% of developers have left a job, or know someone who has, specifically to avoid pressure to minimize deployment errors; among those who stayed, 28% reported lowered productivity due to excessive stress."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["turnover", "stress", "productivity"]
    predictors: ["workload", "technostress"]
  - text: "Nearly three-quarters of developers report having experienced burnout on the job, cited from JetBrains' 2023 developer ecosystem survey."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["burnout"]
    predictors: ["workload", "technostress"]
  - text: "47% of burned-out developers use self-help apps to track their health, and asking developers directly how they spend their time can shorten project lead times by up to 40% (cited McKinsey figure)."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["burnout", "productivity"]
    predictors: ["intervention", "workload"]
population:
  who: "Software developers generally, with a UK-market framing (referencing UK tech vacancy projections); population is characterized only via statistics borrowed from other surveys, not sampled directly by this article."
  where: ["United Kingdom", "unspecified/global (per cited surveys)"]
  when: "2023-2024 (cited survey data)"
  n: null
  sector: ["technology", "software-development"]
  sample_notes: >
    This is a secondary/opinion piece; it has no sample of its own. It aggregates statistics
    from at least six external sources (JetBrains DevEcosystem 2023, Stack Overflow 2023,
    McKinsey, ITPro, standout-cv, worklife.news) without stating their sample sizes,
    sampling methods, or exact dates, so figures cannot be independently verified within
    this document.
limitation:
  primary: "The piece is an opinion/advisory trade article, not original research: it aggregates statistics from multiple third-party surveys without describing their methodology, sample size, or exact survey date, so the cited figures are unverifiable from this document alone."
  others:
    - "Author is an ecommerce technology consultant, not a researcher, writing for a sponsor-supported trade publication (The New Stack)"
    - "Recommendations (reduce meetings, flexible training, offload menial coding tasks) are prescriptive assertions not tested for effectiveness in this piece"
    - "No discussion of causality, confounds, or generalizability of the borrowed statistics"
risk_of_bias: "high"
relevance_to_project: >
  Useful as a source of widely-circulated industry burnout and turnover figures for software
  developers (burnout prevalence, overtime-driven quitting, self-help app adoption) that can
  motivate the SNH project's developer/maintainer burnout framing, but each figure should be
  traced back to and verified against its primary survey (e.g., JetBrains DevEcosystem,
  Stack Overflow Developer Survey) before being cited as evidence.
tags:
  topic: ["burnout", "job-satisfaction", "wellbeing", "technostress"]
  method: ["secondary-data", "survey"]
  population: ["software-developers", "tech-industry"]
source:
  markdown: "Papers_Data/Articles/MD/The Developer Crisis Mental Health Burnout and Retention/The Developer Crisis Mental Health Burnout and Retention.md"
  pdf: "papers/Articles/The Developer Crisis Mental Health Burnout and Retention.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "bekahhw-2024-the-hidden-cost-of-free-why"
title: "The Hidden Cost of Free: Why Open Source Sustainability Matters"
authors:
  - "BekahHW"
year: 2024
doi: null
venue: {type: "other", name: "OpenSauced Blog", volume: null, issue: null, pages: null}
citation: "BekahHW (2024). The Hidden Cost of Free: Why Open Source Sustainability Matters. OpenSauced Blog."
article_type: "commentary"
method: {design: "theory", approach: "analytical", evidence_level: "weak", preregistered: false}
gist: >
  This OpenSauced blog post frames open-source software sustainability as a tragedy-of-the-
  commons problem: companies and users capture enormous value from OSS (citing an HBS
  estimate of $8.8 trillion in demand-side value versus $4.15 billion in supply-side value)
  while maintenance work falls on a small, often unpaid group of maintainers. Drawing on
  Nadia Eghbal's 'Working in Public' and the 2024 Tidelift State of the Open Source
  Maintainer Report (60% of maintainers unpaid, preference for recurring over one-time
  income, paid maintainers more likely to follow security practices), the piece argues that
  free-riding and lack of compensation drive maintainer burnout, security risk, and project
  abandonment, and proposes direct-payment models like Sentry's OSS Pledge as a remedy.
claims:
  - text: "Citing an HBS working paper (Hoffmann, Nagle & Zhou), the demand-side value of widely-used open source software is estimated at $8.8 trillion versus a supply-side value of $4.15 billion, and 96% of that demand-side value is created by only 5% of OSS developers."
    evidence: "cross-sectional"
    support_strength: "low"
    outcomes: ["productivity"]
    predictors: ["open-source-maintenance", "network-structure"]
  - text: "The 2024 Tidelift State of the Open Source Maintainer Report found that 60% of maintainers remain unpaid for their work, and that paid maintainers are significantly more likely to implement critical security practices than unpaid ones."
    evidence: "cross-sectional"
    support_strength: "low"
    outcomes: ["burnout", "retention"]
    predictors: ["open-source-maintenance", "organizational-culture"]
  - text: "The same Tidelift report found maintainers overwhelmingly prefer predictable, recurring income over one-time payments, motivating direct-payment interventions such as Sentry's OSS Pledge, which asks companies to pay a minimum of $2,000 per full-time-equivalent developer per year to maintainers of their choosing."
    evidence: "cross-sectional"
    support_strength: "weak"
    outcomes: ["burnout", "job-satisfaction"]
    predictors: ["intervention", "open-source-maintenance"]
population:
  who: "Open-source software maintainers and the companies/users who depend on their work, discussed through secondary sources rather than an original sample."
  where: []
  when: "2024"
  n: null
  sector: ["technology"]
  sample_notes: >
    Blog essay synthesizing secondary sources (an HBS working paper on OSS value, the 2024
    Tidelift State of the Open Source Maintainer Report, Nadia Eghbal's 'Working in Public',
    and Linux Foundation reports); no original data collection, sample, or methodology of
    its own.
limitation:
  primary: "This is an advocacy/opinion blog post rather than primary research: it synthesizes and paraphrases secondary reports without describing their methodology, sampling, or effect-size confidence, so the cited statistics cannot be independently verified from this document."
  others:
    - "Sources are chosen illustratively to support an argument rather than through a systematic search"
    - "Author is Developer Experience Lead at OpenSauced, a company with a commercial interest in open-source analytics and community narratives"
    - "No original quantitative or qualitative data collected by the author"
risk_of_bias: "high"
relevance_to_project: >
  Articulates a tragedy-of-the-commons mechanism (free-riding, uncompensated labor,
  concentrated maintenance burden) linking open-source sustainability to maintainer burnout
  and security risk, and surfaces survey evidence (60% unpaid; preference for recurring
  income) and a concrete compensation-based intervention (Sentry's OSS Pledge) relevant to
  the project's maintainer-burnout prevention and sustainability-intervention design
  questions.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "community-health"]
  method: ["theory"]
  population: ["open-source-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/The Hidden Cost of Free Why Open Source Sustainability Matters/The Hidden Cost of Free Why Open Source Sustainability Matters.md"
  pdf: "papers/Articles/The Hidden Cost of Free Why Open Source Sustainability Matters.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "lee-2006-the-human-infrastructure-of-cyberinfrastructure"
title: "The human infrastructure of cyberinfrastructure"
authors:
  - "Lee, Charlotte P."
  - "Dourish, Paul"
  - "Mark, Gloria"
year: 2006
doi: "10.1145/1180875.1180950"
venue: {type: "conference", name: "Proceedings of the 2006 20th anniversary conference on Computer supported cooperative work", volume: null, issue: null, pages: "483-492"}
citation: "Lee et al. (2006). The human infrastructure of cyberinfrastructure. Proceedings of the 2006 20th anniversary conference on Computer supported cooperative work, 483-492. https://doi.org/10.1145/1180875.1180950"
article_type: "empirical"
method: {design: "case-study", approach: "ethnography", evidence_level: "low-to-moderate", preregistered: false}
gist: >
  Based on an 18-month ethnography and 20 in-depth interviews within FBIRN, a 13-institution
  NIH-funded biomedical cyberinfrastructure consortium, the paper introduces 'human
  infrastructure' to argue that large-scale distributed scientific collaboration is
  accomplished through overlapping, fuzzy-bordered working groups, traditional site-based
  labs, and personal networks-not through clean 'distributed teams.' It finds that ambiguous
  group membership is pervasive yet does not prevent the collaboration from functioning,
  challenging team-centric accounts of distributed work.
claims:
  - text: "In interviews with 20 participants across 10 institutions, many FBIRN members did not know whether they were formally part of a given working group or task force, or whether a task force they had joined was still active, showing persistently fuzzy team boundaries and membership in a large distributed science collaboration."
    evidence: "case-study"
    support_strength: "low"
    outcomes: ["collaboration", "sense-of-belonging"]
    predictors: ["network-structure", "team-cohesion"]
  - text: "Beyond formal working groups, participants relied heavily on personal ('intensional') networks-relationships built through prior jobs, conferences, and personal contacts-for information, help-seeking, and recruitment onto the project; more senior researchers named substantially more collaborators than junior ones."
    evidence: "case-study"
    support_strength: "low"
    outcomes: ["collaboration", "help-seeking"]
    predictors: ["network-structure", "peer-mentoring"]
  - text: "Traditional, place-based organizations (university labs, departments, hospitals) remained indispensable to the distributed effort-supplying equipment, staff, IRB approval, and local coordination-even as work spanned 13+ institutions, and managers in supervisory roles reported being unable to hold collaborators accountable because they did not control their pay, undermining a pure 'virtual organization' or 'distributed team' account of big-science collaboration."
    evidence: "case-study"
    support_strength: "low"
    outcomes: ["collaboration", "productivity"]
    predictors: ["organizational-culture", "network-structure"]
population:
  who: "FBIRN (Function Biomedical Informatics Research Network) participants: 20 in-depth interviewees (site PIs/co-PIs, engineers/developers, neuroscience researchers, working group chairs, a project manager, a grad student, a postdoc, a research assistant) drawn from 10 of the consortium's 13 US partner institutions, plus 18 months of ethnographic participant observation at FBIRN meetings."
  where: ["United States"]
  when: "circa 2004-2006 (18-month ethnographic engagement; published at CSCW 2006)"
  n: 20
  sector: ["academic-research", "biomedical-research"]
  sample_notes: >
    Interviewees spanned seniority levels and 10 of 13 partner institutions; researchers
    observed 36 biweekly meetings plus teleconferences, videoconferences, and all-hands
    meetings over 18 months and reviewed email list traffic; no formal response rate
    reported; pseudonyms used to protect identity.
limitation:
  primary: "Single case study of one biomedical cyberinfrastructure consortium (FBIRN) based on 20 purposively selected interviewees, so generalizability to other distributed collaborations-including open-source or non-scientific remote-work settings-is uncertain."
  others:
    - "No comparison against a more formally team-structured cyberinfrastructure project to isolate what 'human infrastructure' adds beyond conventional organization."
    - "Relies on self-report interview and observational data interpreted by the ethnographers, with no stated formal coding scheme or inter-rater reliability check."
    - "Data reflect a mid-2000s institutional and technology context (teleconferencing, email lists) that may not map directly onto current remote-collaboration tooling."
risk_of_bias: "medium"
relevance_to_project: >
  Provides grounded qualitative evidence that in large distributed technical collaborations,
  informal personal networks-not formal team or org-chart structure-are a primary channel
  for help-seeking, information flow, and continued participation, and that ambiguous/fuzzy
  membership does not by itself prevent effective collaboration. This is directly relevant
  to how SNH should model belonging and support in remote and open-source communities:
  network-based rather than team-based measures of connection may better predict who gets
  help and who doesn't.
tags:
  topic: ["collaboration", "community-health", "remote-work"]
  method: ["qualitative", "methodology"]
  population: ["researchers", "distributed-teams"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/The Human Infrastructure of Cyberinfrastructure/The Human Infrastructure of Cyberinfrastructure.md"
  pdf: "papers/Articles/01 Articles - Extended/The Human Infrastructure of Cyberinfrastructure.pdf"
  notes: null

---

id: "bekahhw-nd-the-lonely-journey-of-open-source"
title: "The Lonely Journey of Open-Source Maintainers: A Call for Connection and Recognition"
authors:
  - "BekahHW"
year: null
doi: null
venue: {type: "other", name: "OpenSauced (Insights blog)", volume: null, issue: null, pages: null}
citation: "BekahHW (None). The Lonely Journey of Open-Source Maintainers: A Call for Connection and Recognition. OpenSauced (Insights blog)."
article_type: "commentary"
method: {design: "theory", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  A developer-relations blog post argues that loneliness is a major, under-discussed driver
  of open-source maintainer burnout, compounding with invisible labor (community management,
  documentation, issue triage) and lack of user recognition. Drawing on the author's own
  experience and quotes from two other maintainers, it proposes community-building,
  recruiting the 'right' contributors, and public storytelling/recognition as informal
  remedies for maintainer isolation.
claims:
  - text: "The author argues loneliness is one of the major contributors to maintainer burnout, alongside 'contribution farming,' low-quality/spammy PRs, and the 'invisible labor' of community management, documentation, and issue triaging that solo maintainers absorb."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["burnout", "loneliness"]
    predictors: ["isolation", "workload"]
  - text: "Anecdotal accounts from maintainers (e.g., Adriano Raiano, Sean Walberg) are used to argue that having the right-fit contributors reduces maintainer burden, and that public recognition and 'sharing your story' increase feelings of being seen and belonging, which the author claims decreases pervasive maintainer loneliness."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["sense-of-belonging", "loneliness", "burnout"]
    predictors: ["social-support", "community-engagement", "peer-mentoring"]
population:
  who: "Open-source project maintainers, especially solo maintainers, characterized through the author's own experience and anecdotal quotes from two named maintainers found in their public LinkedIn/blog posts."
  where: []
  when: null
  n: null
  sector: ["open-source"]
  sample_notes: >
    No systematic sample or data collection; illustrative quotes drawn from two individuals'
    public writings plus the author's first-person observations as a Developer Experience
    lead at OpenSauced, a GitHub analytics/community tooling company.
limitation:
  primary: "This is an opinion/advocacy blog post with no empirical data collection, systematic sampling, or citations to research literature; its claims about loneliness and burnout rest entirely on the author's personal observations and a handful of anecdotal quotes."
  others:
    - "No definitions or measurement instruments for 'loneliness,' 'burnout,' or 'belonging' are given, and no outcome data are reported."
    - "Published on the blog of OpenSauced, a company whose product is built around maintainer/contributor engagement and recognition, a potential source of promotional bias."
risk_of_bias: "high"
relevance_to_project: >
  Offers a maintainer's-eye-view articulation of a loneliness-to-burnout pathway in open-
  source work and proposes recognition, storytelling, and peer connection as informal
  interventions—useful for generating hypotheses about isolation, invisible labor, and
  social support mechanisms among open-source maintainers, though it provides no empirical
  evidence to support them.
tags:
  topic: ["open-source", "maintainer-burnout", "loneliness", "community-health", "burnout"]
  method: ["theory"]
  population: ["open-source-maintainers", "solo-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/The Lonely Journey of Open-Source Maintainers A Call for Connection and Recognition/The Lonely Journey of Open-Source Maintainers A Call for Connection and Recognition.md"
  pdf: "papers/Articles/The Lonely Journey of Open-Source Maintainers A Call for Connection and Recognition.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "guizani-2021-the-long-road-ahead-ongoing-challenges"
title: "The Long Road Ahead: Ongoing Challenges in Contributing to Large OSS Organizations and What to Do"
authors:
  - "Guizani, Mariam"
  - "Chatterjee, Amreeta"
  - "Trinkenreich, Bianca"
  - "May, Mary Evelyn"
  - "Noa-Guevara, Geraldine J."
  - "Russell, Liam James"
  - "Cuevas Zambrano, Griselda G."
  - "Izquierdo-Cortazar, Daniel"
  - "Steinmacher, Igor"
  - "Gerosa, Marco A."
  - "Sarma, Anita"
year: 2021
doi: "10.1145/3479551"
venue: {type: "journal", name: "Proceedings of the ACM on Human-Computer Interaction", volume: 5, issue: "CSCW2", pages: "1-30"}
citation: "Guizani et al. (2021). The Long Road Ahead: Ongoing Challenges in Contributing to Large OSS Organizations and What to Do. Proceedings of the ACM on Human-Computer Interaction, 5(CSCW2), 1-30. https://doi.org/10.1145/3479551"
article_type: "empirical"
method: {design: "mixed-methods", approach: "survey", evidence_level: "moderate", preregistered: false}
gist: >
  Surveying 624 Apache Software Foundation contributors and conducting 11 follow-up
  interviews, this study builds a grounded-theory conceptual model of 88 ongoing challenges
  (beyond the newcomer stage) that contributors face at the Individual, Project, and
  Foundation levels, spanning Process, Technical, and Social dimensions, plus 48 community-
  recommended mitigation strategies. It finds that in a large, mature, federated OSS
  organization, Process (33) and Social (31) challenges concentrated at the Foundation (33)
  and Project (34) levels dominate over Technical and Individual-level issues, and that 68%
  of identified challenges were not previously documented in the newcomer-barrier
  literature. The paper argues organization-level (not just project-level) governance,
  communication norms, and toxic-environment mitigation are essential to sustaining large
  peer-production communities.
claims:
  - text: "Contributors reported far more Process (33 challenges) and Social (31 challenges) issues than Technical (24), concentrated at the Foundation (33) and Project (34) levels rather than the Individual level (21); at the Foundation level, process-related challenges predominated, followed by social, then technical."
    evidence: "mixed-methods"
    support_strength: "moderate"
    outcomes: ["collaboration", "burnout"]
    predictors: ["organizational-culture", "leadership-style"]
  - text: "Toxic/unwelcoming environment and communication challenges accounted for 74% of all social challenges reported; women and other minority contributors described being overwhelmed and silenced on foundation-wide mailing lists (e.g., one female committer reported never posting to the members list after seeing hostile discussion), and hierarchical leadership was seen as discriminating against less-tenured contributors."
    evidence: "mixed-methods"
    support_strength: "moderate"
    outcomes: ["isolation", "sense-of-belonging", "turnover"]
    predictors: ["psychological-safety", "inclusiveness", "leadership-style"]
  - text: "68% of the 88 identified challenges were not reported in prior OSS newcomer-barrier literature, with the largest gaps in Process (79% novel) and Social (74% novel) categories and concentrated at the Foundation level (88% of novel challenges originated there), indicating organization-level challenges are a distinct, under-studied layer beyond project-level onboarding barriers."
    evidence: "mixed-methods"
    support_strength: "moderate"
    outcomes: ["turnover", "retention"]
    predictors: ["organizational-culture", "network-structure"]
population:
  who: "Contributors to the Apache Software Foundation (ASF), a large federated OSS organization (~460k people, 350+ projects); 624 survey respondents, of whom 223 reported facing ongoing challenges (86.5% men, 77.1% with 3+ years experience, mostly volunteers), plus 11 semi-structured interview participants drawn from a demographically balanced subset"
  where: ["United States", "Italy", "Russia", "Germany", "and other countries across 6 continents (35 countries total among survey respondents)"]
  when: "survey open 45 days; study conducted circa 2020-2021 (published Oct 2021)"
  n: 624
  sector: ["open-source"]
  sample_notes: >
    8.5% survey response rate (624/~7500 community members); analysis focused on the 223
    respondents who reported challenges; interview sample (11 of 20 invited, from 69 who
    consented) intentionally balanced for demographics; findings validated via two-step
    member checking with interviewees and the ASF Diversity & Inclusion committee; self-
    selected, English-proficient, senior-skewed sample likely underrepresents lurkers, early
    dropouts, and non-English speakers.
limitation:
  primary: "Sample skews toward senior, male, English-confident, US/Europe-based contributors who remained engaged enough to respond to a foundation-wide survey, likely undercounting the challenges of those who already disengaged or never felt comfortable enough to participate."
  others:
    - "Single-organization case study (ASF only), so the specific mix and prevalence of challenges may not generalize to other OSS foundations with different governance models."
    - "Qualitative coding and challenge/level categorization involved researcher judgment (e.g., inferring 'level' when not explicitly stated), introducing some subjectivity despite negotiated-agreement procedures."
    - "8.5% survey response rate limits confidence that reported challenge prevalence reflects the full ASF contributor base."
risk_of_bias: "medium"
relevance_to_project: >
  Provides an empirically grounded taxonomy of organization-level (not just project-level)
  social and process challenges in large OSS communities -- toxic/unwelcoming environments,
  communication-channel fragmentation, hierarchical discrimination, and governance opacity
  -- directly informing SNH's model of what erodes belonging and drives turnover in open-
  source maintainer communities, plus 48 community-sourced mitigation strategies (e.g.,
  rethinking veto-based voting, minority-focused meetings, clearer communication norms) that
  could inform intervention design.
tags:
  topic: ["open-source", "community-health", "maintainer-burnout", "psychological-safety", "collaboration"]
  method: ["survey", "qualitative", "mixed-methods"]
  population: ["open-source-contributors"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/The Long Road Ahead Ongoing Challenges in Contributing to Large OSS Organizations and What to Do/The Long Road Ahead Ongoing Challenges in Contributing to Large OSS Organizations and What to Do.md"
  pdf: "papers/Articles/01 Articles - Extended/The Long Road Ahead Ongoing Challenges in Contributing to Large OSS Organizations and What to Do.pdf"
  notes: null

---

id: "bekahhw-2024-the-silent-crisis-in-open-source"
title: "The Silent Crisis in Open Source: When Maintainers Walk Away"
authors:
  - "BekahHW"
year: 2024
doi: null
venue: {type: "other", name: "OpenSauced Blog", volume: null, issue: null, pages: null}
citation: "BekahHW (2024). The Silent Crisis in Open Source: When Maintainers Walk Away. OpenSauced Blog."
article_type: "commentary"
method: {design: "theory", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  This OpenSauced blog post uses the 2022 departure of node-pre-gyp maintainer Dane
  Springmeyer as a case to argue that open source projects face a 'silent crisis' of
  maintainer attrition driven by burnout, loneliness, and lack of institutional support. It
  proposes two quantitative proxies for project vulnerability -- the Lottery Factor
  (dependency concentration among top contributors) and Contributor Confidence (likelihood
  that stargazers/forkers return to contribute) -- and calls for sustainable funding,
  succession planning, and community health metrics as mitigations.
claims:
  - text: "A project is considered vulnerable by the Lottery Factor metric if two or fewer contributors account for 50% or more of the project's pull request contributions, indicating a single point of failure risk."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["turnover", "collaboration"]
    predictors: ["open-source-maintenance", "network-structure"]
  - text: "The Contributor Confidence metric predicts the likelihood that users who star or fork a repository return to make contributions; a score in the 30-40% range is described as indicating a healthy, active project."
    evidence: "theory"
    support_strength: "speculative"
    outcomes: ["retention", "collaboration"]
    predictors: ["community-engagement", "sense-of-belonging"]
  - text: "The author frames maintainer departures (e.g., node-pre-gyp, Faker.js) as driven by burnout, loneliness, and an unsustainable 'free labor' model, and argues this causes loss of institutional knowledge, security vulnerabilities, and cascading risk to dependent projects."
    evidence: "case-study"
    support_strength: "weak"
    outcomes: ["burnout", "turnover", "isolation"]
    predictors: ["workload", "social-support", "open-source-maintenance"]
population:
  who: "Not a research sample; a practitioner blog post illustrated by anecdotal cases of individual open source maintainers (e.g., Dane Springmeyer of node-pre-gyp, Marak Squires of Faker.js)."
  where: []
  when: "2024"
  n: null
  sector: ["open-source"]
  sample_notes: >
    No systematic data collection; single case anecdote plus references to two proprietary
    OpenSauced platform metrics without validation data, methodology, or citations to peer-
    reviewed sources.
limitation:
  primary: "No empirical evidence, data, or methodology is presented; claims about burnout, loneliness, and metric validity are asserted rather than tested or sourced."
  others:
    - "Promotes the author's own company's (OpenSauced) proprietary metrics without independent validation."
    - "Relies on a single anecdotal case (node-pre-gyp) generalized to the whole open source ecosystem."
risk_of_bias: "high"
relevance_to_project: >
  Illustrates practitioner-level framing of maintainer burnout and loneliness as a social-
  network-health problem in open source, and surfaces two candidate operational metrics
  (Lottery Factor, Contributor Confidence) that could inform SNH measures of community
  concentration risk and engagement health, though neither is empirically validated here.
tags:
  topic: ["open-source", "maintainer-burnout", "community-health", "burnout"]
  method: ["theory"]
  population: ["open-source"]
source:
  markdown: "Papers_Data/Articles/MD/The Silent Crisis in Open Source When Maintainers Walk Away/The Silent Crisis in Open Source When Maintainers Walk Away.md"
  pdf: "papers/Articles/The Silent Crisis in Open Source When Maintainers Walk Away.pdf"
  notes: "no-doi: web article / no registered DOI found"

---

id: "riehle-2012-the-single-vendor-commercial-open-course"
title: "The single-vendor commercial open course business model"
authors:
  - "Riehle, Dirk"
year: 2012
doi: "10.1007/s10257-010-0149-x"
venue: {type: "journal", name: "Information Systems and e-Business Management", volume: 10, issue: 1, pages: "5-17"}
citation: "Riehle (2012). The single-vendor commercial open course business model. Information Systems and e-Business Management, 10(1), 5-17. https://doi.org/10.1007/s10257-010-0149-x"
article_type: "theory"
method: {design: "theory", approach: "secondary-data", evidence_level: "weak", preregistered: false}
gist: >
  Riehle synthesizes public statements, interviews, and presentations by practitioners at
  single-vendor commercial open source firms (e.g., MySQL, SugarCRM, Jaspersoft, Alfresco)
  into a comprehensive account of how such firms build and monetize an open source project
  they alone control. The central argument is that an engaged, self-supporting user
  community is the core business asset: it lowers customer acquisition cost, produces
  credible peer marketing, feeds product and engineering innovation, and absorbs most
  support burden through community self-help, all while the firm withholds full utility or
  operational comfort for paying customers. For SNH, the paper is a firm-level account of
  how organizations deliberately cultivate community engagement and peer support as a
  commercial resource, illuminating the incentive structures maintainer communities operate
  under.
claims:
  - text: "Conversion rates from non-paying open source user to paying customer are commonly only 0.5-2% for single-vendor commercial open source firms, per practitioner-reported figures (Taylor 2009), meaning the vast majority of the engaged community never becomes a revenue source."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["customer-conversion"]
    predictors: ["community-engagement"]
  - text: "Reliance on a self-supporting community substantially lowers a firm's support costs: engaged non-paying users build and maintain documentation, wikis, and peer knowledge bases, and increasingly resolve problems via search before ever contacting paid support, shifting the support burden away from the commercial firm."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["help-seeking", "collaboration"]
    predictors: ["community-engagement", "peer-mentoring"]
  - text: "Estimated sales-and-marketing-to-R&D expense ratios are much lower for commercial open source firms than for traditional vendors -- roughly 0.6 for a hypothetical open source CRM vendor versus 2.3 typical for traditional software firms and 6 for proprietary competitor Salesforce -- attributed to community members providing free, credible word-of-mouth marketing."
    evidence: "theory"
    support_strength: "weak"
    outcomes: ["productivity"]
    predictors: ["community-engagement", "open-source-maintenance"]
population:
  who: "Single-vendor commercial open source software firms and their user/developer communities (e.g., MySQL, SugarCRM, Jaspersoft, Alfresco), characterized through public interviews, conference presentations, and industry reports by practitioners and analysts (2005-2009)."
  where: []
  when: "2005-2009 (source statements); published 2010"
  n: null
  sector: ["technology", "open-source"]
  sample_notes: >
    Not a systematic empirical study: the author compiled anecdotal public statements,
    interviews, and presentations by open source business practitioners and industry
    analysts (Gartner, IDC, FLOSSmetrics), then synthesized them into a descriptive
    framework. No sampling frame, response rate, or primary data collection is reported; a
    handful of named firms serve as illustrative examples throughout.
limitation:
  primary: "The paper is a narrative synthesis of anecdotal practitioner statements and presentations rather than systematic empirical research, so its claims (conversion rates, cost ratios, causal community benefits) lack controlled measurement, sampling rigor, or statistical validation."
  others:
    - "Focuses exclusively on single-vendor commercial firms, so findings about community dynamics may not generalize to volunteer-governed community open source projects."
    - "Now over a decade old (published 2010, sources from 2005-2009); the commercial open source landscape and business models have evolved substantially since."
    - "The author acknowledges no prior comprehensive reference existed, underscoring the exploratory, non-cumulative nature of the evidence base."
risk_of_bias: "high"
relevance_to_project: >
  Documents the incentive structure firms use to cultivate engaged, self-supporting open
  source communities -- treating community peer-support and word-of-mouth engagement as a
  deliberate cost-saving business strategy. This is directly relevant to SNH's interest in
  open-source maintainer and contributor dynamics: it frames community engagement and help-
  seeking behavior as something organizations actively design for and extract value from,
  which has implications for maintainer workload and burnout risk when 'self-supporting'
  communities under-deliver.
tags:
  topic: ["open-source", "community-health", "maintainer-burnout", "collaboration"]
  method: ["theory", "secondary-data"]
  population: ["open-source-firms", "software-industry"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/The Single-Vendor Commercial Open Source Business Model/The Single-Vendor Commercial Open Source Business Model.md"
  pdf: "papers/Articles/01 Articles - Extended/The Single-Vendor Commercial Open Source Business Model.pdf"
  notes: null

---

id: "zhang-2022-turnover-of-companies-in-openstack-prevalence"
title: "Turnover of Companies in OpenStack: Prevalence and Rationale"
authors:
  - "Zhang, Yuxia"
  - "Liu, Hui"
  - "Tan, Xin"
  - "Zhou, Minghui"
  - "Jin, Zhi"
  - "Zhu, Jiaxin"
year: 2022
doi: "10.1145/3510849"
venue: {type: "journal", name: "ACM Transactions on Software Engineering and Methodology", volume: 31, issue: 4, pages: "1-24"}
citation: "Zhang et al. (2022). Turnover of Companies in OpenStack: Prevalence and Rationale. ACM Transactions on Software Engineering and Methodology, 31(4), 1-24. https://doi.org/10.1145/3510849"
article_type: "empirical"
method: {design: "mixed-methods", approach: "secondary-data", evidence_level: "moderate", preregistered: false}
gist: >
  This mixed-methods study of 18 versions of OpenStack finds that company (not just
  individual developer) withdrawal is common and accelerating: about 12% of sustaining
  companies exit each version, and 266 of 490 companies (54%) ultimately withdrew, with
  withdrawals outpacing new company joins after version 13. Withdrawn companies contributed
  far less before leaving (median 1 developer, 6 commits, 3 repos) and had roughly 2.7x
  lower contribution intensity than companies that stayed, though similar breadth of
  repositories touched. An email survey and Cox survival model show withdrawal reasons
  cluster into company, community, developer, and project factors, with achieving or failing
  a commercial goal most common, and low contribution intensity, business-integration goals,
  and small company scale statistically predicting withdrawal.
claims:
  - text: "Approximately 12% of companies sustaining in a given OpenStack version withdraw by the next version, and more than half of companies that join in any given version eventually withdraw; the number of withdrawing companies surpasses new joiners starting around version 13-14, ending the ecosystem's growth trend in contributing organizations."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["turnover", "retention"]
    predictors: ["organizational-culture", "community-engagement"]
  - text: "Withdrawn companies (n=266) made limited contributions before leaving (median 1 developer, 6 commits, 3 repositories, 2 versions) and had a contribution intensity approximately 2.7 times lower than companies that joined in the same version but stayed (Mann-Whitney p=0.037, medium effect r=-0.36), while contribution extent (repository scope) was similar between the two groups (p=0.63, r=-0.086)."
    evidence: "cross-sectional"
    support_strength: "moderate"
    outcomes: ["turnover", "collaboration"]
    predictors: ["community-engagement", "organizational-culture"]
  - text: "A Cox survival model (n=977 company-versions, 260 withdrawal events, concordance=0.86) found lower contribution intensity, an 'integrating business' commercial goal, and being a development-infrastructure vendor significantly predicted higher withdrawal hazard, while larger company scale (1,000-10,000+ employees, hazard reduced ~83%) and a 'selling partial solutions' goal predicted higher survival; project/community domination was not a significant predictor despite being frequently cited in survey responses."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["turnover", "retention"]
    predictors: ["organizational-culture", "workload", "community-engagement"]
population:
  who: "Companies contributing code to the OpenStack open-source cloud-computing ecosystem across 18 software versions (roughly a decade), plus a subset of their developer representatives surveyed by email"
  where: ["international (OpenStack global contributor base, company HQs not restricted to one country)"]
  when: "OpenStack versions 1 through 18 (approx. 2010-2021), data collected/analyzed through January 2021"
  n: 490
  sector: ["open-source", "technology"]
  sample_notes: >
    490 companies and 9,653 developers across 1,292 repositories and 338,035 commits form
    the core commit-mining dataset (266 identified as withdrawn, ~89% validated accuracy).
    Email survey of 455 candidate developer-representatives from withdrawn companies yielded
    38 responses from 37 distinct companies (16% response rate after excluding 222 bounced
    emails), a plausible source of self-report and selection bias. Survival model used a
    smaller manually-coded subsample of 60 withdrawn and 60 sustaining companies for
    commercial-goal data.
limitation:
  primary: "Withdrawal is inferred algorithmically from commit-history gaps (not confirmed departure) for the large-scale quantitative analysis, and while manually validated at ~89% accuracy, the method only captures withdrawal from source-code contribution, missing other contribution types (reviewing, issue reporting) that some 'withdrawn' companies may still perform."
  others:
    - "Email survey has a low 16% response rate and relies on self-reported reasons from company representatives, who may self-censor or give socially acceptable rather than true reasons for withdrawal."
    - "The survival model's commercial-goal and scale data were manually coded for only a 120-company subsample, limiting statistical power and generalizability of the predictive factors."
    - "Single-ecosystem case study (OpenStack only); authors note generalization is to theoretical propositions, not necessarily to all OSS ecosystems, especially those less dominated by commercial contributors."
risk_of_bias: "medium"
relevance_to_project: >
  Directly informs how the SNH project might operationalize organizational-level
  'turnover/retention' and 'community-engagement' constructs beyond individual developers:
  it offers a validated method (contribution-interval survival analysis) and concrete
  predictors (contribution intensity, organizational goal type, organizational scale) for
  detecting disengagement risk in open-source/tech communities before it happens, which is
  transferable to designing early-warning or retention interventions for maintainer and
  contributor-organization health.
tags:
  topic: ["open-source", "maintainer-burnout", "community-health", "measurement"]
  method: ["mixed-methods", "secondary-data", "survey"]
  population: ["open-source-contributors", "organizations"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/Turnover of Companies in OpenStack Prevalence and Rationale/Turnover of Companies in OpenStack Prevalence and Rationale.md"
  pdf: "papers/Articles/01 Articles - Extended/Turnover of Companies in OpenStack Prevalence and Rationale.pdf"
  notes: null

---

id: "mockus-2005-two-case-studies-of-open-source"
title: "Two Case Studies of Open Source Software Development: Apache and Mozilla"
authors:
  - "Mockus, Audris"
  - "Fielding, Roy T."
  - "Herbsleb, James D."
year: 2005
doi: "10.7551/mitpress/5326.003.0016"
venue: {type: "book", name: "Perspectives on Free and Open Source Software", volume: null, issue: null, pages: "163-210"}
citation: "Mockus et al. (2005). Two Case Studies of Open Source Software Development: Apache and Mozilla. Perspectives on Free and Open Source Software, 163-210. https://doi.org/10.7551/mitpress/5326.003.0016"
article_type: "empirical"
method: {design: "case-study", approach: "secondary-data", evidence_level: "moderate", preregistered: false}
gist: >
  This paper mines email, CVS, and bug-database archives from the Apache and Mozilla open
  source projects (plus five commercial telecom projects as a baseline) to show that OSS
  communities have a highly skewed 'onion' participation structure: a small core of 15-35
  developers does the great majority of new-functionality work, while much larger and looser
  groups handle defect repair and problem reporting. It argues that as project size grows
  beyond roughly 10-15 people, informal trust-based coordination among core developers
  becomes insufficient and is replaced by formal mechanisms such as enforced code ownership
  and mandatory multi-stage inspection (as seen in Mozilla versus Apache), trading
  development speed for coordination capacity.
claims:
  - text: "In Apache, the top 15 ('core') developers contributed more than 83% of modification requests and code deltas, 88% of added lines, and 91% of deleted lines, while a much larger and more loosely engaged group did the bulk of defect reporting: about 3,060 people submitted 3,975 problem reports but only 458 of them (591 reports) led to an actual code change."
    evidence: "case-study"
    support_strength: "moderate"
    outcomes: ["collaboration", "communication"]
    predictors: ["network-structure", "open-source-maintenance"]
  - text: "Despite being volunteer and part-time, Apache's core developers were roughly as productive as full-time developers on comparable commercial telecom projects (within a factor of 1.5 in KLOC/developer/year) and Apache's pre-system-test defect density (2.64 defects/KLOC added) was substantially lower than four commercial comparison projects (5.7-6.9 defects/KLOC added at the same development stage)."
    evidence: "case-study"
    support_strength: "moderate"
    outcomes: ["productivity", "performance"]
    predictors: ["team-cohesion", "open-source-maintenance"]
  - text: "As module size scaled beyond what a small informally-coordinated core could handle, Mozilla adopted formal code ownership and mandatory two-stage inspections; per-module core teams ranged from 22 to 36 developers (versus Apache's 15), and this formality came with a large cost in speed: roughly half of Apache's problem reports were resolved within a single day, while Mozilla's median resolution intervals ran from about 15 to 50 days depending on module and outcome."
    evidence: "case-study"
    support_strength: "moderate"
    outcomes: ["collaboration", "productivity"]
    predictors: ["team-cohesion", "network-structure"]
population:
  who: "Archival trace data from two large open source software communities (Apache HTTP Server: ~388 code contributors and ~3,060 distinct problem reporters from 1995-1999; seven Mozilla browser modules: 486 code contributors and ~6,837 problem reporters, 1998-2001) benchmarked against five in-house commercial telecommunications software projects at Lucent/Avaya."
  where: ["United States"]
  when: "Apache: Feb 1995-May 1999 (email/CVS archives); Mozilla: 1998-2001; commercial comparison projects: contemporaneous telecom development at Lucent/Avaya"
  n: null
  sector: ["software-development", "open-source-software", "telecommunications"]
  sample_notes: >
    Not a random sample: Apache and Mozilla were chosen as prominent, well-documented OSS
    projects, and the five commercial projects were chosen for data availability and
    researcher familiarity rather than representativeness. Population counts vary by measure
    (e.g., 388 Apache code contributors vs. ~3,060 problem reporters) because different
    archival sources (email, CVS, BUGDB/Bugzilla) capture different participant roles.
limitation:
  primary: "Two-case comparative design with a convenience sample of five commercial baseline projects chosen for the authors' familiarity and data access rather than random or representative selection, limiting generalizability of the hypotheses to other OSS communities or hybrid commercial/OSS efforts."
  others:
    - "Defect density measures are acknowledged by the authors to be confounded by unmeasured usage intensity and code verbosity ('bloat'), with no fully satisfactory solution offered."
    - "Mozilla had not yet shipped a non-beta release at time of writing, so postrelease defect density (the customer-relevant measure used for Apache) could not be computed for Mozilla, weakening the cross-project comparison."
    - "Qualitative process descriptions relied on a small number of core informants (one Apache core developer/co-author; Mozilla's 'Chief Lizard Wrangler') reviewed by only one or two additional people each, risking an idealized or narrow account of how governance actually worked."
risk_of_bias: "medium"
relevance_to_project: >
  This is a foundational quantitative account of the OSS 'onion' participation structure the
  SNH project's open-source/maintainer-burnout strand relies on: it shows the funnel from
  thousands of problem reporters down to a small (15-35 person) core that carries most
  development workload, and it documents the concrete mechanism (informal trust-based
  coordination vs. enforced code ownership plus mandatory inspection) that governs how
  coordination and workload concentration change as a community scales, directly informing
  how the project models maintainer workload and community-engagement structure.
tags:
  topic: ["open-source", "collaboration", "community-health", "maintainer-burnout", "productivity"]
  method: ["case-study", "secondary-data"]
  population: ["open-source-contributors", "software-engineers"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/Two Case Studies of Open Source Software Development Apache and Mozilla/Two Case Studies of Open Source Software Development Apache and Mozilla.md"
  pdf: "papers/Articles/01 Articles - Extended/Two Case Studies of Open Source Software Development Apache and Mozilla.pdf"
  notes: null

---

id: "barcomb-2020-uncovering-the-periphery-a-qualitative-survey"
title: "Uncovering the Periphery: A Qualitative Survey of Episodic Volunteering in Free/Libre and Open Source Software Communities"
authors:
  - "Barcomb, Ann"
  - "Kaufmann, Andreas"
  - "Riehle, Dirk"
  - "Stol, Klaas-Jan"
  - "Fitzgerald, Brian"
year: 2020
doi: "10.1109/tse.2018.2872713"
venue: {type: "journal", name: "IEEE Transactions on Software Engineering", volume: 46, issue: 9, pages: "962-980"}
citation: "Barcomb et al. (2020). Uncovering the Periphery: A Qualitative Survey of Episodic Volunteering in Free/Libre and Open Source Software Communities. IEEE Transactions on Software Engineering, 46(9), 962-980. https://doi.org/10.1109/tse.2018.2872713"
article_type: "empirical"
method: {design: "qualitative", approach: "interview", evidence_level: "low", preregistered: false}
gist: >
  Based on a qualitative survey (interviews with 11 community managers and 9 episodic
  volunteers across 13 FLOSS communities, triangulated with 50 supplemental documents), the
  paper argues that the core/periphery 'Onion model' oversimplifies peripheral contributors
  and proposes replacing it with the habitual/episodic volunteer distinction drawn from the
  general volunteering literature. It finds episodic volunteering (EV) is widespread across
  all types of FLOSS contribution (not just code), that five volunteering-retention
  constructs (motivation, social norms, psychological sense of community, satisfaction,
  community commitment) apply in FLOSS, and that no community studied had a deliberate
  strategy for managing or retaining episodic (as opposed to habitual) contributors.
claims:
  - text: "Episodic volunteering was observed in every type of FLOSS contribution examined (code, translation, documentation, events, evangelism, support) across all 13 communities studied, yet none of the community managers interviewed reported a deliberate strategy for recruiting or retaining episodic (versus habitual) volunteers."
    evidence: "qualitative"
    support_strength: "low"
    outcomes: ["retention"]
    predictors: ["organizational-culture", "community-engagement"]
  - text: "Personal invitation, not formal recruitment channels, was the most common route into volunteering for non-code contributors; although an intake questionnaire suggested episodic volunteers did not see social norms (pressure/support from friends and family) as relevant to their participation, interview data showed several had actually started volunteering after a personal invitation from someone they knew."
    evidence: "qualitative"
    support_strength: "low"
    outcomes: ["retention", "community-engagement"]
    predictors: ["social-norms", "social-support"]
  - text: "Satisfaction — especially feeling appreciated for one's contributions — was the reason most frequently cited by episodic volunteers and community managers for continued participation, and episodic volunteers who talked publicly about their FLOSS involvement were more inclined to report intention to remain, regardless of how long they had already been contributing."
    evidence: "qualitative"
    support_strength: "low"
    outcomes: ["retention", "job-satisfaction"]
    predictors: ["sense-of-belonging", "community-engagement"]
population:
  who: "11 community managers (CM1–CM11) and 9 self-selected episodic volunteers (EV1–EV9, some active in multiple projects) drawn from 13 FLOSS communities (Mozilla, Perl Foundation, Chef, Red Hat, Bolt CMS, JSON-RPC Client, ownCloud, Zato, Butterfly Effect, Gnash, Django, KDE, TinyRPC), plus 50 supplemental documents (public interviews, web pages, mailing-list threads) for triangulation."
  where: []
  when: "Autumn 2014 to Spring 2017"
  n: 20
  sector: ["open-source"]
  sample_notes: >
    Theoretical/purposive sampling designed to span multi-/single-project and
    vendor-/community-oriented quadrants; community managers recruited via personal contacts
    and mailing-list ads; episodic volunteers self-selected through an open call on social
    media, mailing lists, and conferences (Mozfest, FOSDEM) tied to a parallel motivations
    survey, screened by self-reported episodic status and hours; contribution levels were
    cross-checked against commit counts for only about half of code-contributing
    participants; small, non-probabilistic sample not intended to be statistically
    representative.
limitation:
  primary: "Small, self-selected qualitative sample (20 interviewees across 13 communities) relying substantially on self-reported volunteering behavior and retrospective identification of episodic status, so the study can describe patterns but cannot establish causal or quantitative links between the five proposed retention constructs and actual retention."
  others:
    - "Exploratory design was built to test researcher-derived predictions from the general volunteering literature rather than to generate a fully independent theory, risking confirmation bias despite member checks and investigator triangulation"
    - "Most claims about contribution levels/motivations rely on self-report rather than behavioral trace data"
    - "Findings, while consistent across the sampled communities, are explicitly described by the authors as not generalizable to all FLOSS communities"
risk_of_bias: "medium"
relevance_to_project: >
  Provides a concrete, literature-grounded framework (contributor motivation, social norms,
  psychological sense of community, satisfaction, community commitment) plus specific
  practices (thanking/crediting all contribution types, personal invitations, low-effort
  task-finding dashboards, time-based releases, opt-in calls for help) for designing
  engagement and retention mechanisms aimed at the large, mostly-ignored periphery of
  infrequent open-source contributors, directly relevant to SNH's community-health and
  maintainer-burnout design work on episodic rather than only habitual/core participation.
tags:
  topic: ["open-source", "community-health", "job-engagement", "social-support"]
  method: ["qualitative", "interview"]
  population: ["open-source-contributors", "volunteers", "community-managers"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/Uncovering the Periphery A Qualitative Survey of Episodic Volunteering in Free Libre and Open Source Software Communities/Uncovering the Periphery A Qualitative Survey of Episodic Volunteering in Free Libre and Open Source Software Communities.md"
  pdf: "papers/Articles/01 Articles - Extended/Uncovering the Periphery A Qualitative Survey of Episodic Volunteering in Free Libre and Open Source Software Communities.pdf"
  notes: null

---

id: "wang-2020-unveiling-elite-developers-activities-in-open"
title: "Unveiling Elite Developers’ Activities in Open Source Projects"
authors:
  - "Wang, Zhendong"
  - "Feng, Yang"
  - "Wang, Yi"
  - "Jones, James A."
  - "Redmiles, David"
year: 2020
doi: "10.1145/3387111"
venue: {type: "journal", name: "ACM Transactions on Software Engineering and Methodology", volume: 29, issue: 3, pages: "1-35"}
citation: "Wang et al. (2020). Unveiling Elite Developers’ Activities in Open Source Projects. ACM Transactions on Software Engineering and Methodology, 29(3), 1-35. https://doi.org/10.1145/3387111"
article_type: "empirical"
method: {design: "longitudinal", approach: "secondary-data", evidence_level: "moderate", preregistered: false}
gist: >
  This study mines fine-grained GitHub event data (900,862 events, Jan 2015-Oct 2018) from
  20 large open source projects to profile 'elite' developers (those with write/admin
  privileges) across four activity types: communicative, organizational, supportive, and
  typical (coding). It finds elite developers perform the large majority of nontechnical
  work as well as most code, that their effort mix shifts sharply toward nontechnical work
  as a project grows while their coding stagnates or declines, and that this nontechnical
  effort is generally negatively correlated with project productivity and (mixed) with
  quality, except supportive effort which is linked to a higher bug fix rate. The paper
  frames this as a workload-imbalance and role-transition dilemma with direct implications
  for maintainer burnout and tool/workflow design.
claims:
  - text: "Elite developers perform over 50% of organizational, supportive, and typical activities and 34% of communicative activities in their projects; on average an elite developer performs 7x more communicative, 145x more organizational, 22x more supportive, and 22x more typical activities per month than a nonelite developer."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["burnout", "collaboration"]
    predictors: ["open-source-maintenance", "workload"]
  - text: "As projects grow, elite developers significantly increase communicative and supportive effort while typical (coding) activity growth is significantly lower and even negative on average (-1.63% monthly growth), meaning an elite developer does roughly half the technical work after three years that they did initially, even as communicative and supportive work doubled."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["burnout", "job-engagement"]
    predictors: ["open-source-maintenance", "workload"]
  - text: "In fixed-effects panel regressions, elite developers' communicative and supportive effort shares are negatively correlated with new commits and (via supportive share) with longer bug cycle time (productivity loss, beta = -155.96 to -138.21, p<.01-.001); organizational and supportive effort shares are positively correlated with new bugs found (quality loss), while supportive effort share is positively correlated with bug fix rate (quality gain); these effects are stronger in company-sponsored projects."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["productivity", "collaboration"]
    predictors: ["workload", "open-source-maintenance"]
population:
  who: "20 large, established open source GitHub projects (11 company-sponsored, 9 non-company-sponsored) with formal PR-based governance, at least 100 pull requests and 50 contributors historically; unit of analysis is elite vs. nonelite developer activity aggregated to project-months."
  where: []
  when: "January 2015 to October 2018"
  n: 720
  sector: ["open-source"]
  sample_notes: >
    Sample is 20 purposively selected large, mature GitHub projects (e.g., React,
    TensorFlow, TiDB); 720 project-month observations (20 projects x 36 months) used in
    regressions. Elite status inferred indirectly via a permissions-check heuristic (write-
    permission-requiring actions) rather than direct access to GitHub's permission list,
    with a 90-day rolling 'elite-ship' window. Findings generalize only to large, governed
    OSS projects, not small/medium ones, and rely solely on public GitHub trace data (no
    email, IRC, or chat channels).
limitation:
  primary: "All regressions establish correlation, not causation, between elite developers' effort allocation and project productivity/quality outcomes, despite the paper's narrative framing some relationships as if causal."
  others:
    - "Elite/nonelite status and activity categories are inferred from a single data source (public GitHub events) using an indirect permissions-check heuristic, since GitHub does not expose actual permission lists to outside researchers."
    - "Sample is restricted to 20 large, well-governed projects with established PR workflows, so findings may not generalize to small, informal, or poorly governed OSS projects."
    - "Some GitHub event data (e.g., certain issue-management actions) could only be captured via a supplementary customized API script, and non-GitHub communication channels (email, IRC, Slack) are entirely excluded."
risk_of_bias: "medium"
relevance_to_project: >
  Provides quantitative, project-scale evidence that open-source maintainers' (elite
  developers') shift toward communicative/organizational/supportive labor as projects scale
  is associated with productivity loss and mixed quality effects, directly substantiating
  the maintainer-burnout and workload-imbalance mechanism the SNH project cares about, and
  motivating tool/workflow interventions (task delegation, automation of routine
  admin/support work) to protect maintainer wellbeing.
tags:
  topic: ["open-source", "maintainer-burnout", "collaboration", "community-health"]
  method: ["secondary-data", "longitudinal", "panel-regression"]
  population: ["open-source-maintainers", "software-developers"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/Unveiling Elite Developers Activities in Open Source Projects/Unveiling Elite Developers Activities in Open Source Projects.md"
  pdf: "papers/Articles/01 Articles - Extended/Unveiling Elite Developers Activities in Open Source Projects.pdf"
  notes: null

---

id: "miller-2019-why-do-people-give-up-flossing"
title: "Why Do People Give Up FLOSSing? A Study of Contributor Disengagement in Open Source"
authors:
  - "Miller, Courtney"
  - "Widder, David Gray"
  - "Kästner, Christian"
  - "Vasilescu, Bogdan"
year: 2019
doi: "10.1007/978-3-030-20883-7_11"
venue: {type: "book", name: "IFIP Advances in Information and Communication Technology", volume: null, issue: null, pages: "116-129"}
citation: "Miller et al. (2019). Why Do People Give Up FLOSSing? A Study of Contributor Disengagement in Open Source. IFIP Advances in Information and Communication Technology, 116-129. https://doi.org/10.1007/978-3-030-20883-7_11"
article_type: "empirical"
method: {design: "mixed-methods", approach: "survey", evidence_level: "moderate", preregistered: false}
gist: >
  This mixed-methods study surveys 151 established open source contributors who recently
  disengaged from all public GitHub activity, then uses Cox proportional-hazards survival
  modeling on 206 contributors (103 disengaged, 103 control) to test which factors predict
  disengagement. Occupational transitions (job or school changes) were by far the most
  commonly cited reason for disengagement, more so than lack of peer support or loss of
  interest, and contributors working nights/weekends cited social reasons more than those
  working office hours. The survival model confirms that working during office hours and
  experiencing a job/school transition both significantly increase disengagement risk, while
  higher activity level and working on more popular projects decrease it.
claims:
  - text: "In an open-ended survey of 151 recently disengaged contributors (239 total reasons cited), occupational reasons such as job or school transitions were the most common category (106 citations), more frequent than lack of peer support or losing interest in FLOSS, which are more commonly emphasized in prior literature."
    evidence: "mixed-methods"
    support_strength: "moderate"
    outcomes: ["turnover", "retention"]
    predictors: ["community-engagement", "social-support"]
  - text: "In the Cox proportional-hazards survival model (n=206 contributors, 103 disengaged), experiencing a job/school transition in the last year increased risk of disengagement by a hazard ratio of 2.48 (p<0.01), and working predominantly during office hours (vs. nights/weekends) increased disengagement risk with a hazard ratio of 1.56-2.20 (p<0.05)."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["turnover", "retention"]
    predictors: ["boundary-management", "workload"]
  - text: "Higher overall activity level (hazard ratio 0.36, p<0.001) and working on more popular projects (higher GitHub stars; hazard ratio 0.85-0.86, p<0.01) both significantly decreased a contributor's risk of disengagement, while doing more support-oriented work (issues/PR management) showed no statistically significant effect on disengagement risk."
    evidence: "longitudinal"
    support_strength: "moderate"
    outcomes: ["retention", "turnover"]
    predictors: ["community-engagement", "network-structure"]
population:
  who: "Established open source contributors on GitHub who had contributed at least 100 commits per six-month period for three consecutive periods (18 months of sustained activity); survey sample of 151 who then went nearly silent (disengaged), plus a survival-model sample of 206 (103 disengaged 'treatment', 103 active 'control')"
  where: []
  when: "GHTorrent trace data version 2018-08; survey conducted circa 2018-2019"
  n: 206
  sector: ["open-source"]
  sample_notes: >
    Survey invited 702 identified recently-disengaged contributors with public email
    addresses; received 151 valid responses (21.5% response rate). Survival model further
    restricted to 206 of these plus controls for whom public CV data could be located (34
    excluded for lack of CV data), risking selection bias. Sample targets established/highly
    active contributors, not peripheral or episodic ones, so findings may not generalize to
    occasional contributors.
limitation:
  primary: "The survival model's treatment group is limited to survey respondents with locatable public CVs, introducing selection bias and constraining statistical power due to the resulting moderate sample size (206)."
  others:
    - "Self-reported survey reasons for disengagement may be subject to social-desirability bias (respondents citing more acceptable reasons like job transitions rather than dissatisfaction or conflict)."
    - "Disengagement was operationalized as a sudden drop in public GitHub activity within a six-month window, which may not capture more gradual disengagement and could misclassify moves to private repositories or other platforms."
    - "Findings are specific to highly active, established contributors identified via GHTorrent trace data and may not generalize to peripheral, episodic, or non-GitHub open source contributors."
risk_of_bias: "medium"
relevance_to_project: >
  Provides a concrete, trace-data-operationalizable predictor set (job/school transitions,
  working-hours pattern, activity level, project popularity) for identifying at-risk open
  source contributors before they disengage, directly informing SNH's design of early-
  warning or support-targeting mechanisms for maintainer/contributor burnout and turnover.
  The finding that occupational transitions dominate self-reported disengagement reasons
  over lack of peer support suggests SNH interventions should consider life-transition-aware
  support alongside community-belonging interventions.
tags:
  topic: ["open-source", "maintainer-burnout", "community-health", "methodology"]
  method: ["mixed-methods", "survey"]
  population: ["open-source-contributors"]
source:
  markdown: "Papers_Data/Articles/01 Articles - Extended/MD/Why Do People Give Up FLOSSing A Study of Contributor Disengagement in Open Source/Why Do People Give Up FLOSSing A Study of Contributor Disengagement in Open Source.md"
  pdf: "papers/Articles/01 Articles - Extended/Why Do People Give Up FLOSSing A Study of Contributor Disengagement in Open Source.pdf"
  notes: null

---

id: "sapegin-nd-why-i-quit-open-source"
title: "Why I quit open source"
authors:
  - "Sapegin, Artem"
year: null
doi: null
venue: {type: "other", name: "sapegin.me (personal blog)", volume: null, issue: null, pages: null}
citation: "Sapegin (None). Why I quit open source. sapegin.me (personal blog)."
article_type: "commentary"
method: {design: "case-study", approach: "other", evidence_level: "weak", preregistered: false}
gist: >
  A veteran open-source maintainer (roughly ten years, publisher of the widely-used React
  Styleguidist project) explains in first person why he quit maintaining open-source
  software entirely, arguing that quitting, not the moderation tips in GitHub's official
  burnout-avoidance guide, was the only solution that actually worked for him. He attributes
  his burnout to entitled and toxic users, low-quality drive-by pull requests, failure to
  build a sustaining contributor community even around a 10K-star project, near-zero
  financial compensation, and mounting tooling/configuration overhead, and closes by
  describing how he now treats his repos as private projects that happen to be public.
claims:
  - text: "The maintainer reports receiving essentially no sustainable income from a decade of open-source work: an Open Collective project budget of about $8/month, zero results from GitHub Sponsors aside from one $550 payment from GitHub itself that was later cancelled, and no payments via a 'Buy Me a Coffee' link despite the project's popularity."
    evidence: "case-study"
    support_strength: "weak"
    outcomes: ["burnout", "job-satisfaction"]
    predictors: ["open-source-maintenance", "workload"]
  - text: "Even his most popular project (10,000+ GitHub stars) never developed a self-sustaining contributor community; occasional volunteers still required heavy guidance from him, so the project remained a single point of failure that would stop entirely if he stopped working on it."
    evidence: "case-study"
    support_strength: "weak"
    outcomes: ["collaboration", "isolation", "burnout"]
    predictors: ["community-engagement", "network-structure", "open-source-maintenance"]
  - text: "He identifies entitled/toxic user behavior (demands, insults, spam pings, low-effort 'hit and run' pull requests, and abuse during Hacktoberfest) as a primary driver of burnout, and argues GitHub's platform does too little to detect, remove, or discourage this behavior."
    evidence: "case-study"
    support_strength: "weak"
    outcomes: ["burnout", "stress"]
    predictors: ["open-source-maintenance", "psychological-safety", "workload"]
population:
  who: "A single individual open-source maintainer (JavaScript/TypeScript ecosystem, author of React Styleguidist and other projects) recounting roughly ten years of unpaid maintenance work."
  where: []
  when: null
  n: 1
  sector: ["tech", "open-source"]
  sample_notes: >
    First-person autobiographical blog post; n=1, no systematic data collection, no external
    verification of the claims about compensation or contribution volume.
limitation:
  primary: "Single-author anecdotal account with no independent data or systematic sampling; findings are one maintainer's retrospective attribution of his own burnout and cannot be generalized to open-source maintainers broadly."
  others:
    - "No date given in the source, so it is unclear how recent the experience or the GitHub ecosystem context is."
    - "Written explicitly as a rebuttal to a specific GitHub guide, which frames the piece argumentatively rather than as neutral description."
risk_of_bias: "high"
relevance_to_project: >
  Provides a vivid, specific first-person account of the mechanisms (unrewarded labor, toxic
  user entitlement, inability to build a sustaining community, tooling overhead) that the
  project's maintainer-burnout and open-source community-health design work needs to
  address; useful as illustrative evidence and for generating hypotheses, not as a causal or
  generalizable finding.
tags:
  topic: ["maintainer-burnout", "open-source", "burnout", "community-health"]
  method: ["case-study"]
  population: ["software-developers", "open-source-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/Why I Quit Open Source/Why I Quit Open Source.md"
  pdf: "papers/Articles/Why I Quit Open Source.pdf"
  notes: "no-doi: confirmed none (manual review)"

---

id: "thompson-2022-why-open-source-developers-are-burning"
title: "Why Open-Source Developers Are Burning Out"
authors:
  - "Thompson, Clive"
year: 2022
doi: null
venue: {type: "other", name: "Better Programming (Medium)", volume: null, issue: null, pages: null}
citation: "Thompson (2022). Why Open-Source Developers Are Burning Out. Better Programming (Medium)."
article_type: "commentary"
method: {design: "case-study", approach: "other", evidence_level: "speculative", preregistered: false}
gist: >
  This Medium/Better Programming piece uses the January 2022 'colors' npm library incident —
  in which maintainer Marak Squires intentionally sabotaged his own widely-used code,
  breaking thousands of dependent apps — as a case study for arguing that open-source
  maintenance has become unpaid, unsustainable labor performed by stressed individuals
  rather than the collaborative 'barn-raising' the movement promised. The corpus copy
  available here is truncated at Medium's paywall, so only the opening anecdote and framing
  are present, not the article's full argument or sourcing.
claims:
  - text: "The npm library 'colors', used by roughly 19,000 software projects with over 20 million weekly downloads, was deliberately sabotaged by its own maintainer, Marak Squires, who added an infinite loop producing garbled output and breaking dependent applications."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout"]
    predictors: ["open-source-maintenance", "workload"]
  - text: "Unnamed observers linked the sabotage to burnout, noting Squires had recently said he was feeling burned out and speculating about unspecified mental-health issues as a contributing factor."
    evidence: "case-study"
    support_strength: "speculative"
    outcomes: ["burnout", "mental-health"]
    predictors: ["open-source-maintenance"]
population:
  who: "A single open-source maintainer (Marak Squires, developer of the npm 'colors' and 'faker' libraries) used as an illustrative case; the article's implicit broader subject is unpaid maintainers of widely-depended-upon open-source software."
  where: []
  when: "January 2022"
  n: null
  sector: ["open-source", "software-development"]
  sample_notes: >
    This corpus copy contains only the article's opening ~500 words (the 'colors' library
    anecdote) before hitting a Medium members-only paywall; the rest of the file is site
    navigation, author bio, and unrelated 'recommended' article links, not further article
    content. No systematic sample — a single high-profile incident used illustratively, not
    research data.
limitation:
  primary: "Only the introductory anecdote of the article is present in this corpus copy; the full piece is behind Medium's paywall, so its main argument, evidence, and any additional examples are missing from this source file."
  others:
    - "Journalistic commentary, not peer-reviewed research, and even the visible portion rests on a single high-profile incident used illustratively."
    - "The claim that Squires's actions were mental-health related is attributed only to unnamed 'observers', with no cited sources."
risk_of_bias: "high"
relevance_to_project: >
  Provides a vivid, widely-cited motivating case for the SNH project's maintainer-burnout
  concern — sabotage of critical infrastructure as a visible failure mode of unsupported
  unpaid open-source labor — useful for framing why-it-matters narratives, though the
  fragment available here is too thin and unsourced to use as evidentiary support for any
  specific claim.
tags:
  topic: ["open-source", "maintainer-burnout", "burnout", "mental-health"]
  method: ["case-study"]
  population: ["open-source-maintainers"]
source:
  markdown: "Papers_Data/Articles/MD/Why Open-Source Developers Are Burning Out/Why Open-Source Developers Are Burning Out.md"
  pdf: "papers/Articles/Why Open-Source Developers Are Burning Out.pdf"
  notes: "no-doi: web article / no registered DOI found"
