![](_page_0_Picture_0.jpeg)

# Why Do People Give Up FLOSSing? A Study of Contributor Disengagement in Open Source

Courtney Miller $^{1(\boxtimes)}$ , David Gray Widder $^{2(\boxtimes)}$ , Christian Kästner $^{2(\boxtimes)}$ , and Bogdan Vasilescu $^{2(\boxtimes)}$ 

 New College of Florida, Sarasota, USA courtney.miller17@ncf.edu
 Carnegie Mellon University, Pittsburgh, USA {dwidder,kaestner,vasilescu}@cmu.edu

**Abstract.** Established contributors are the backbone of many free/libre open source software (FLOSS) projects. Previous research has shown that it is critically important for projects to retain contributors and it has also revealed the motivations behind why contributors choose to participate in FLOSS in the first place. However, there has been limited research done on the reasons why established contributors disengage, and factors (on an individual and project level) that predict their disengagement. In this paper, we conduct a mixed-methods empirical study, combining surveys and survival modeling, to identify the reasons and predictive factors behind established contributor disengagement. We find that different groups of established contributors tend to disengage for different reasons; however, overall contributors most commonly cite some kind of transition (e.g., switching jobs or leaving academia). We also find that factors such as the popularity of the projects a contributor works on, whether they have experienced a transition, when they work, and how much they work are all factors that can be used to predict their disengagement from open source.

#### 1 Introduction

Contributor disengagement in open source is widely known as a costly and critical issue [9,19,49], as it can directly affect the sustainability of projects. For example, in a recent study Coelho et al. reported that 41% of failed open source projects cited a reason involving the developer team, such as lack of interest or time of the main contributor [9]. Such local (project-level) sustainability issues in open source can have cascading effects on the entire ecosystem because of project interdependencies [12,53]. So-called "core", i.e., established, contributors are particularly critical for the sustainability of open source projects [19,57].

C. Miller—Part of this work was carried our during the author's REU program at CMU.

© IFIP International Federation for Information Processing 2019 Published by Springer Nature Switzerland AG 2019 F. Bordeleau et al. (Eds.): OSS 2019, IFIP AICT 556, pp. 116–129, 2019. https://doi.org/10.1007/978-3-030-20883-7\_11

There are many reasons why established contributors disengage. Some may be unavoidable, whereas others could perhaps be prevented through interventions or by providing better community support. Likely there are various dynamics in play, including the role of volunteers as compared to corporate employees [\[44](#page-12-1)], the role of external events such as family planning and job changes, and the role of perceived purpose, community support, and stress. Effects might include abruptly leaving the project, but also slow disengagement, or causing rippling frustrations through delays or cynicism.

The goal of our research is to better understand disengagement factors and which established contributors are at risk and when; this will enable us to build and validate a conceptual framework and theory. Moreover, we pursue a datadriven approach, operationalizing uncovered factors based on publicly available trace data. This way, we can identify at-risk open source contributors and communities, and help guide resources (e.g., volunteers, sponsors) toward projects and contributors in need, enhancing the sustainability of the overall ecosystem.

We identify potential disengagement factors from literature on turnover and open source retention, cross-validate them with results from a survey among contributors who recently stopped all open source activities on GitHub, operationalize select factors with public trace data, and finally conduct survival modeling among a set of 206 GitHub users to triangulate the survey results.

Among others, we identify the degree to which contributors work outside of typical office hours and to what degree they engage in support activities as important moderating factors. According to Claes et al. [\[8\]](#page-10-1), 33% of open source contributors do not follow typical working hours, but instead work nights and weekends. Our survey shows that contributors who work nights and weekends proportionally tend to disengage for different reasons than those working regular hours. In addition, our survey reveals that the most common reasons for complete disengagement relate to transitions in employment, such as graduating from academia, changing employers, and changing roles.

To validate disengagement factors beyond our survey, we model to what degree hypothesized factors—such as working hours, engagement in support activities, and team size, which can be measured in public trace data of contributor activities—can predict the later disengagement of those contributors. To that end, we use the quantitative statistical method of survival modeling. As a key factor in our model, derived from our survey results, we incorporate transitions identified from public CVs of developers. Specifically, we analyze which contributor populations are more resilient to transitions such as job changes.

We find that working predominantly during office hours and experiencing a transition both increase a contributors risk of disengagement. Conversely, we find that increased levels of activity and working on more popular projects both decrease a contributors risk of disengagement.

In summary, we contribute (1) a survey revealing the reasons behind contributor disengagement; (2) a comparison between different groups of contributors; (3) measures to differentiate between groups, which could be used to help identify at-risk groups and better target support interventions; (4) a novel operationalization of transition data; and (5) a survival model demonstrating which factors are able to predict contributor disengagement.

# <span id="page-2-0"></span>**2 Related Work**

*Turnover.* Prior work has shown that the turnover rate of a project profoundly affects its survival probability [\[33,](#page-12-2)[46](#page-12-3)] and code quality [\[21\]](#page-11-2). Approximately 80% of open source projects fail due to contributor turnover related issues [\[46\]](#page-12-3). Even within projects that do not outright fail, contributor turnover has a significant adverse effect on software quality [\[21\]](#page-11-2). On a project level, contributor disengagement results in knowledge loss, which is a particularly expensive issue [\[33](#page-12-2)].

*Employee turnover* and *retention* have been broadly studied across many fields [\[31](#page-12-4)[,35](#page-12-5)]. In professional settings, early turnover research has focused often on personal characteristics (e.g., ability, age) and employee satisfaction, measured with hiring tests and surveys, whereas later research has explored many more nuanced factors, such as labor market (e.g., job opportunities), non-work values, and organizational commitment [\[31\]](#page-12-4). Research has shown that, while far from all turnover can be explained by dissatisfaction and similar factors [\[38\]](#page-12-6), there are positive and negative factors that can buffer against shocks such as external job offers [\[6,](#page-10-2)[20](#page-11-3)]. Turnover among volunteers is less explored: Although some research suggests that similar personal and environmental factors influence their decisions to quit [\[41](#page-12-7)], other researchers point out that satisfaction and achievement, compatible working hours, training, challenging work, and role identity may play particularly strong roles [\[25,](#page-11-4)[34](#page-12-8)[,50](#page-13-2)].

Whereas reasons for joining open source [\[5](#page-10-3)[,24](#page-11-5),[37,](#page-12-9)[44,](#page-12-1)[48](#page-12-10)[,54,](#page-13-3)[55\]](#page-13-4) and interventions to improve the onboarding experience for new developers [\[7,](#page-10-4)[18,](#page-11-6)[30](#page-11-7)[,52](#page-13-5)] have been studied in depth, studies of contributor retention are rarer. Prior research has focused primarily on testing basic attributes [\[11,](#page-11-8)[39,](#page-12-11)[40](#page-12-12)[,46,](#page-12-3)[49](#page-12-0)[,53](#page-13-0)[,58](#page-13-6)]. For example, they have shown that retention is higher for contributors that have participated longer [\[39](#page-12-11)[,49](#page-12-0)], contributed more code changes [\[11](#page-11-8)[,39](#page-12-11)], and communicated more [\[11\]](#page-11-8). However, there has been a limited amount of prior research has also explored more nuanced factors, like whether a developers gender and social network effect their risk of disengagement [\[43](#page-12-13)]. Using surveys, researchers further associated ratings of general dissatisfaction and lack of community identification with higher perceived turnover and turnover intentions [\[32,](#page-12-14)[56](#page-13-7)]. Zhou et al.'s case study of three projects further suggests that commercial participation can crowd out volunteers [\[58\]](#page-13-6).

Long working hours, lack of sleep, and lack of recovery on weekends are often discussed as stressors. Many studies confirm the importance of "mentally switching off" [\[1](#page-10-5)[,4](#page-10-6)[,51](#page-13-8)]. In software engineering, several studies have shown the influence of time-related factors, such as late-night commits and long working sessions being more likely to contain bugs [\[17](#page-11-9)[,45](#page-12-15)], sleep deprivation reducing code quality [\[22\]](#page-11-10), Monday commit comments using more negative language [\[29\]](#page-11-11), and time pressure is often seen as an important stressor [\[36](#page-12-16)].

*Open Source Practitioners Reporting Stress.* In addition to the academic literature, open source practitioners also spoke out about frustrations, funding concerns, stress, and even burnout. Often, there are high expectations and copious amounts of pressure placed on established open source contributors.

Many stories via blog posts from maintainers who disengaged have a similar narrative that describes the growing pressures and responsibilities they experienced that lead to their disengagement. One such blog post describes how *"as [my project's] popularity rose and rose, my drive to continue to create new projects, fell. All while the burden of supporting the needs of the massive user bases of my successful projects and the pressure of maintaining those projects grew."*[1](#page-3-0)

In addition to blog posts, there were also participants from the survey we ran who explicitly cited a lack of support as a reason for their disengagement. For example *"[The open source project] is increasingly depended upon by other projects, but very few external developers are interested/willing enough to [understand the company] let alone contribute improvements/fixes. The support burden is a good problem to have (people are finding [the project] useful), but it does impose a productivity (and sometimes a motivation) burden."* (P35)

Contributors are broadly expected to maintain their projects. Having a seemingly never-ending list of tasks is another commonly cited reason for disengagement among the aforementioned blog posts and survey respondents. As described in a blog post by a now-retired developer, *"working long hours for endless months"* was a critical reason for their disengagement.[2](#page-3-1)

# **3 Overview: Mixed-Method Research**

Our mixed-method empirical study follows a sequential exploratory design [\[14\]](#page-11-12), combining qualitative and quantitative analysis of survey and GitHub trace data.

Step 1: Survey (Sect. [4\)](#page-4-0). Although the turnover literature (Sect. [2\)](#page-2-0) provides several starting points for potential disengagement factors, there has been only limited research on the actual reasons *why* open source contributors disengage. Therefore, we decided to ground our research by conducting an open-ended survey among developer who recently disengaged from all public GitHub activities. We furthermore analyze the frequency of self-reported reasons for disengagement regarding whether different populations disengage for different reasons.

Step 2: Survival analysis (Sect. [5\)](#page-6-0). We test to what degree the potential disengagement factors identified statistically explain disengagement. To that end, we operationalize several disengagement factors, including when and what contributors worked on as well as job transitions in historic trace data and public CVs, and use survival modeling [\[42\]](#page-12-17) to test their significance.

<sup>1</sup> [https://www.kennethreitz.org/essays/the-reality-of-developer-burnout.](https://www.kennethreitz.org/essays/the-reality-of-developer-burnout)

<span id="page-3-1"></span><span id="page-3-0"></span><sup>2</sup> [https://hackernoon.com/what-is-programmer-burnout-651aa48984ef.](https://hackernoon.com/what-is-programmer-burnout-651aa48984ef)

# <span id="page-4-0"></span>**4 Self-reported Reasons for Disengagement (Survey)**

## <span id="page-4-1"></span>**4.1 Survey Methodology**

To ground our analyses, we surveyed a sample of open source contributors who recently disengaged from all public GitHub activities, asking about their reasons.

*Recently Disengaged Established Contributors.* We invited open source contributors who stopped all public activity on GitHub after being active for at least 18 month. We identified such contributors from GHTorrent [\[26](#page-11-13)] trace data (version 2018-08). We then constructed six-month panels aggregating contributions (commits and issue/pull request events) per person, and selected those contributors who contributed at least 100 commits per six-month period for three consecutive periods, but at most 5 commits in the following period (the five commit threshold allows for some residual activity). This way, we identified a total of 702 contributors who disengaged (i.e., stopped contributing publicly) within the last year and had public email addresses listed on their GitHub profile pages.

We specifically sampled only previously active contributors with at least 100 commits per period across all of GitHub. Previous research has shown that within a single project, there are many different kinds of contributors, with one of the most popular models being the onion model [\[15](#page-11-14)]. With our threshold we target contributors who are likely very active in at least one project, rather than more peripheral or episodic contributors, which may have different motivations [\[2](#page-10-7)].

*Survey Design.* We designed a simple, single-question, open-ended survey, asking *"Could you help us understand your reasons for reducing your contributions to GitHub projects?"* We chose the open-ended format to avoid priming the participants to ensure organic but relevant responses. We use the single-question format without external survey software, because it reduces the barrier to participation. We invited all 702 identified candidates and received 151 valid answers (21.5% response rate). Our response rate is in line with other GitHub surveys, e.g., [\[27\]](#page-11-15).

*Card Sorting Analysis.* We used card sorting, a qualitative content analysis [\[47](#page-12-18)] method, to analyze the survey answers. Two researchers reviewed the cards and organized them into mutually agreed upon categories using a ground-up process resulting in 17 subgroups. These subgroups were then further grouped into three overarching themes: Technical, Social, and Occupational. Note that many participants cited multiple reasons, resulting in 239 reasons from 151 responses.

*Quantitative Analysis.* In addition to identifying common self-reported reasons for disengagement from the survey responses, we additionally explore whether different populations report different reasons. Based on the literature and reports from open source practitioners (cf. Sect. [2\)](#page-2-0), we specifically investigate whether contributors (a) working mostly "regular" office hours or (b) performing more support activities report disengaging for different reasons.

*Working Hours:* Analyzing GitHub data, we measure what percentage of contributions are made between 7am and 7pm local time, Monday through Friday, captured as *indexWorkHours* (the slightly wider interval than the traditional 9am to 5pm increases robustness to daylight savings [\[8\]](#page-10-1)). To detect the contributor's local time, we adjusted the UTC times in GHTorrent with the average time zone offset for each developer, collected from a small random sample of their commits after cloning repositories locally. We then separate our survey participants into two groups, *Office Hours* (more likely paid contributors) and *Nights and Weekends* (more likely volunteers), based on whether they perform more or less relative amount in the office hour window described above than average (average *indexW orkHours* = 0*.*6; design following prior research [\[39](#page-12-11)]).

*Support Activity:* We also measured *indexSupport* as the percentage of support activities among all activities, i.e., all non-commit GHTorrent events related to managing issues and pull requests. We distinguish between *High Support Work* and *Low Support Work* relative to the mean (*indexSupport* = 0*.*2).

Note that given the different ways in which we aggregate the survey responses and the relatively small sample size overall, we cannot draw sound statistical conclusions about differences between the (sub)groups. While we report exact numbers, readers should focus on qualitative differences.

*Threats to Survey Validity.* As usual for surveys, our results may be affected by a selection bias: contributors who did not answer may have had different

| Subgroup                                       | Count | Office Hrs                            | More Support                          |
|------------------------------------------------|-------|---------------------------------------|---------------------------------------|
| Occupational reasons                           |       | vs Nights&We                          | vs Less                               |
| Got new job that doesn't support FLOSS         | 37    |                                       |                                       |
| Changed role/project                           | 25    |                                       |                                       |
| Left job where they contributed to FLOSS       | 16    |                                       |                                       |
| No time: new job                               | 15    |                                       |                                       |
| No time: existing job                          | 10    |                                       |                                       |
| Left school where they contributed to FLOSS    | 12    |                                       |                                       |
| No time: in school                             | 12    |                                       |                                       |
| FLOSS in school, now job doesn't support FLOSS | 7     |                                       |                                       |
| Too much coding at work                        | 4     |                                       |                                       |
| Social reasons                                 |       |                                       |                                       |
| Lost interest in FLOSS                         | 24    |                                       |                                       |
| No time: personal                              | 23    |                                       |                                       |
| Lack of peer support                           | 16    |                                       |                                       |
| No time: nondescript                           | 15    |                                       |                                       |
| Technical reasons                              |       |                                       |                                       |
| Issues w GitHub or industry                    | 14    |                                       |                                       |
| Individually moved to private repos            | 12    |                                       |                                       |
| Changed platform                               | 10    |                                       |                                       |
| Feature complete project                       | 3     | 30<br>20<br>10<br>0<br>10<br>20<br>30 | 30<br>20<br>10<br>0<br>10<br>20<br>30 |

<span id="page-5-0"></span>**Table 1.** Self-reported reasons for disengagement in survey

reasons for disengaging. To identify contributors who had disengaged, we used public GitHub data, which covers much but not all open source activities, as also visible in 10 (of 151) survey responses that indicate changing platforms. Deriving the survival model data from survey participants enabled modeling only contributors confirmed to have disengaged. Note that we consider moving to private repositories (12 answers) still as disengagement from public open source activities. Furthermore, our approach to identify disengagement looks for sudden disengagement (within a six-month window) and results may not generalize to contributors who disengage more gradually. Contributors may also deliberately or unconsciously self-censor in their answers, providing socially acceptable reasons rather than real—a common concern in turnover research [\[31](#page-12-4)]. Note however, that our survival model (discussed later) is built entirely on historic trace data rather than self-reported answers, and thus reduces this threat.

## **4.2 Results from Survey**

In Table [1,](#page-5-0) we show the survey results. The most common self-reported reason for disengagement was changing jobs to a job that does not support open source work and occupational reasons were generally the most frequent.

Furthermore, we observe differences across populations: *Contributors who work nights and weekends tend to disengage for different reasons than those who work during office hours:* contributors who worked nights and weekends most commonly cited social reasons, whereas those who worked during office hours most commonly cited occupational reasons; the largest difference is between those who cited *Left job where they contributed to OSS*, with 19% and 0% citing it respectively.

Next, we turn to the aggregation by type of work, noting *Contributors who do less support work tend to disengage for different reasons than those who do more:* In particular, only 67% of the *More Support Work* group cited at least once Occupational reason, compared to 72% of the *Less Support Work* group. The difference between these two groups may be because since they are less stressed when major life changes occur (i.e., getting a new job or leaving school), they are better able to cope with transitions.

Finally, we emphasize a surprising result. For all contributors, occupational reasons such as major life changes (e.g., getting a new job or leaving school) were the most cited (with 106 citations), significantly more than lacking peer support or losing interest that are more commonly discussed in the literature. This motivated us to consider transitions explicitly in our survival analysis below.

# <span id="page-6-0"></span>**5 Modeling Disengagement Factors (Survival Analysis)**

## **5.1 Survival Model Methodology**

We use survival analysis to triangulate the survey results and model the relative strengths of the effects of the three main factors emerging from the survey analysis on the risk of disengagement from public GitHub activity (Work Hours vs Nights and Weekends; High Support Work vs Low Support Work; and Job Transitions). Survival analysis is a statistical modeling technique that specializes in time-to-event data [42], particularly suited for modeling right censored data. In our study, the event is public GitHub disengagement; right censorship can occur for contributors whose last recorded event may be very close to the end of the observation period, for which it is not clear whether they will return to contribute more. In particular, we use a Cox Proportional Hazards regression model [13]. The estimated regression coefficients describe each variable's hazard ratio (HR), which is analogous to an odds ratio in for multiple logistic regression analysis. Briefly, an HR > 1 indicates an increased risk of observing the event, and an HR < 1 indicates a decreased risk, relative to a one unit change in a predictor variable (or flipping the value, in case of binary variables), while holding all other predictors constant.

Data. We collect GitHub data on several variables for the open source contributors who disengaged and responded to our survey (the 'treatment' group), as well as for an equal sized 'control' group of contributors who did not disengage. With this design, a survival model estimates which factors are statistically useful for distinguishing groups.

For job transition data, we collect publicly available CV data from contributors by following links on their GitHub profiles. Since our data collection is not yet fully automated, we can currently only assemble a dataset of moderate size, therefore we only collected data for our survey participants (plus the control group), because their survey answers validate that they actually disengaged. For non-CV data, we use GHTorrent (Sect. 4). We discard 34 participants for which we cannot find CVs or similar information from which we can deduce past transitions, leaving us with a dataset of 206 contributors of which 103 disengaged. By construction, both groups contributed actively for 18 months (at least 100 commits per six-month period for three consecutive periods; Sect. 4); the 'control' group contributors then remained active for at least another six months at similar levels or higher, while the 'treatment' group contributors made at most five commits in the following period, i.e., they disengaged.

#### Model Factors and Operationalization. We compute:

- Activity level: Prior work has shown that more active contributors are less
  likely to disengage [11], hence we control for the average quarterly activity
  level by counting all activities (commits and support) per person.
- Working hours and support: We use the two factors indexWorkHours and index-Support as introduced in Sect. 4.1 to characterize the degree of work outside regular working hours (more likely volunteers) and the degree of support activities, both identified as stressors by practitioners (cf. Sect. 2). We compute dummy variables indicating being above or below the mean.
- Organizational affiliation: Previous research has shown that on a project scale, having an organizational affiliation can help increase developer retention rates [58]. We test whether organizational affiliation has the same affect

on engagement on an individual scale as it does on a project scale. Using GHTorrent, we record whether contributors had an Organizational Affiliation listed on their GitHub public profile.

- *Team size:* Turnover research regularly reveals social embedding in a team as an antidote to turnover [\[19\]](#page-11-0). We operationalize this as the number of contributors per project. Since a contributor may be part of multiple projects, we consider only their main projects (for a contributor, taking all projects with the highest number of contributions that together constitute at least 50% of all contributions) and record the average team size among those projects. 'Teams' comprise everyone who authored at least one commit.
- *Project popularity:* To control for whether contributors are more likely to disengage from small or very popular projects, we use the number of stars a project has on GitHub as a proxy for its popularity (standard measure in GitHub research [\[16](#page-11-17)]). We model popularity in addition to activity level because previous research has shown that the popularity of a project influences its survival probability [\[53](#page-13-0)], and we are interested in whether the popularity of a project also affects the survival probability of its contributors on an individual level. For contributors working on multiple projects, we consider the max popularity of the contributor's active projects (see team size).
- *Transition found:* Finally, to operationalize a contributor's transition data, identified as very important in our survey, we went to their linked publicly available CV and created a binary variable that recorded whether there was a transition present in the last year or not. We considered a transition to be either the stopping or starting of a job or educational program.

*Model Diagnostics.* We performed the standard model diagnostics: We log transformed variables with highly skewed distributions, as necessary, to reduce heteroscedasticity [\[23](#page-11-18)]. We tested for multicollinearity using the variance inflation factor (VIF *<* 3) [\[10](#page-10-8)]. We also inspected Schoenfeld residual plots to graphically diagnose Cox regression modeling assumptions [\[28\]](#page-11-19).

*Threats to Model Validity.* Regarding the survival model, statistical power is limited by the small sample size, which is limited by our design of modeling only survey participants with public CV data (due to confirming disengagement with the survey and manual effort required, as discussed). Since our treatment group was limited to the survey respondents, our survival model also has the risk of suffering from selection bias. As usual, our operationalization of factors in our survival model can only capture part of the concept to be measured. While we experimented with different operationalizations of our factors to ensure construct validity and robustness, one needs to be careful in generalizing our results beyond our specific operationalizations.

### **5.2 Results from Survival Modeling**

Table [2](#page-9-0) presents the results from the two survival models created; a base model without the novel transition found variable, and a full model with.

| Base model     |          | Full model     |          |
|----------------|----------|----------------|----------|
| 0.36 (0.21)∗∗∗ | 29.00∗∗∗ | 0.36 (0.21)∗∗∗ | 27.92∗∗∗ |
| 0.90 (0.21)    | 0.27     | 0.92 (0.21)    | 0.17     |
| 1.17 (0.08)    | 3.59     | 1.17 (0.08)    | 3.41     |
| 0.85 (0.05)∗∗  | 10.01∗∗  | 0.86 (0.05)∗∗  | 9.08∗∗   |
| 1.29 (0.26)    | 0.96     | 1.43 (0.27)    | 1.74     |
| 1.56 (0.21)∗   | 4.52∗    | 2.20 (0.30)∗∗  | 5.59∗    |
|                |          | 2.48 (0.31)∗∗  | 8.15∗∗   |
|                |          | 0.55 (0.42)    |          |
| 0.21           |          | 0.25           |          |
|                |          |                |          |

<span id="page-9-0"></span>**Table 2.** Survival models for contributor disengagement.

The *base model* had a goodness of fit of R<sup>2</sup> = 0*.*21. The controls behave as expected. *Total activity* had a hazard rate of 0.36, meaning it decreases a contributor's risk of disengaging by a factor of 0.38. Similarly, contributors who work on more popular projects are less likely to disengage (*Max number of stars* has a hazard ratio of 0.85).

As predicted based on previous research, the *workHours* dummy affects a contributor's risk of disengaging, having a hazard ratio of 1.56. This suggests that working during business hours more than the average contributor increases the risk of disengaging by a factor of 1.56. Surprisingly, we do not observe any statistically significant effects of doing more support work than average (the *highSupportWork* dummy), perhaps due to our operationalization or relatively small sample size.

The *full model* fits the data better (R<sup>2</sup> = 0*.*25), meaning that adding in the *jobTransition* variable helped increase the explanatory power of the model. The *jobTransition* variable has a hazard ratio of 2.48, meaning, as suggested by the survey results, that experiencing a transition significantly increases a contributor's risk of disengagement by a factor of 2.48.

# **6 Discussion and Conclusions**

In this research, we have looked at the reasons why established open source contributors disengage, using a survey with 151 responses and a survival model to quantify factors which predict disengagement. From the grouped analysis of survey results, we learned that the *Nights and Weekends* and *Office Hours* groups tend to cite different reasons for their disengagement, and so do more the *Less Support Work* and *More Support Work* groups.

Importantly, our study shows that operationalizations of different disengagement risk factors using publicly observable trace data are plausible. For example, since occupational reasons were the most commonly cited, we used online public CVs to operationalize the *jobTransition* variable; however, other commonly

<sup>∗∗∗</sup>*p <* 0*.*001, ∗∗*p <* 0*.*01, <sup>∗</sup>*p <* 0*.*05

cited reasons from the survey may also be operationalizable. Another commonly cited reason was 'no time, personal circumstance', more specifically people often cited having children or getting married. Such circumstances may be observable on social networking platforms. This suggest that a data-driven systems could be developed to help identify at-risk groups on a significantly larger scale, instead of having to rely on relatively expensive survey data. This information could be useful to different stakeholders, such as open source foundations and other funding agencies, looking to target support interventions. Overall, support interventions targeted more appropriately could significantly increase the sustainability of open source ecosystems.

We aim to work on these extensions of the research and more, to better understand the reasons why different kinds of established contributors disengage, since defining the problem is the first step to solving it [\[3\]](#page-10-9).

**Acknowledgements.** This work was supported through CMU's REU in SE, NSF (1318808, 1552944, 1717022, and 1717415), and AFRL and DARPA (FA8750-16-2- 0042). We thank our survey participants, and colleagues at CMU, especially Jim Herbsleb, Chris Bogart, Marat Valiev, and Sophie Rosas-Smith.

# **References**

- <span id="page-10-5"></span>1. Bannai, A., Tamakoshi, A.: The association between long working hours and health: a systematic review of epidemiological evidence. Scand. J. Work Environ. Health **40**, 5–18 (2014)
- <span id="page-10-7"></span>2. Barcomb, A., Kaufmann, A., Riehle, D., Stol, K.-J., Fitzgerald, B.: Uncovering the periphery: a qualitative survey of episodic volunteering in free/libre and open source software communities. IEEE Trans. Softw. Eng. (2018)
- <span id="page-10-9"></span>3. Bardach, E., Patashnik, E.M.: A Practical Guide for Policy Analysis: The Eightfold Path to More Effective Problem Solving. CQ Press, Washington D.C. (2015)
- <span id="page-10-6"></span>4. Binnewies, C., Sonnentag, S., Mojza, E.J.: Recovery during the weekend and fluctuations in weekly job performance: a week-level study examining intra-individual relationships. J. Occup. Org. Psychol. **83**(2), 419–441 (2010)
- <span id="page-10-3"></span>5. Bonaccorsi, A., Rossi, C.: Comparing motivations of individual programmers and firms to take part in the open source movement: from community to business. Knowl. Technol. Policy **18**(4), 40–64 (2006)
- <span id="page-10-2"></span>6. Burton, J.P., Holtom, B.C., Sablynski, C.J., Mitchell, T.R., Lee, T.W.: The buffering effects of job embeddedness on negative shocks. J. Vocat. Behav. **76**(1), 42–51 (2010)
- <span id="page-10-4"></span>7. Canfora, G., Di Penta, M., Oliveto, R., Panichella, S.: Who is going to mentor newcomers in open source projects? In: Proceedings of International Symposium Foundations of Software Engineering (FSE), p. 44. ACM Press, New York (2012)
- <span id="page-10-1"></span>8. Claes, M., M¨antyl¨a, M.V., Kuutila, M., Adams, B.: Do programmers work at night or during the weekend? In: ICSE, pp. 705–715. ACM (2018)
- <span id="page-10-0"></span>9. Coelho, J., Valente, M.T.: Why modern open source projects fail. In: ESEC/FSE, pp. 186–196. ACM (2017)
- <span id="page-10-8"></span>10. Cohen, P., West, S.G., Aiken, L.S.: Applied Multiple Regression/Correlation Analysis for the Behavioral Sciences. Psychology Press, London (2014)

- <span id="page-11-8"></span>11. Constantinou, E., Mens, T.: An empirical comparison of developer retention in the RubyGems and NPM software ecosystems. Innov. Syst. Softw. Eng. **13**(2–3), 101–115 (2017)
- <span id="page-11-1"></span>12. Constantinou, E., Mens, T.: Socio-technical evolution of the Ruby ecosystem in GitHub. In: SANER, pp. 34–44. IEEE (2017)
- <span id="page-11-16"></span>13. Cox, D.R.: Analysis of Survival Data. Routledge, Abingdon (2018)
- <span id="page-11-12"></span>14. Creswell, J.W., Clark, V.L.P.: Designing and Conducting Mixed Methods Research. Wiley, Hoboken (2007)
- <span id="page-11-14"></span>15. Crowston, K., Annabi, H., Howison, J., Masango, C.: Effective work practices for software engineering: free/libre open source software development. In: Proceedings of the 2004 ACM Workshop on Interdisciplinary Software Engineering Research, pp. 18–26. ACM (2004)
- <span id="page-11-17"></span>16. Dabbish, L., Stuart, C., Tsay, J., Herbsleb, J.: Social coding in GitHub: transparency and collaboration in an open software repository. In: Proceedings of the ACM 2012 Conference on Computer Supported Cooperative Work, pp. 1277–1286. ACM (2012)
- <span id="page-11-9"></span>17. Eyolfson, J., Tan, L., Lam, P.: Do time of day and developer experience affect commit bugginess? In: Proceedings of the 8th Working Conference on Mining Software Repositories, pp. 153–162. ACM (2011)
- <span id="page-11-6"></span>18. Fagerholm, F., Guinea, A.S., Borenstein, J., M¨unch, J.: Onboarding in open source projects. IEEE Softw. **31**(6), 54–61 (2014)
- <span id="page-11-0"></span>19. Fang, Y., Neufeld, D.: Understanding sustained participation in open source software projects. J. Manag. Inf. Syst. **25**(4), 9–50 (2009)
- <span id="page-11-3"></span>20. Feldman, D.C., Ng, T.W.H.: Careers: mobility, embeddedness, and success. J. Manag. **33**(3), 350–377 (2007)
- <span id="page-11-2"></span>21. Foucault, M., Palyart, M., Blanc, X., Murphy, G.C., Falleri, J.-R.: Impact of developer turnover on quality in open-source software. In: ESEC/FSE, pp. 829–841. ACM (2015)
- <span id="page-11-10"></span>22. Fucci, D., Scanniello, G., Romano, S., Juristo, N.: Need for sleep: the impact of a night of sleep deprivation on novice developers' performance. IEEE Trans. Softw. Eng. (2018)
- <span id="page-11-18"></span>23. Gelman, A., Hill, J.: Data Analysis Using Regression and Multilevel/Hierarchical Models. Cambridge University Press, Cambridge (2006)
- <span id="page-11-5"></span>24. Ghosh, R.A., Glott, R., Krieger, B., Robles, G.: Free/libre and open source software: survey and study - part 4: survey of developers. Technical report, International Institute of Informatics, University of Maastricht, Maastricht (2002)
- <span id="page-11-4"></span>25. Gidron, B.: Predictors of retention and turnover among service volunteer workers. J. Soc. Serv. Res. **8**(1), 1–16 (1985)
- <span id="page-11-13"></span>26. Gousios, G.: The GHTorent dataset and tool suite. In: MSR, pp. 233–236. IEEE (2013)
- <span id="page-11-15"></span>27. Gousios, G., Zaidman, A., Storey, M.-A., Van Deursen, A.: Work practices and challenges in pull-based development: the integrator's perspective. In: ICSE, pp. 358–368. IEEE (2015)
- <span id="page-11-19"></span>28. Grambsch, P.M., Therneau, T.M.: Proportional hazards tests and diagnostics based on weighted residuals. Biometrika **81**(3), 515–526 (1994)
- <span id="page-11-11"></span>29. Guzman, E., Az´ocar, D., Li, Y.: Sentiment analysis of commit comments in GitHub: an empirical study. In: Proceedings of the 11th Working Conference on Mining Software Repositories, pp. 352–355. ACM (2014)
- <span id="page-11-7"></span>30. Hannebauer, C., Gruhn, V.: On the relationship between newcomer motivations and contribution barriers in open source projects. In: Proceedings of International Symposium on Open Collaboration, OpenSym 2017, pp. 2:1–2:10. ACM, New York (2017)

- <span id="page-12-4"></span>31. Hom, P.W., Lee, T.W., Shaw, J.D., Hausknecht, J.P.: One hundred years of employee turnover theory and research. J. Appl. Psychol. **102**(3), 530 (2017)
- <span id="page-12-14"></span>32. Homscheid, D., Schaarschmidt, M.: Between organization and community: investigating turnover intention factors of firm-sponsored open source software developers. In: Proceedings of Conference Web Science (WebSci), pp. 336–337. ACM, New York (2016)
- <span id="page-12-2"></span>33. Izquierdo-Cortazar, D., et al.: Using software archaeology to measure knowledge loss in software projects due to developer turnover. In: HICSS, pp. 1–10. IEEE (2009)
- <span id="page-12-8"></span>34. Jamison, I.B.: Turnover and retention among volunteers in human service agencies. Rev. Publ. Pers. Adm. **23**(2), 114–132 (2003)
- <span id="page-12-5"></span>35. Kim, H., Kao, D.: A meta-analysis of turnover intention predictors among us child welfare workers. Child. Youth Serv. Rev. **47**, 214–223 (2014)
- <span id="page-12-16"></span>36. Kuutila, M., M¨antyl¨a, M.V., Claes, M., Elovainio, M.: Reviewing literature on time pressure in software engineering and related professions: computer assisted interdisciplinary literature review. In: 2017 IEEE/ACM 2nd International Workshop on Emotion Awareness in Software Engineering (SEmotion), pp. 54–59. IEEE (2017)
- <span id="page-12-9"></span>37. Lakhani, K., Wolf, R.G.: Why hackers do what they do: understanding motivation and effort in free/open source software projects. Technical report, MIT Sloan Working Paper (2003)
- <span id="page-12-6"></span>38. Lee, T.W., Mitchell, T.R.: An alternative approach: the unfolding model of voluntary employee turnover. Acad. Manag. Rev. **19**(1), 51–89 (1994)
- <span id="page-12-11"></span>39. Lin, B., Robles, G., Serebrenik, A.: Developer turnover in global, industrial open source projects: insights from applying survival analysis. In: 2017 IEEE 12th International Conference on Global Software Engineering (ICGSE), pp. 66–75. IEEE (2017)
- <span id="page-12-12"></span>40. Midha, V., Palvia, P.: Retention and quality in open source software projects. In: AMCIS 2007 Proceedings, p. 25 (2007)
- <span id="page-12-7"></span>41. Miller, L.E., Powell, G.N., Seltzer, J.: Determinants of turnover among volunteers. Hum. Relat. **43**(9), 901–917 (1990)
- <span id="page-12-17"></span>42. Miller Jr., R.G.: Survival Analysis, vol. 66. Wiley, Hoboken (2011)
- <span id="page-12-13"></span>43. Qiu, H.S., Nolte, A., Brown, A., Serebrenik, A., Vasilescu, B.: Going farther together: the impact of social capital on sustained participation in open source. In: International Conference on Software Engineering, ICSE. IEEE (2019)
- <span id="page-12-1"></span>44. Roberts, J.A., Hann, I.-H., Slaughter, S.A.: Understanding the motivations, participation, and performance of open source software developers: a longitudinal study of the Apache projects. Manag. Sci. **52**(7), 984–999 (2006)
- <span id="page-12-15"></span>45. Rodriguez, A., Tanaka, F., Kamei, Y.: Empirical study on the relationship between developer's working habits and efficiency. In: Proceedings of Conference on Mining Software Repositories (MSR) (2018)
- <span id="page-12-3"></span>46. Schilling, A., Laumer, S., Weitzel, T.: Who will remain? An evaluation of actual person-job and person-team fit to predict developer retention in FLOSS projects. In: HICCS, pp. 3446–3455. IEEE (2012)
- <span id="page-12-18"></span>47. Schreier, M.: Qualitative Content Analysis in Practice. Sage Publications, Thousand Oaks (2012)
- <span id="page-12-10"></span>48. Shah, S.K.: Motivation, governance, and the viability of hybrid forms in open source software development. Manag. Sci. **52**(7), 1000–1014 (2006)
- <span id="page-12-0"></span>49. Sharma, P.N., Hulland, J., Daniel, S.: Examining turnover in open source software projects using logistic hierarchical linear modeling approach. In: Hammouda, I., Lundell, B., Mikkonen, T., Scacchi, W. (eds.) OSS 2012. IAICT, vol. 378, pp. 331– 337. Springer, Heidelberg (2012). [https://doi.org/10.1007/978-3-642-33442-9](https://doi.org/10.1007/978-3-642-33442-9_30) 30

- <span id="page-13-2"></span>50. Skoglund, A.G.: Do not forget about your volunteers: a qualitative analysis of factors influencing volunteer turnover. Health Soc. Work **31**(3), 217 (2006)
- <span id="page-13-8"></span>51. Sonnentag, S., Binnewies, C., Mojza, E.J.: Staying well and engaged when demands are high: the role of psychological detachment. J. Appl. Psychol. **95**(5), 965 (2010)
- <span id="page-13-5"></span>52. Steinmacher, I., Conte, T., Gerosa, M.A.: Redmiles, D.: Social barriers faced by newcomers placing their first contribution in open source software projects. In: Proceedings of Conference on Computer Supported Cooperative Work (CSCW), pp. 1379–1392. ACM, New York (2015)
- <span id="page-13-0"></span>53. Valiev, M., Vasilescu, B., Herbsleb, J.: Ecosystem-level determinants of sustained activity in open-source projects: a case study of the PyPI ecosystem. In: ESEC/FSE. ACM (2018)
- <span id="page-13-3"></span>54. Von Krogh, G., Haefliger, S., Spaeth, S., Wallin, M.W.: Carrots and rainbows: motivation and social practice in open source software development. MIS Q. **36**(2), 649–676 (2012)
- <span id="page-13-4"></span>55. West, J., Gallagher, S.: Challenges of open innovation: the paradox of firm investment in open-source software. R&D Manag. **36**(3), 319–331 (2006)
- <span id="page-13-7"></span>56. Yu, Y., Benlian, A., Hess, T.: An empirical study of volunteer members' perceived turnover in open source software projects. In: Proceedings of Hawaii International Conference on System Sciences (HICSS), pp. 3396–3405. IEEE (2012)
- <span id="page-13-1"></span>57. Zhou, M., Mockus, A.: Developer fluency: achieving true mastery in software projects. In: ESEC/FSE, pp. 137–146. ACM (2010)
- <span id="page-13-6"></span>58. Zhou, M., Mockus, A., Ma, X., Lu, Z., Mei, H.: Inflow and retention in OSS communities with commercial involvement: a case study of three hybrid projects. ACM Trans. Softw. Eng. Methodol. (TOSEM) **25**(2), 13 (2016)