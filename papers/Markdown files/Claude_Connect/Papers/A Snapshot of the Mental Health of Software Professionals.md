# A Snapshot of the Mental Health of Software Professionals

Eduardo Santana de Almeida, Ingrid Oliveira de Nunes, Raphael Pereira de Oliveira, Michelle Larissa Luciano Carvalho, Andre Russowsky Brunoni, Shiyue Rong, and Iftekhar Ahmed ´

**Abstract**—Mental health disorders affect a large number of people, leading to many lives being lost every year. These disorders affect struggling individuals and businesses whose productivity decreases due to days of lost work or lower employee performance. Recent studies provide alarming numbers of individuals who suffer from mental health disorders, *e.g.*, depression and anxiety, in particular contexts, such as academia. In the context of the software industry, there are limited studies that aim to understand the presence of mental health disorders and the characteristics of jobs in this context that can be triggers for the deterioration of the mental health of software professionals. In this paper, we present the results of a survey with 500 software professionals. We investigate different aspects of their mental health and the characteristics of their work to identify possible triggers of mental health deterioration. Our results provide the first evidence that mental health is a critical issue to be addressed in the software industry, as well as raise the direction of changes that can be done in this context to improve the mental health of software professionals.

✦

**Index Terms**—Software development, Mental Health, Mental Health disorder, Mental illness, Social and human factors.

**1 INTRODUCTION**

On the 28th of July, Simone Biles, considered the greatest gymnast of all time, shocked the world after she withdrew from the women's individual all-around final at the Tokyo Olympic Games to focus on her mental health[1](#page-0-0) . Simone Biles attitude is not an isolated case. According to a published report from American Psychological Association (APA) with emergent trends in psychology for 2021 [\[1\]](#page-10-0), the national mental health crisis is among the top 10.

This crisis has shown unsettling aspects: two-thirds of employees report that poor mental health has undercut their job performance during the COVID-19 pandemic, and 40% of employees are battling burnout. In addition, more than a third of Americans experienced clinical anxiety or depression symptoms. Employees' mental health struggles have an outsize impact on U.S. businesses also, with mental illness the leading cause of disability in the country, accounting for some 217 million days of lost work annually [\[2\]](#page-10-1).

The mental health crisis has affected many sectors of society such as sports, entertainment [\[3\]](#page-10-2), health care [\[4\]](#page-10-3), and information technology (IT) is not an exception since the software is literally "eating the world" [\[5\]](#page-10-4). Based on a study with Indian professionals, Nayak [\[6\]](#page-10-5) identified that software developers have a considerably higher chance of experiencing fatigue, burnout, anxiety, and stress, compared to colleagues who perform mechanical tasks.

In Stack Overflow's 2022 survey [\[7\]](#page-10-6), which included participation from nearly 70k developers, respondents ad-

*Manuscript received ...; revised...*

mitted having some type of mental issue, with memory disorder (10.6%), anxiety (10.3%) and depression (9.7%) being the most common ones. These results indicate a significant prevalence of mental issues among software professionals.

Existing research usually focuses on a diversity of aspects related to the job of software engineers [\[8\]](#page-10-7), [\[9\]](#page-10-8), their mental model [\[10\]](#page-10-9) and work habits [\[11\]](#page-10-10)–[\[15\]](#page-10-11), work conditions [\[16\]](#page-10-12), [\[17\]](#page-10-13), the need of sleep [\[18\]](#page-10-14), what makes a good day [\[19\]](#page-10-15), and their main motivations and satisfactions [\[20\]](#page-10-16), [\[21\]](#page-10-17).

Nevertheless, to the best of our knowledge, there are no studies reporting on the main aspects that affect the mental health of software professionals at work. Despite some reports [\[6\]](#page-10-5), [\[22\]](#page-10-18) of the occurrence of mental disorders such as depression and anxiety, very little is known about its prevalence among software professionals. In addition, human and social factors that directly impact the mental health of these individuals are also under-investigated.

This work aims to report the research findings of an investigation aimed at identifying the dimension of software professionals that suffer from mental disorders and the working context in which these individuals are more susceptible to developing them. We considered the working context into four directions: *(i)* the work of software professionals concerning position, role, and experience; *(ii)* work environment; *(iii)* schedule; and *(iv)* any tasks undertaken. However, it was also important to consider the mental health history of software professionals and the impact caused by the COVID-19 pandemic [\[23\]](#page-10-19)–[\[26\]](#page-10-20).

Thus, to obtain a broad understanding of mental health issues among software professionals, we investigated the following research questions (RQs):

**RQ1.** *What are the mental health disorders that affect software professionals, and what are their experiences associated with mental health?*

<sup>•</sup> *E. Almeida was with the Institute of Computing (IC-UFBA), Federal University of Bahia, Brazil. E-mail: esa@rise.com.br*

<sup>•</sup> *I. Ahmed and Shiyue Rong are with University of California, Irvine (UCI).*

<span id="page-0-0"></span><sup>1.</sup> https://edition.cnn.com/2021/07/28/sport/simone-bilesgymnastics-tokyo-2020-mental-health-spt-intl/index.html

**RQ2.** *What leisure and entertainment activities do software professionals engage?*

**RQ3.** *What are the characteristics in the work nature that are associated with triggers for mental health disorders?*

**RQ4.** *What are the characteristics in the work environment that might be triggers for mental health disorders?*

**RQ5.** *What are the characteristics in the work schedule that might be triggers for mental health disorders?*

In RQ1, we aimed to investigate the mental health disorders that are primarily present among software professionals. In addition, even when mental health disorders are not present, there might be indicators that professionals are concerned with their mental health, such as by doing psychotherapy or reading on the topic. This is also investigated in this research question. RQ2 is used to observe external factors that may affect the mental health of our study participants, such as the frequency in which they engage social activity or practice sports. This is relevant because this can be a confounding factor in the job-related triggers of mental health disorders. These triggers are then investigated in RQ3-5, which aimed to identify triggers related to the work nature (*e.g.*, type of work contract and position), work environment (*e.g.*, relationship with colleagues, and pressure to stay up-to-date), and work schedule (*e.g.*, amount of work hours, and unrealistic deadlines).

To answer our research questions, we surveyed 500 software professionals from 35 countries. The survey asked respondents to provide feedback on their mental health, work environment characteristics, and daily activities.

In summary, the main contributions of this paper are described as follows:

- We collected a set of evidence that show how software development work can affect the mental health of software professionals;
- We also report the dimension of software professionals that suffer from mental health disorders beyond the depression and/or anxiety levels of these professionals; and
- We provide information on how organizations can offer better working conditions. In addition, we identified which and how leisure activities can be used as preventive measures beyond contributing to the well-being of software engineers.

#### **2 BACKGROUND AND RELATED WORK**

According to World Health Organization (WHO)[2](#page-1-0) , Mental health is a state of well-being in which an individual realizes his or her abilities, can cope with the normal stresses of life, can work productively and can contribute to his or her community.

Multiple social, psychological, and biological factors determine a person's mental health level at any time. For example, poor mental health is also associated with stressful work conditions, unhealthy lifestyles, and physical illhealth.

Despite the increasing importance of mental health, there is evidence that individuals have been struggling with

<span id="page-1-0"></span>2. https://www.who.int/news-room/fact-sheets/detail/mentalhealth-strengthening-our-response

mental disorders in many contexts. A recent study by [\[27\]](#page-10-21) reported alarming numbers of incidence of *depression* and *anxiety* among graduate students. Anecdotal evidence also shows that these mental disorders are also present among academics [\[28\]](#page-10-22).

According to the manual of mental disorders of the American Psychiatric Association [\[29\]](#page-10-23), depressed individuals exhibit sad, empty, or irritable moods. Their ability to function is largely affected by somatic and cognitive changes. Anxiety, in turn, refers to disorders that share features of excessive fear and anxiety and related behavioral disturbances. As opposed to fear, which is an emotional response to a real or perceived imminent threat, anxiety is the anticipation of a future threat. Among the mental disorders, the most impairing, common, and costly is major depression. Previous studies indicate that circa 5–12% of males and 9–26% of females have at least one episode of depression over the course of their life [\[30\]](#page-10-24), [\[31\]](#page-10-25).

Despite the increasing importance that mental health has received in other contexts, the software engineering community has only recently paid attention to aspects that can affect the mental health of software professionals. In this section, we present the main work discussing these aspects.

#### **2.1 Depression and Anxiety in Software Development**

The software engineering field encompasses many social and human aspects [\[32\]](#page-10-26), [\[33\]](#page-10-27) that go beyond the technical aspects [\[34\]](#page-10-28). These factors pressure the professionals involved in the software development process in such a way that generates a high level of depression, and anxiety [\[6\]](#page-10-5), [\[33\]](#page-10-27). In general, software development is a highly collaborative process that includes large projects in terms of source code, developers, and users. In this sense, a major challenge facing software professionals is dealing not only with the high complexity of the technical aspects but also the human and social aspects that affect their performance at work [\[17\]](#page-10-13), [\[33\]](#page-10-27).

Psychotherapists state that software professionals often demonstrate feelings such as inadequacy, insecurity, low self-esteem, and dissatisfaction, resulting in problems in the social, marital, and sexual areas [\[6\]](#page-10-5). They also claim that these symptoms can manifest due to the work environment stemming from the growing demand for software that exceeds the capacity of software professionals. In addition, technology is changing fast, which makes it difficult for software professionals to keep updated at the same time as doing daily tasks at work [\[35\]](#page-10-29).

By interviewing systems analysts, Cohen [\[36\]](#page-10-30) observed psychological problems such as irritability, depression, tension, and severe fatigue.

To examine the relationships between job stressors and depressive symptoms, Haratani et al. [\[37\]](#page-10-31) surveyed software engineers and managers in Japan. Engineers had significantly higher depression scores than managers. After controlling for confounding variables, interpersonal conflict in the project team and lack of control were common significant stressors for each group. In managers, job overload and changes in computer technology are significantly associated with depressive symptoms.

Fujigaki [\[38\]](#page-10-32) conducted an observational study with ten male software engineers observing them every two weeks for five months. His goal was to conduct an observation of a time series of job-event/life events and depressive symptoms. The job events that were scored were the presence of time pressure/deadline, work overload, amount of work increase, responsibility increase, and trouble with clients.

Rajeswari and Anantharaman [\[35\]](#page-10-29) surveyed 156 software professionals from India to investigate factors that cause negative pressure on professionals. Ten key factors were identified. Fear of obsolescence and individual team interaction are two factors that explained twenty-five percent of the variance in the study, followed by the eight other factors, namely client interactions, work-family interface, role overload, work culture, technical constraints, family support to career, workload, and technical risk propensity.

Rocha and Debert-Ribeiro [\[39\]](#page-10-33) carried out a crosssectional study in two Brazilian companies with 636 system analysts to evaluate possible associations between working conditions and visual fatigue, mental and psycho-social health of systems analysts. They found that mental and psycho-social health aspects were associated with mental workload, difficulties with clients, strict deadlines, inadequate equipment, and work environment.

Nayak [\[6\]](#page-10-5) surveyed 50 mechanical engineers and 50 software engineers from India to understand the dimensions contributing to their well-being. The study identified that software professionals experience a high level of anxiety than mechanical professionals. On the other hand, no significant difference was found between software and mechanical professionals related to the psychological dimension of mental health.

Despite studies focusing on the consequences of professional practice in the software development area, there is a significant research gap related to the main aspects that affect the mental health of software professionals in the work context, mainly considering different countries and companies. In this sense, we conducted an investigation to collect evidence that contributes to understanding how software development work affects the mental health of professionals, especially considering aspects such as job characteristics, work environment, schedules, and tasks undertaken.

#### **3 SURVEY DESIGN AND METHODOLOGY**

To understand different aspects related to the mental health of software professionals, we conducted an online survey with 500 professionals. We designed our study as a crosssectional survey [\[40\]](#page-10-34), which involves collecting information from participants at one point in time.

#### **3.1 Survey Construction**

Based on our research questions, we created a 20-minute survey questionnaire composed of nine parts: (1) *Consent*: free and clarified consent term and consent to participate in the study; (2) *Personal Data*: questions related to the demographic characteristics of the participants; (3) *Mental Health History*: questions related to the participant mental health; (4) *Leisure Activities*: questions related to how the participants enjoy their free time; (5) *Job*: questions related to the characteristics of the nature of the job of participants (such

as their position, team, and stability); (6) *Work Environment*: questions related to the setup of the work environment; (7) *Schedule*: questions related to the time available for the participants to complete their task, pressure, and workload (in terms of time); (8) *Tasks*: questions related to the tasks performed by participants, such as whether they perceive value in what they do and the need for staying up-todate; and finally; (9) *Patient Health Questionnaire*: questions of a validated instrument to asses the current participants mental health. In the end, participants could also provide additional comments and provide their email in case they allowed us to contact them further or would like to receive the research results.

For selecting the questions to be included in the questionnaire related to software engineering, we used the demographic data typically collected in software engineering surveys and related studies, such as that by Johnson et al. [\[17\]](#page-10-13), who investigated the impact of the work environment on productivity and satisfaction. In addition, the authors that work on software engineering (and have experience as researchers and software engineers) first had a brainstorming session to identify possible questions. Then, they individually listed additional possible questions related to each topic. Next, all questions were assessed and possibly improved, discarded, or merged.

One of the authors, who is a psychiatrist, reviewed and provided feedback on the questionnaire. In addition, he selected possible validated instruments for our patient health questionnaire. Two instruments were considered: (i) CIS-R [\[41\]](#page-10-35), which diagnostic interview used for the National Survey of Psychiatric Morbidity in Great Britain; and (ii) PHQ-9 [\[42\]](#page-10-36), which is a reliable and valid measure of depression severity. While CIS-R, as opposed to PHQ-9, provides a diagnosis, it is long. Therefore, it could prevent participants from participating in the study. Both were assessed, and based on our pilot study (discussed as follows), PHQ-9 was selected. Due to space restrictions, we do not detail all questions in our questionnaire, which is available online.[3](#page-2-0)

### **3.2 Ethical Considerations**

As there is a stigma and mental health is considered a taboo where people struggling with mental health can feel different than other people or feel like no one else understands, before sharing our survey, we submitted it to our IRB to minimize legal risks and ensure participants felt comfortable answering honestly. Thus, first, we made our survey anonymous and confidential: we did not collect names or IP addresses. Next, all participants gave informed consent. Third, we collected emails only from participants who would like to receive the study results. Finally, we are unable to publish our full dataset since it contains (although anonymous) demographic data that can inadvertently identify participants.

#### **3.3 Survey Distribution**

**Survey platform.** Because of its simplicity and ease of use, we chose Google Forms to manage our survey. We scoped our study of mental health to software professionals around

<span id="page-2-0"></span>3. Survey Instrument. https://github.com/MentalHealthSE/survey

the world. All recruitment materials stated that the survey was optional, anonymous, and confidential. To mitigate participant self-selection bias, we stated that prior mental health issue was not required to participate. All data were collected between May-July 2021.

**Survey Pilot.** We piloted our survey with two software professionals from the industry to get feedback on the questions and their corresponding answers, the difficulties faced in answering the survey, and the time to finish it. As these pilot respondents were experts in the area, we also would like to know if we were asking the right questions. Next, we conducted another pilot study with two software developers (one from the open-source community and one from the industry). We conducted several iterations of the survey, rephrasing some questions and removing others to make the survey easier to understand and answer. Another concern in this stage was ensuring that the participants could finish it in 20-minutes. The pilot survey responses were used solely to improve the questions, and these responses were not included in the final results.

**Survey recruitment.** We followed a three-step approach to recruit survey respondents: initially, we posted survey information on personal accounts on social media (Twitter, LinkedIn, and Instagram). Next, the authors contacted potential respondents by email (convenience sampling) and asked them to share it with other potential respondents (snowballing). Because of this process, we could not track the total number of invitations.

**Survey data validation.** In total, we received 503 responses. We disqualified three responses: two responses that refused to participate and a repeated one, leading to 500 valid responses.

**Statistical Analysis.** After collecting the survey data, we used descriptive statistics and statistical tests to perform the analysis. For testing normality, we applied the Shapiro–Wilk Test [\[43\]](#page-10-37). In our analysis, Shapiro-Wilk Test showed a non normal distribution (*p-value* less than 0.05). Thus, we applied the Wilcoxon Test [\[44\]](#page-10-38) to identify significant statistical difference between samples and the Cohen's d test to measure the effect size [\[45\]](#page-10-39). Finally, to identify a correlation between variables, we applied Spearman's test [\[46\]](#page-11-0).

# **4 POPULATION CONTEXTUALIZATION**

Table [1](#page-4-0) overviews our study population. The ages of participants ranged from 18 to 69, with an average age of 31.8. The majority (82%) of our population are men which was similar to other studies in software engineering [\[15\]](#page-10-11). The participants spread out in 35 countries across four continents. The top three countries where the respondents come from are Brazil, Germany, and United States.

54% of participants have a Bachelor's degree and 32% have an advanced degree (Master/Ph.D.). The professional experience of these 500 respondents varies from no experience to 45 years, with an average of 9.2 years. The number of different companies which they worked ranged from 0 to 20 with an average of 3.8 companies.

Regarding relationship status, there is a balance: 31% are married and 30.2% single. Only 26.2% of participants are parents. 13% of parents live with one children and 12.4% live with two or three children.

# **5 SURVEY RESULTS**

This section describes the survey results. We organize the survey analysis around our research questions:

#### **5.1 RQ1: Mental Health of Software Professionals**

Overall, we find that 30.2% (151/500) of our participants were diagnosed with mental health disorders in the past or currently. As it can be seen in Figure [1,](#page-3-0) anxiety disorders and depression are representative: 103 participants had anxiety (20.6%) and 74 (14.8%) had depression.

It is important to highlight that these mental disorders are not isolated cases in some situations. 65 participants reported more than one mental disorder, and one participant reported being diagnosed with five mental disorders. The participants (P) also highlighted the impact on their work and relationship with co-workers:

✗*P 282: "Wanted to end my life. Ended up loosing my job instead.*"

✗*P 39: "Fear of meetings with my boss, sleep deprivation, and permanent stress. I had to take medicine.*"

✗*P 101: "Fell tired all the time. No disposition to social interaction.*"

#### **Observation 1**

30.2% (151/500) of our participants were diagnosed with mental health disorders in the past or currently. Anxiety (20.6%) and depression (14.8%) were the most representative disorders.

**PHQ-9 Classification.** The PHQ-9 is a multipurpose instrument for screening, diagnosing, monitoring and measuring the severity of depression. It is composed of nine questions which analyze different aspects of the patient over the last 2 weeks. Figure [2](#page-4-1) shows the distribution of the depression level of software professionals according to PHQ-9 classification.

In our population, 126 participants (25.2%) have moderately severe depression or severe depression. 69 participants (13.8%) had moderately severe depression which generally warrants treatment for depression using medication, therapy, or a combination of the two and 57 participants (11.4%) have severe depression which also warrants the same treatment.

An important remark is that analyzing the participants without any record of mental health disorders (349 partici-

![](_page_3_Figure_24.jpeg)

<span id="page-3-0"></span>Fig. 1. Mental Health Disorders among Software Professionals.

TABLE 1 Demographic characteristics of the participants (number and percentage, N = 500).

<span id="page-4-0"></span>

| Age (Years)      | 18–25       | 115 (23%)   | 26–35       | 238 (48%)   | 36–45             | 115 (23%)   | 46–55            | 26 (5%)    | 55+      | 6 (1%)      |
|------------------|-------------|-------------|-------------|-------------|-------------------|-------------|------------------|------------|----------|-------------|
| Gender           | Female      | 84 (16.8%)  | Male        | 410 (82%)   | NA                | 4 (0.8%)    | Other            | 2 (0.4%)   |          |             |
| Country of Res.  | Brazil      | 374 (74.8%) | Germany     | 17 (3.4%)   | USA               | 17 (3.4%)   | France           | 16 (3.2%)  | Other    | 76 (15.2% ) |
| Education        | Less than   | 2 (0.4%)    | Graduated   | 46 (9%)     | Bachelor's        | 270 (54%)   | Trade/technical  | 21 (4.2%)  | Advanced | 161 (32.2%) |
|                  | high school |             | high school |             | degree            |             | school           |            | degree   |             |
| Exp. (Years)     | 0–2         | 85 (17%)    | 3–5         | 123 (24.6%) | 6–10              | 115 (23%)   | 10–15            | 87 (17.4%) | 15+      | 90 (18%)    |
| Exp. (Companies) | 0–2         | 168 (33.6%) | 3–5         | 236 (47.2%) | 6–8               | 69 (13.8%)  | 9–13             | 20 (4%)    | 13+      | 7 (1.4%)    |
| Rel. Status      | Married     | 155 (31%)   | Single      | 151 (30.2%) | In a relationship | 104 (20.8%) | In a civil union | 44 (8.8%)  | Other    | 46 (9.2%)   |
| Parent           | No          | 369 (73.8%) | Yes         | 131 (26.2%) |                   |             |                  |            |          |             |
| Children         | 0           | 373 (74.6%) | 1           | 65 (13%)    | 2–3               | 62 (12.4%)  |                  |            |          |             |

pants - 69.8%), we found that according to PHQ-9 classification, 75 participants (21.5%) had moderate depression, 42 participants had moderately severe depression (12%) and 26 (7.4%) participants had severe depression.

#### **Observation 2**

25.2% (126/500) of our participants were diagnosed with moderately severe depression or severe depression, which generally warrants treatment for depression using medication, therapy, or a combination of the two. Moreover, 68 participants (19.4%) without any record of mental health disorders were diagnosed with moderately severe depression or severe depression.

**Mitigation strategies.** Software professionals have used different ways to deal with mental health disorders. 249 participants (50%) have already done therapy from which 104 (21%) currently do to mitigate the consequences of mental health disorders. 346 participants (69%) have already searched the web for mental health information. YouTube, Medium and Reddit are the top 3 places to find information related to mental health. The participants (184 - 37%) also read book, the majority of them (95 - 52%) read 1-2 books related to mental health. An worrisome aspect is that 107 participants (21.4%) have already taken drugs, 39 (8%) without medical prescription.

**COVID-19 pandemic.** Different studies in software engineering [\[23\]](#page-10-19)–[\[26\]](#page-10-20) have discussed the impact of COVID-19 in software development. In our study, 286 respondents (57%) said that the pandemic period impacted negatively their mental health. 153 respondents were not affected and 35 respondents (7%) said that during the pandemic their mental health improved.

![](_page_4_Figure_9.jpeg)

<span id="page-4-1"></span>Fig. 2. Depression Levels of Software Professionals according to PHQ-9 classification.

# **5.2 RQ2: Leisure and Entertainment Activities**

Different studies have indicated the long-term benefits of leisure and entertainment activities on mental health and well-being [\[47\]](#page-11-1)–[\[49\]](#page-11-2) of unemployed and employed workers in general. We investigated which leisure and entertainment activities software professionals engage and how the COVID-19 pandemic impacted them, since during the pandemic different restrictions and lockdown were imposed around the world.

Before the pandemic, 388 participants (77.6%) said they performed physical exercise (walking, running, swimming, and so on) sometimes (99 - 19.8%), usually (144 - 28.8%), or always (145 - 29%). Regarding social activities, which involved meet friends and go out to restaurants and bars, 435 participants (87%) reported they sometimes (162 - 32.4%), usually (166 - 33.2%), or always (107 - 21.4%) engage them.

445 participants (89%) sometimes (155 - 31%), usually (185 - 37%), or always (105 - 21%) dedicate some time to hobbies, such as cooking, reading, playing an instrument, and so on. Finally, we investigated also how the software professionals spend time with family without any concern related to the job activities. 404 participants (80.8%) reported that they sometimes (118 - 23.6%), usually (178 - 35.6%), or always (108 - 25.6%) spend time with family.

Figure [3](#page-5-0) shows how software professionals engaged in leisure and entertainment activities before and during the pandemic and Table [2](#page-4-2) reports the comparison statistics results.

TABLE 2 Before x During Activities and Leisure Results.

<span id="page-4-2"></span>

| Activity / Leisure | Wilcoxon (p-value) | Cohen's d                  | In favor of |
|--------------------|--------------------|----------------------------|-------------|
| Physical exercise  | 2.2e-16            | 0.68 [0.56, 0.81] (medium) | Before      |
| Social activities  | 2.2e-16            | 1.97 [1.81, 2.12] (large)  | Before      |
| Hobbies            | 1.537e-09          | 0.40 [0.27, 0.52] (small)  | Before      |
| Time with family   | 2.567e-08          | 0.36 [0.24, 0.49] (small)  | Before      |

# **Observation 3**

During the COVID-19 pandemic, software professionals reduced the amount of physical exercises, social activities, hobbies and engagement with family members.

**No History x History.** Table [3](#page-5-1) shows the significant statistics results when comparing the participants *without history* of mental health disorders (349/500) and participants *with history* of mental health disorders (151/500) before and during the pandemic.

![](_page_5_Figure_2.jpeg)

<span id="page-5-0"></span>Fig. 3. Summary of Leisure and Entertainment Activities before and during the pandemic. BC= Before Covid and DC= During Covid

TABLE 3 No History x History Results.

<span id="page-5-1"></span>

| Period | Activity / Leisure | Wilcoxon (p-value) | Cohen's d                    | In favor of |
|--------|--------------------|--------------------|------------------------------|-------------|
|        | Physical exercise  | 0.01086            | -0.22 [-0.41, -0.03] (small) | No history  |
| Before | Hobbies            | 0.02926            | -0.21 [-0.40, -0.02] (small) | No history  |
|        | Time with family   | 1.133e-06          | -0.49 [-0.68, -0.30] (small) | No history  |
| During | Time with family   | 0.005383           | -0.27 [-0.47, -0.08] (small) | No history  |

# **Observation 4**

Before the pandemic, software professionals *with history* of mental health disorders did less physical exercise and had less hobbies. Moreover, before and during the pandemic this group also spent less time with their family.

# **5.3 RQ3: Work Nature**

Previous studies [\[50\]](#page-11-3) have identified that the level of occupational stress workers tend to feel directly correlates to the size of the business they are employed by. According to the study, micro businesses employing a maximum of four members of staff had the lowest instances of workers reporting job related stress of companies of any other size.

In our study, we investigated organization size and other aspects related to work nature which could be triggers for mental health disorders, such as the team size, the work type, and the employees role in a project.

**Organization size.** From our population, we find that 42.2% of respondents work for organizations with 1000 or more employees, 20.4% of the participants work for organizations with 100-499 employees, 16.6% of the respondents work for organizations with 10-99 employees, 9.2% of the respondents work for organizations with 500-999 employees, and 5.6% of the participants work for organizations with 0-9 employees. 4.6% and 1.4% of respondents, respectively, did not know or were not applicable.

Analyzing the participants with history of mental health disorders (151/500) and each organization size (0-9, 10-99, 100-499, 500-999, 1000 or more, Do not know), we did not find any correlation after applying the Spearman's test (all the *p*-values were ≥ 0.05).

**Team size.** Different studies in software engineering have discussed the impact of team size on software development effort [\[51\]](#page-11-4), cost [\[52\]](#page-11-5), and productivity [\[53\]](#page-11-6). While Scrum methodology [\[54\]](#page-11-7) and companies like Amazon (Jeff Bezos's two-pizza rule[4](#page-5-2) ) advocate the adoption of small teams for better communication and collaboration, no study has investigated the impact of team size on mental health.

From our survey, we found that 71% of respondents work in teams with 1-10 members, 15.6% of the participants work in teams with 11-20 members, 3.6% of respondents work in teams with 31 or more members, 2.8% of the participants work in teams 21-30 members, and 7% was not applicable. After applying the Spearman's test to identify a correlation between the participants with history of mental health disorders (151/500) and each one of the team sizes (1- 10, 11-20, 21-30, 31 or more), we did not find any significant correlation (all the *p*-values from Spearman's test were ≥ 0.05).

**Work type.** As software professionals can work in different ways (freelancer, open-source project, private organization, and so on), we investigated whether specific work types could impact in some way their mental health. 92.7% (464/500) of our participants work for an organization, 13% of participants contribute to open-source projects, 11.4% of participants work as freelancer, 1.8% of participants were unemployment, and 4.6% were not applicable.

<span id="page-5-2"></span>4. https://docs.aws.amazon.com/whitepapers/latest/introductiondevops-aws/two-pizza-teams.html

Considering the participants with history of mental health disorders (151/500) and each one of the work types (*organization*, *freelancer*, *OSS*, *unemployed*, *other*), we applied the Spearman's test and we found a significant correlation between *organization* and participants with mental health disorders (*p*-value = 0.02). However, the correlation was negative (*rho* = -0.10), implying that if the number of participants working in a organization increase, the number of participants with history of mental health disorders decrease. Regarding *freelancer*, we found a significant (*p*-value = 0.03) and positive (*rho* = 0.09) correlation with participants with mental health disorders. Thus, we found that *freelancer* is a trigger to mental health disorders.

**Roles.** Previous research in psychology [\[55\]](#page-11-8), [\[56\]](#page-11-9) has suggested over the decades that job characteristics and role stressors are related to the measures of job-related mental health, such as work dissatisfaction, burnout, and depression. Role stress is the stress experienced by workers because of their role (job) in the organization. In a software development project, software professionals act in different roles with specific activities, responsibilities and concerns. In our survey, we investigated the possible impact of roles on mental health. Unlike other areas [\[57\]](#page-11-10)–[\[60\]](#page-11-11) few is known about this aspect in software development.

78.2% (391/500) of our respondents work as software engineers, 20.4% of respondents work as software architects, 14.4% of respondents work as project managers, 9.6% of respondents work as requirements analysts, 7.6% of respondents work as test engineers, and 10.8% of respondents work in other roles, such as data scientist, head of quality assurance, and so on.

After applying the Spearman's test to identify correlations between the participants with history of mental health disorders (151/500) and each one of the roles (*Product Manager*, *Requirements Analyst*, *Software Architect*, *Software Engineer/Programmer*, *Test Engineer*, *Other*), we did not find any significant correlation for *Product Manager*, *Requirements Analyst*, *Software Architect*, *Software Engineer/Programmer*, and *Other* (all p-values were ≥ 0.05). However, we found a significant (*p*-value = 0.0004) and positive (*rho* = 0.15) correlation after applying the Spearman's test to check the correlation of participants with history of mental health disorders and *Test Engineer*. Hence, we found that the role of *Test Engineer* is associated with mental health disorders.

#### **Observation 5**

Analyzing software professionals with history of mental health disorders, we found that the work type (freelancer) and role (test engineer) are associated with mental health disorders.

#### **5.4 RQ4: Work Environment**

The connection between working conditions and mental health has been long conceptualized, discussed, and documented in the epidemiological, medical, and sociological literature [\[61\]](#page-11-12), [\[62\]](#page-11-13). The Mental Health Foundation (2021), for example, has recently recognized that working conditions and the environment can significantly affect mental health [\[62\]](#page-11-13). Recently, the software engineering area has also starting paying attention to effect of work environments on productivity and satisfaction of software engineers [\[17\]](#page-10-13). However, aspects related to mental health are not explored.

In our survey, we investigated which characteristics of the work environment (physical structure, leisure facilities, resting facilities, social activities, relationship with colleagues, and dissatisfaction with the job) can be triggers for mental health disorders.

**Physical work environment.** From our population, we find that before COVID-19, 42.4% of our participants worked in private workspaces, 37.2% of participants worked in open workspaces, 15.6% of participants worked in home office, and 4.8% of participants worked in other work environments, such as public spaces and coffee shops. The following are some feedback from participants' satisfaction regarding their physical work environment before COVID-19:

✓*P 64: "Frequent contact with different co-workers from different teams who helped in aspects related to innovation, motivation, and understanding of general goals of the organization.*"

✓*P 14: "Perfect place, nice landscape, infrastructure with places for drinking coffee and chat with colleagues, meeting rooms, video games, and good lighting.*"

✗*P 1: "Noise from parallel conversation, interruptions, and fix working hour.*"

✗*P 28: "Too many people. Uncomfortable chairs and tables. Long commute.*"

During the COVID-19 pandemic, 94.2% of our respondents worked in home office, 2.2% of respondents worked in private workspaces, 0.8% of respondents worked in open spaces, and 2.8 % of participants worked in hybrid environments (home office/private workspace, home office, coworking spaces).

On the overall satisfaction with the work environment, 68.8% of the survey respondents are satisfied with the working environment. 98, 48, and 9 respondents are neutral, dissatisfied, and very dissatisfied, respectively. The average Likert score for this statement is 3.79 (*i.e.*, between "Neutral" and "Satisfied").

#### **Observation 6**

68.8% of the survey respondents are satisfied with the working environment.

**Leisure and Resting facilities.** 341 participants work in organizations which provide leisure facilities (gym or game room). Nevertheless, 61% of these participants never used the leisure facilities. 62, 39, and 26 participants used rarely, sometimes, and usually, respectively. The average Likert score for this statement is 1.71 (*i.e.*, between "Never" and "Rarely").

Regarding resting facilities, 340 respondents work in organizations which provide resting facilities, such as massage or nap room. However, 60.88% of these respondents never used the resting facilities. 61, 40, and 19 respondents used rarely, sometimes, and usually, respectively. The average Likert score for this statement is 1.74 (*i.e.*, between "Never" and "Rarely").

### **Observation 7**

61% of the survey respondents never used the leisure facilities in their organizations. Regarding resting facilities, 60.88% of respondents never used them.

**Social Activities.** 412 participants work in organizations which organize social activities for their employees. However, 26.70% of these participants never participate in social activities. 73, 66, and 73 participants participated rarely, sometimes, and usually, respectively. The average Likert score for this statement is 2.90 (*i.e.*, between "Rarely" and "Sometimes").

#### **Observation 8**

26.70% of the survey respondents never participated in social activities organized by their company.

**Relationship with Colleagues.** We asked participants if they have a healthy relationship with their colleagues. Overall, 87% of the participants have a healthy relationship with their colleagues. 35, 8, and 3 respondents are neutral, disagree, and strongly disagree, respectively. The average Likert score for this statement is 4.40 (*i.e.*, between "Agree" and "Strongly Agree").

#### **Observation 9**

The majority of the survey respondents (87%) have a healthy relationship with their colleagues.

**Dissatisfaction with the Job.** We asked participants if they are always dissatisfied with their job. Overall, 35% of the participants disagreed with this statement. 123, 136, and 52 respondents are neutral, agree, and strongly agree, respectively. The average Likert score for this statement is 3.01 (*i.e.*, between "Neutral" and "Agree").

#### **Observation 10**

Several survey respondents (38%) are dissatisfied with their job.

After applying Spearman's test to correlate each one of the levels of work environment characteristics with participants with history of mental health disorders, we found five significant correlations shown in Table [5.](#page-7-0) The other tests (available online[5](#page-7-1) ) did not present a significant correlation.

#### **Observation 11**

Before COVID-19, working at home office represented a trigger for mental health disorders. Moreover, rarely frequency to social activities explicitly organized by the company represents a trigger as well. Also, survey respondents who are neutral or strongly agree with healthy relationships with colleagues, are less prone to have history of mental health disorders. Finally, survey respondents often dissatisfied with their job are more prone to have history of mental health disorders.

#### **5.5 RQ5: Work Schedule**

Evidence has shown that several types of job stressors, including workplace conditions, can influence the onset

<span id="page-7-1"></span>5. Survey Instrument. https://github.com/MentalHealthSE/survey

TABLE 4 Work Environment Correlation Results

| Working Environment      | Correlation with History   | Spearman's Test |         |  |
|--------------------------|----------------------------|-----------------|---------|--|
| Characteristics          | of Mental Health Disorders | p-value         | rho     |  |
|                          | Home Office                | 0.0049          | 0.1253  |  |
| Work                     | Open Workspace             | 0.7133          | 0.0164  |  |
| Environment              | Private Workspace          | 0.0298          | -0.0971 |  |
| [before COVID-19]        | Other                      | 0.5705          | -0.0254 |  |
|                          | Home Office                | 0.4648          | 0.0327  |  |
| Work                     | Open Workspace             | 0.1873          | -0.0590 |  |
| Environment              | Private Workspace          | 0.3810          | -0.0392 |  |
| [during COVID-19]        | Other                      | 0.6493          | 0.0203  |  |
|                          | Very satisfied             | 0.2084          | -0.0563 |  |
| Satisfaction with the    | Satisfied                  | 0.1412          | 0.0659  |  |
| Working Environment      | Neutral                    | 0.8840          | -0.0065 |  |
|                          | Dissatisfied               | 0.6217          | -0.0221 |  |
|                          | Very dissatisfied          | 0.8367          | 0.0092  |  |
|                          | Never                      | 0.8154          | 0.0104  |  |
| How Often do you         | Rarely                     | 0.9352          | 0.0036  |  |
| use Leisure Facilities   | Sometimes                  | 0.9359          | 0.0036  |  |
|                          | Usually                    | 0.9484          | 0.0029  |  |
|                          | Always or Almost Always    | 0.4686          | -0.0324 |  |
|                          | Company does not provide   | 0.5489          | -0.0268 |  |
|                          | Never                      | 0.3730          | -0.0399 |  |
| How Often do you         | Rarely                     | 0.0504          | 0.0875  |  |
| use Resting Facilities   | Sometimes                  | 0.6989          | -0.0173 |  |
|                          | Usually                    | 0.1637          | -0.0623 |  |
|                          | Always or Almost Always    | 0.5718          | -0.0253 |  |
|                          | Company does not provide   | 0.5323          | 0.0279  |  |
| How Often do you         | Never                      | 0.4500          | -0.0338 |  |
| go to Social Activities  | Rarely                     | 0.0282          | 0.0981  |  |
| explicitly organized by  | Sometimes                  | 0.2426          | 0.0523  |  |
| the company              | Usually                    | 0.5734          | -0.0252 |  |
|                          | Always or Almost Always    | 0.1176          | -0.0700 |  |
|                          | Company does not provide   | 0.2991          | -0.0465 |  |
|                          | Strongly disagree          | 0.4239          | -0.0358 |  |
| I have a healthy         | Disagree                   | 0.1613          | 0.0627  |  |
| relationship with        | Neutral                    | 0.0485          | -0.0882 |  |
| my colleagues            | Agree                      | 0.3124          | 0.0452  |  |
|                          | Strongly agree             | 0.0227          | -0.1018 |  |
|                          | Strongly disagree          | 0.1845          | -0.0594 |  |
| I am often               | Disagree                   | 0.0908          | -0.0756 |  |
| dissatisfied with my job | Neutral                    | 0.1690          | -0.0616 |  |
|                          | Agree                      | 0.5939          | 0.0239  |  |
|                          | Strongly agree             | 0.0324          | 0.0956  |  |

TABLE 5 Work Environment Correlation Results

<span id="page-7-0"></span>

| Working Environment                | Correlation with History   | Spearman's Test |         |
|------------------------------------|----------------------------|-----------------|---------|
| Characteristics                    | of Mental Health Disorders | p-value         | rho     |
| Work Environment [before COVID-19] | Home Office                | 0.0049          | 0.1253  |
| Social Activities                  | Rarely                     | 0.0282          | 0.0981  |
|                                    | Neutral                    | 0.0485          | -0.0882 |
| Relationship with Colleagues       | Strongly agree             | 0.0227          | -0.1018 |
| Dissatisfaction with the Job       | Strongly agree             | 0.0324          | 0.0956  |

and progress of mental health disorders [\[63\]](#page-11-14). One of the main conditions affecting workers' mental health is working hours. Some empirical research suggests a close relationship between working hours and workers' mental health [\[64\]](#page-11-15)– [\[68\]](#page-11-16). Additionally to the number of working hours, other work schedule characteristics, such as the frequency of night work and short daily rest periods (quick return), can affect workers' health as work-related stressors [\[63\]](#page-11-14). In our survey, we investigated which six work schedule characteristics (working hours, work on weekends, checking messages outside working hours, unrealistic deadlines, the impact of COVID-19 pandemic, and tasks performed) can affect software professionals' mental health.

**Working hours.** We asked the survey participants, the number of hours they are expected to work in a typical week and the actual number of worked hours. Regarding all participants, the median for both expected and actual worked hours is 40 hours. However, their means are different (38.37 hours for expected and 40.97 hours for actual). When we analyzed only the participants with history of mental health, we found that the median for both is also 40 hours and their means are different (38.66 hours for expected and 40.83 hours for actual). Table [6](#page-8-0) shows the statistics results after applying the Wilcoxon test to compare the difference between expected and actual worked hours.

TABLE 6 Expected x Actual Working Hours Results.

<span id="page-8-0"></span>

| Population               | Wilcoxon (p-value) | Cohen's d                    | In favor of |
|--------------------------|--------------------|------------------------------|-------------|
| All                      | 2.318e-08          | -0.27 [-0.39, -0.14] (small) | Actual      |
| History of mental health | 0.009              | -0.21 [-0.44, 0.01] (small)  | Actual      |

#### **Observation 12**

Software professionals work more hours than expected and it can be a trigger to deteriorate their mental health.

**Weekends.** We found that 166 out of 500 survey respondents never worked during the weekend. In addition, a substantial number of respondents worked rarely or sometimes (174 rarely respondents and 108 sometimes respondents). The average Likert score for this statement is 2.12 (*i.e.*, between "Rarely" and "Sometimes"). Considering only the participants with history of mental health, we did not find any significant correlation with each one of the weekend's possible answers after applying Spearman's test.

**Messages.** In a typical workday, software professionals use different communication tools, such as emails, meeting notifications, real-time messaging and chat, and remote video calls. We asked the survey participants how often they check messages outside normal working hours. Among the 500 participants, 21.85% always check messages outside normal working hours, whereas 20.8% usually. 70, 110, and 107 participants never, rarely, and sometimes check messages outside normal working hour. The average Likert scale for this statement is 3.14 (*i.e.*, between "Sometimes" and "Usually"). Analyzing only the participants with history of mental health, we did not find any significant correlation for each one of the message's possible answers after applying Spearman's test.

**Unrealistic deadlines.** The inability to meet the established deadline for a software development project completion can be problematic in many different ways. Besides the quality, economic, and business aspects, it can result in burnout since teams work overtime to try and meet the deadline. We surveyed the participants about how often they are required to meet unrealistic deadlines. 133, 172, and 121 participants never, rarely, and sometimes are required to meet unrealistic deadlines. The average Likert score for this statement is 2.34 (*i.e.*, between "Rarely" and "Sometimes"). Considering only the participants with history of mental health, we found an inverse correlation with participants that never are required to meet unrealistic deadlines after applying the Spearman's test (*p*-value = 0.0434, *rho* = -0.09).

# **Observation 13**

As more participants state that they never are required to meet unrealistic deadlines, their probability of having mental health disorders decrease.

**COVID-19 pandemic.** Before the COVID-19 pandemic, 65.8% of participants never worked from home. 78, 33, and 8 participants worked once a week, 2-3 times, and 4- 5 times a week, respectively. The average Likert score for this statement is 1.75 (*i.e.*, between "Never" and "Rarely"). Considering only the participants with history of mental health, we found, applying Spearman's test, that participants that always use to work from home have a positive correlation with mental health disorders (*p*-value = 0.044, *rho* = 0.0898). Moreover, we found a negative correlation with participants that never use to work from home and mental health disorders (*p*-value = 0.0334, *rho* = -0.0951).

### **Observation 14**

Working from home before COVID-19 was a trigger to mental health disorders. Moreover, participants that never had to work from home before COVID-19 are less prone to mental health disorders.

During the COVID-19 pandemic, as expected, because of restrictions, 87.2% of participants worked from home. Analyzing only the participants with history of mental health, we did not find any significant correlation between each one of the possible answers and participants with history of mental health disorders.

**Tasks.** We also asked the participants how often their assigned tasks change abruptly without prior notice. 76, 157, and 156 participants answered never, a few times a year, and a few times a month, respectively. The average Likert score for this statement is 2.59 (*i.e.*, between "A few times a year" and "A few times a month"). Analyzing the participants with history of mental health, we found an inverse correlation for participants who never had their tasks changed abruptly without prior notice (*p*-value = 0.0043, *rho* = -0.1272).

#### **Observation 15**

Participants that never have their tasks changed abruptly without prior notice are less prone to have mental health disorders.

Additionally, we asked the participants if they did not have enough time to perform their tasks with the quality they expected. 55, 137, and 125 participants strongly disagree, are neutral, and disagree, respectively, with this statement. The average Likert score for this statement is 2.96 (*i.e.*, between "Disagree" and "Neutral"). Analyzing the participants with history of mental health, we found an inverse correlation for participants that strongly disagree that they do not have time to do their tasks with the quality they expect (*p*-value = 0.0126, *rho* = -0.1113).

# **Observation 16**

Participants which agree that they have time to do their tasks with the quality they expect are less prone to have mental health disorders.

#### **6 DISCUSSION**

In this section, we discuss each research question in the context of the findings and survey results.

**Mental Health Disorders (RQ1) and Leisure and Entertainment activities (RQ2)**. Mental health disorders are a reality affecting software professionals. We found that 30.2% of the survey participants were diagnosed with mental health disorders in the past or currently. Moreover, 19.4% of participants without any record of mental health disorders were diagnosed with depression. Some participants are taking drugs without medical prescriptions and searching the web and other sources to find information about mental health. We believe that educators can use our findings and disseminate this problem and its consequences for helping practitioners since mental health is often seen as taboo in society.

Currently, some companies are offering psychological services for employees, mainly after the COVID-19 pandemic, which affected them considerably (mental health aspects and leisure and entertainment activities). This practice must be more disseminated in the software industry, and these programs should be more proactive in identifying early symptoms of mental health disorders.

Researchers must also be involved better to understand the efficiency and limitations of these programs. Moreover, longitudinal case studies can be designed to investigate the impact of mental health disorders in software development (quality, productivity, and well-being). While the literature discusses some aspects related to a good day for software professionals [\[19\]](#page-10-15) and what makes them happy [\[20\]](#page-10-16), [\[21\]](#page-10-17), little is known regarding mental health aspects.

Finally, software professionals must engage more in leisure and entertainment activities, mainly those with a history of mental health disorders who did less physical exercise, had fewer hobbies, and spent less time with their family since these aspects can impact mental health and well-being. Researchers in future studies could also explore these aspects to investigate, for example, the software professionals' participation in these activities and the consequences for mental health (for example, monitoring the depression level of software professionals based on PHQ-9 classification during some months).

**Work nature (RQ3)**. We did not find any correlation between organization and team size with mental health disorders. However, analyzing participants with history of mental health disorders, we found that the work type of freelancer and the role of test engineer are associated with mental health disorders. An initial hypothesis can be related to uncertainty in a contract as a freelancer, which can bring more concerns. Nevertheless, new studies must be conducted to understand this aspect and why the test engineer role is more related to mental health disorders. So far, companies and their psychological programs can better keep track of these professionals.

**Work environment (RQ4)**. 68.8% of participants are satisfied with the work environment, and most of the respondents (87%) have a healthy relationship with their colleagues. Nevertheless, some aspects must be better investigated. 38% of participants are dissatisfied with their job. Researchers and companies must work together to understand the reasons behind this aspect and the consequences for software development projects and mental health disorders. Additionally, companies and researchers must work together to investigate why software professionals do not use leisure/resting facilities and do not participate in social activities organized by the company.

**Work schedule (RQ5)**. We identified that software professionals have worked more hours than expected, and this aspect can be a trigger to deteriorate their mental health. In addition, we found that survey participants that never are required to meet unrealistic deadlines, their tasks do not change abruptly without prior notice, and participants who agree that they have time to perform their tasks with the quality they expect are less prone to have mental health disorders.

These aspects should be better addressed by organizations, mainly project managers responsible for project planning. We also consider that researchers should collaborate more with organizations and software professionals (managers and software engineers) to understand the current problems related to project planning (estimates, tasks size, and duration) and productivity and define new solutions to improve estimating and productivity in real settings.

# **7 LIMITATIONS AND THREATS TO VALIDITY**

**Internal Validity:** It is possible that the survey participants misunderstood some of the survey questions. To mitigate this threat, we employed pilot studies to test and collect feedback on our survey. We also conducted a pilot study with survey design experts. The pilot studies were also important to avoid respondent fatigue bias by making sure that the survey could be answered within 20 minutes. We updated the survey based on the findings of these pilot studies.

**External validity:** Our findings may be limited to the survey participants. However, we believe that the large number of participants from various backgrounds more than adequately addresses this concern.

**Construct validity**. Threats to construct validity are concerned with the extent to which the setting of the experiment reflects the construct under study, which include the potential problem of evaluation apprehension. It was mitigated by the anonymity of the participants, as well as the guaranty that all information gathered during the survey would be used only by the research team.

#### **8 CONCLUSION**

In this paper, we presented the results of the snapshot of the mental health of software professionals. To do it, we surveyed 500 software professionals from open source and private projects.

Based on our findings, we derived 16 observations that can be used by practitioners, organizations, and researchers. Practitioners can use our findings to maintain a healthy work-life balance in their careers, even with the specific aspects of software development. Organizations can learn from our survey respondents and take steps to remain productive while creating good programs to ensure the mental health of their employees. The research community can explore the social and human aspects to understand the impact of mental health in software development.

As future work, we intend to conduct a longitudinal case study with software professionals from a private company to gain more insights into the impact of mental health on software quality and productivity.

#### **REFERENCES**

- <span id="page-10-0"></span>[1] T. Spiner, "2021 trends report," *Monitor on Psychology*, vol. 52, p. 40, 2021.
- <span id="page-10-1"></span>[2] Lyra Health, "American worker in crisis: Understanding employee mental health in unprecedented times," [https://www.lyrahealth.com/wp-content/uploads/2020/07/](https://www.lyrahealth.com/wp-content/uploads/2020/07/LYRA-NA-Employee-Mental-Health-Report.pdf) [LYRA-NA-Employee-Mental-Health-Report.pdf,](https://www.lyrahealth.com/wp-content/uploads/2020/07/LYRA-NA-Employee-Mental-Health-Report.pdf) 2020.
- <span id="page-10-2"></span>[3] M. Wilkes, H. Carey, and R. Florisson, "The looking glass: Mental health in the uk film, tv and cinema industry," [https://filmtvcharity.org.uk/wp-content/uploads/2020/02/](https://filmtvcharity.org.uk/wp-content/uploads/2020/02/The-Looking-Glass-Final-Report-Final.pdf) [The-Looking-Glass-Final-Report-Final.pdf,](https://filmtvcharity.org.uk/wp-content/uploads/2020/02/The-Looking-Glass-Final-Report-Final.pdf) 2020.
- <span id="page-10-3"></span>[4] A. E. Muller, E. V. Hafstad, J. P. W. Himmels, G. Smedslund, S. Flottorp, S. Øien Stensland, S. Stroobants, S. Van de Velde, and G. E. Vist, "The mental health impact of the covid-19 pandemic on healthcare workers, and interventions to help them: A rapid systematic review," *Psychiatry Research*, vol. 293, p. 113441, 2020.
- <span id="page-10-4"></span>[5] M. Andreessen, "Why software is eating the world," *The Wall Street Journal*, 2011.
- <span id="page-10-5"></span>[6] R. D. Nayak, "Anxiety and mental health of software professionals and mechanical professionals," *International Journal of Humanities and Social Science Invention*, vol. 3, no. 2, pp. 52–56, 2014.
- <span id="page-10-6"></span>[7] Stack Overflow, "Stack overflow developer survey - 2022," [https:](https://survey.stackoverflow.co/2022/) [//survey.stackoverflow.co/2022/,](https://survey.stackoverflow.co/2022/) 2022.
- <span id="page-10-7"></span>[8] P. L. Li, A. J. Ko, and J. Zhu, "What makes a great software engineer?" in *Proceedings of the 37th International Conference on Software Engineering, ICSE 2015*, 2015, pp. 700–710.
- <span id="page-10-8"></span>[9] P. L. Li, A. J. Ko, and A. Begel, "What distinguishes great software engineers?" *Empir. Softw. Eng.*, vol. 25, no. 1, pp. 322–352, 2020.
- <span id="page-10-9"></span>[10] T. D. LaToza, G. Venolia, and R. DeLine, "Maintaining mental models: a study of developer work habits," in *Proceedings of the 28th international Conference on Software Engineering, ICSE 2006*, 2006, pp. 492–501.
- <span id="page-10-10"></span>[11] M. Claes, M. V. Mantyl ¨ a, M. Kuutila, and B. Adams, "Do pro- ¨ grammers work at night or during the weekend?" in *Proceedings of the 40th International Conference on Software Engineering, ICSE 2018*, 2018, pp. 705–715.
- [12] E. R. Murphy-Hill, E. K. Smith, C. Sadowski, C. Jaspan, C. Winter, M. Jorde, A. Knight, A. Trenk, and S. Gross, "Do developers discover new tools on the toilet?" in *Proceedings of the 41st International Conference on Software Engineering, ICSE 2019*, 2019, pp. 465–475.
- [13] L. E. Barton, G. Candan, T. Fritz, T. Zimmermann, and G. C. Murphy, "The sound of software development: Music listening among software engineers," *IEEE Softw.*, vol. 37, no. 2, pp. 78–85, 2020.
- [14] A. N. Meyer, G. C. Murphy, T. Zimmermann, and T. Fritz, "Enabling good work habits in software developers through reflective goal-setting," *IEEE Transactions on Software Engineering*, vol. 47, no. 9, pp. 1872–1885, 2021.
- <span id="page-10-11"></span>[15] M. Endres, K. Boehnke, and W. Weimer, "Hashing it out: A survey of programmers cannabis usage, perception, and motivation," in *Proceedings of the 44th International Conference on Software Engineering, ICSE 2022*, 2022, pp. 1107–1119.
- <span id="page-10-12"></span>[16] A. N. Meyer, L. E. Barton, G. C. Murphy, T. Zimmermann, and T. Fritz, "The work life of developers: Activities, switches and perceived productivity," *IEEE Transactions on Software Engineering*, vol. 43, no. 12, pp. 1178–1193, 2017.
- <span id="page-10-13"></span>[17] B. Johnson, T. Zimmermann, and C. Bird, "The effect of work environments on productivity and satisfaction of software engineers," *IEEE Transactions on Software Engineering*, vol. 47, no. 4, pp. 736– 757, 2021.
- <span id="page-10-14"></span>[18] D. Fucci, G. Scanniello, S. Romano, and N. Juristo, "Need for sleep: the impact of a night of sleep deprivation on novice developers' performance," *IEEE Transactions on Software Engineering*, vol. 46, no. 1, pp. 1–19, 2018.
- <span id="page-10-15"></span>[19] A. N. Meyer, E. T. Barr, C. Bird, and T. Zimmermann, "Today was a good day: The daily life of software developers," *IEEE Transactions on Software Engineering*, vol. 47, no. 5, pp. 863–880, 2021.
- <span id="page-10-16"></span>[20] D. Graziotin, F. Fagerholm, X. Wang, and P. Abrahamsson, "What happens when software developers are (un)happy," *Journal of Systems and Software (JSS)*, vol. 140, pp. 32–47, 2018.
- <span id="page-10-17"></span>[21] M.-A. Storey, T. Zimmermann, C. Bird, J. Czerwonka, B. Murphy, and E. Kalliamvakou, "Towards a theory of software developer job satisfaction and perceived productivity," *IEEE Transactions on Software Engineering*, vol. 47, no. 10, pp. 2125–2142, 2021.
- <span id="page-10-18"></span>[22] Y. Fujigaki, "A study of mental workload of software engineers," *Work with display units*, vol. 89, pp. 395–402, 1990.

- <span id="page-10-19"></span>[23] P. Ralph, S. Baltes, G. Adisaputri, R. Torkar, V. Kovalenko, M. Kalinowski, N. Novielli, S. Yoo, X. Devroey, X. Tan, M. Zhou, B. Turhan, R. Hoda, H. Hata, G. Robles, A. M. Fard, and R. Alkadhi, "Pandemic programming," *Empir. Softw. Eng.*, vol. 25, no. 6, pp. 4927–4961, 2020.
- [24] C. Miller, P. Rodeghero, M. D. Storey, D. Ford, and T. Zimmermann, ""how was your weekend?" software development teams working from home during COVID-19," in *Proceedings of the 43rd International Conference on Software Engineering, ICSE 2021*, 2021, pp. 624–636.
- [25] P. Silveira, U. Mannan, E. Almeida, N. Nagappan, D. Lo, P. S. Kochhar, C. Gao, and I. Ahmed, "A deep dive into the impact of covid-19 on software development," *IEEE Transactions on Software Engineering*, no. 01, pp. 1–1, jun 2022.
- <span id="page-10-20"></span>[26] D. Ford, M. D. Storey, T. Zimmermann, C. Bird, S. Jaffe, C. S. Maddila, J. L. Butler, B. Houck, and N. Nagappan, "A tale of two cities: Software developers working from home during the COVID-19 pandemic," *ACM Transactions on Software Engineering Methodology (TOSEM)*, vol. 31, no. 2, pp. 27:1–27:37, 2022.
- <span id="page-10-21"></span>[27] T. M. Evans, L. Bira, J. B. Gastelum, L. T. Weiss, and N. L. Vanderford, "Evidence for a mental health crisis in graduate education," *Nature Biotechnology*, vol. 36, pp. 282–284, 2018.
- <span id="page-10-22"></span>[28] C. Wooldton, "Why mental health matters," *Nature*, vol. 557, pp. 129–131, 2018.
- <span id="page-10-23"></span>[29] American Psychiatric Association, *Diagnostic and statistical manual of mental disorders*, 5th ed. Addison-Wesley, 2013.
- <span id="page-10-24"></span>[30] W. H. Crown, S. Finkelstein, E. R. Berndt, D. Ling, A. W. Poret, A. J. Rush, and J. M. Russell, "The impact of treatment-resistant depression on health care utilization and costs," *The Journal of clinical psychiatry*, vol. 63, no. 11, pp. 963–971, 2002.
- <span id="page-10-25"></span>[31] R. C. Kessler, P. Berglund, O. Demler, R. Jin, D. Koretz, K. R. Merikangas, J. Rush, E. E. Walters, and P. S. Wang, "The epidemiology of major depressive disorder: results from the national comorbidity survey replication," *JAMA*, vol. 289, no. 23, pp. 3095– 3105, 2003.
- <span id="page-10-26"></span>[32] R. E. Mayer, "The psychology of how novices learn computer programming," *ACM Computing Surveys (CSUR)*, vol. 13, no. 1, pp. 121–141, 1981.
- <span id="page-10-27"></span>[33] C. Franc¸a, F. Q. Da Silva, and H. Sharp, "Motivation and satisfaction of software engineers," *IEEE Transactions on Software Engineering*, vol. 46, no. 2, pp. 118–140, 2018.
- <span id="page-10-28"></span>[34] T. DeMarco and T. Lister, *Peopleware: productive projects and teams*. Addison-Wesley, 2013.
- <span id="page-10-29"></span>[35] K. Rajeswari and R. Anantharaman, "Development of an instrument to measure stress among software professionals: Factor analytic study," in *Proceedings of the 2003 SIGMIS conference on Computer personnel research: Freedom in Philadelphia–leveraging differences and diversity in the IT workforce*, 2003, pp. 34–43.
- <span id="page-10-30"></span>[36] B. Cohen, "Psychosocial environments created by computer use for managers & systems analysts," *Human-computer interaction. Amsterdam: Elsevier*, pp. 379–84, 1984.
- <span id="page-10-31"></span>[37] T. Haratani, Y. Fujigaki, and T. Asakura, "Job stressors and depressive symptoms in japanese computer software engineers and managers," vol. 20, 1995, pp. 699–704.
- <span id="page-10-32"></span>[38] Y. Fujigaki, "Time series investigation of job-events and depression in computer software engineers," *Industrial Health*, vol. 34, pp. 71– 79, 1996.
- <span id="page-10-33"></span>[39] L. E. Rocha and M. Debert-Ribeiro, "Working conditions, visual fatigue, and mental health among systems analysts in sao paulo, brazil," *Occupational and environmental medicine*, vol. 61, no. 1, pp. 24–32, 2004.
- <span id="page-10-34"></span>[40] K. F. Punch, *Survey research: The basics*. Sage, 2003.
- <span id="page-10-35"></span>[41] T. S. Brugha, P. E. Bebbington, R. Jenkins, H. Meltzer, N. A. Taub, M. Janas, and J. Vernon, "Cross validation of a general population survey diagnostic interview: a comparison of cis-r with scan icd-10 diagnostic categories," *Psychological medicine*, vol. 29, no. 5, pp. 1029–1042, 1999.
- <span id="page-10-36"></span>[42] K. Kroenke, R. L. Spitzer, and J. B. Williams, "The phq-9: validity of a brief depression severity measure," *Journal of general internal medicine*, vol. 16, pp. 606–13, 2001.
- <span id="page-10-37"></span>[43] S. S. Shapiro and M. B. Wilk, "An analysis of variance test for normality (complete samples)," *Biometrika*, vol. 52, no. 3-4, pp. 591–611, dec 1965.
- <span id="page-10-38"></span>[44] R. Woolson, "Wilcoxon signed-rank test," *Wiley encyclopedia of clinical trials*, pp. 1–3, 2007.
- <span id="page-10-39"></span>[45] B. Kitchenham, L. Madeyski, D. Budgen, J. Keung, P. Brereton, S. Charters, S. Gibbs, and A. Pohthong, "Robust statistical

- methods for empirical software engineering," *Empirical Software Engineering*, vol. 22, pp. 579–630, 04 2017.
- <span id="page-11-0"></span>[46] C. spearman, "The proof and measurement of association between two things." 1961.
- <span id="page-11-1"></span>[47] W. Goodman, A. Geiger, and J. Wolf, "Differential links between leisure activities and depressive symptoms in unemployed individuals," *Journal of Clinical Psychology*, vol. 72, pp. 70–78, 2016.
- [48] ——, "Leisure activities are linked to mental health benefits by providing time structure: comparing employed, unemployed and homemakers," *Journal of Epidemiology and Community Health*, vol. 71, pp. 4–11, 2017.
- <span id="page-11-2"></span>[49] G. N. Tonietto, S. A. Malkoc, R. W. Reczek, and M. I. Norton, "Viewing leisure as wasteful undermines enjoyment," *Journal of Experimental Social Psychology*, vol. 97, p. 104198, 2021.
- <span id="page-11-3"></span>[50] Perkbox, *The 2O18 UK Workplace Stress Survey*. Perkbox, 2018.
- <span id="page-11-4"></span>[51] P. C. Pendharkar and J. A. Rodger, "An empirical study of the impact of team size on software development effort," *Information Technology and Management Journal*, vol. 8, no. 4, p. 253–262, 2007.
- <span id="page-11-5"></span>[52] ——, "The relationship between software development team size and software development cost," *Communications of the ACM*, vol. 52, no. 1, p. 141–144, 2009.
- <span id="page-11-6"></span>[53] D. Rodr´ıguez, M. A. Sicilia, E. Garc´ıa, and R. Harrison, "Empirical findings on team size and productivity in software development," *Journal of Systems and Software (JSS)*, vol. 85, no. 3, p. 562–570, 2012.
- <span id="page-11-7"></span>[54] K. S. Rubin, *Essential Scrum: A Practical Guide to the Most Popular Agile Process*, 1st ed. Addison-Wesley Professional, 2012.
- <span id="page-11-8"></span>[55] E. K. Kelloway and J. Barling, "Job characteristics, role stress and mental health," *Journal of Occupational Psychology*, vol. 64, no. 4, pp. 291–304, 1991.
- <span id="page-11-9"></span>[56] D. Ortqvist and J. Wincent, "Prominent consequences of role ¨ stress: A meta-analytic review," *International Journal of Stress Management*, vol. 13, no. 4, p. 399–422, 2006.
- <span id="page-11-10"></span>[57] D. N. Behrman and J. William D. Perreault, "A role stress model of the performance and satisfaction of industrial salespersons," *Journal of Marketing*, vol. 48, no. 4, pp. 9–21, 1984.
- [58] V. A. Lambert and C. E. Lambert, "Literature review of role stress/strain on nurses: An international perspective," *Nursing & Health Sciences*, vol. 3, no. 3, pp. 161–172, 2001.
- [59] E. M. Chang, K. M. Hancock, A. Johnson, J. Daly, and D. Jackson, "Role stress in nurses: Review of related factors and strategies for moving forward," *Nursing & Health Sciences*, vol. 7, no. 1, pp. 57– 65, 2005.
- <span id="page-11-11"></span>[60] G. Wu, Z. Hu, and J. Zheng, "Role stress, job burnout, and job performance in construction project managers: The moderating role of career calling," *International Journal of Environmental Research and Public Health*, vol. 16, no. 13, 2019.
- <span id="page-11-12"></span>[61] S. B. Harvey, M. Modini, S. Joyce, J. S. Milligan-Saville, L. Tan, A. Mykletun, R. A. Bryant, H. Christensen, and P. B. Mitchell, "Can work make you mentally ill? a systematic meta-review of work-related risk factors for common mental health problems," *Occupational and Environmental Medicine Journal*, vol. 74, no. 4, pp. 301–310, 2017.
- <span id="page-11-13"></span>[62] M. Belloni, L. Carrino, and E. Meschi, "The impact of working conditions on mental health: Novel evidence from the uk," *Labour Economics Journal*, vol. 76, 2022.
- <span id="page-11-14"></span>[63] M. Virtanen, J. E. Ferrie, A. Singh-Manoux, M. J. Shipley, S. A. Stansfeld, M. G. Marmot, K. Ahola, J. Vahtera, and M. Kivimaki, ¨ "Long working hours and symptoms of anxiety and depression: a 5-year follow-up of the whitehall ii study," *Psychological Medicine*, vol. 41, no. 12, p. 2485–2494, 2011.
- <span id="page-11-15"></span>[64] T. Amagasa and T. Nakayama, "Relationship between long working hours and depression: A 3-year longitudinal study of clerical workers," *Journal of Occupational and Environmental Medicine*, vol. 55, no. 8, pp. 863–872, 2013.
- [65] G. Weston, A. Zilanawala, E. Webb, L. A. Carvalho, and A. Mc-Munn, "Long work hours, weekend working and depressive symptoms in men and women: findings from a uk populationbased study," *Journal of Epidemiology & Community Health*, vol. 73, no. 5, pp. 465–474, 2019.
- [66] P. Afonso, M. Fonseca, and J. F. Pires, "Impact of working hours on sleep and mental health," *Occupational Medicine*, vol. 67, no. 5, pp. 377–382, 06 2017.
- [67] K. Wong, A. H. S. Chan, and S. C. Ngan, "The effect of long working hours and overtime on occupational health: A metaanalysis of evidence from 1998 to 2018," *International Journal of Environmental Research and Public Health*, vol. 16, no. 12, 2019.

<span id="page-11-16"></span>[68] K. Sato, S. Kuroda, and H. Owan, "Mental health effects of long work hours, night and weekend work, and short rest periods," *Social Science Medicine Journal*, vol. 246, p. 112774, 2020.