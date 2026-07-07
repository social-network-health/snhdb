# A Model for Understanding and Reducing Developer Burnout

Bianca Trinkenreich<sup>∗</sup> , Klaas-Jan Stol† , Igor Steinmacher‡ , Marco A. Gerosa‡ , Anita Sarma§ , Marcelo Lara<sup>∗</sup> , Michael Feathers<sup>∗</sup> , Nicholas Ross<sup>∗</sup> , Kevin Bishop<sup>∗</sup>

<sup>∗</sup>Globant, United States, {first.lastname}@globant.com †Lero and University College Cork, Ireland, k.stol@ucc.ie ‡Northern Arizona Uniersity, United States, {igor.steinmacher, marco.gerosa}@nau.edu §Oregon State University, United States, anita.sarma@oregonstate.edu

*Abstract*—Job burnout is a type of work-related stress associated with a state of physical or emotional exhaustion that also involves a sense of reduced accomplishment and loss of personal identity. Burnt out can affect one's physical and mental health and has become a leading industry concern and can result in high workforce turnover. Through an empirical study at Globant, a large multi-national company, we created a theoretical model to evaluate the complex interplay among organizational culture, work satisfaction, and team climate, and how they impact developer burnout. We conducted a survey of developers in software delivery teams (n=3,281) to test our model and analyzed the data using structural equation modeling, moderation, and multigroup analysis. Our results show that Organizational Culture, Climate for Learning, Sense of Belonging, and Inclusiveness are positively associated with Work Satisfaction, which in turn is associated with Reduced Burnout. Our model generated through a large-scale survey can guide organizations in how to reduce workforce burnout by creating a climate for learning, inclusiveness in teams, and a generative organizational culture where new ideas are welcome, information is actively sought and bad news can be shared without fear.

*Index Terms*—job burnout, work satisfaction, culture, belonging, inclusiveness

## I. INTRODUCTION

Developers' well-being and work satisfaction have a strong influence on workforce retention [\[1\]](#page-10-0), [\[2\]](#page-10-1). When organizations invest in the health and safety of its workforce, it is linked to organizational commitment among employees [\[3\]](#page-10-2) and results in returns that is 2x the amount invested [\[4\]](#page-10-3), [\[5\]](#page-10-4). On the other hand, employee attrition has significant costs, including disruption of ongoing working in a team as well as costs involved in recruiting and training a new team member. This is particularly important for the software industry where 'jobhopping' is quite normal, with many developers changing jobs every few years [\[6\]](#page-10-5). Developer retention is, therefore, a key to the long-term success of software organizations.

Prior research in other fields suggests that burnout is an important factor in employees' intention to leave their job [\[7\]](#page-10-6). Burnout refers to an individual's experiences of exhaustion on physical, emotional, and cognitive levels [\[8\]](#page-10-7). Freudenberger was among the first to explore this concept, invoking a dictionary definition as *"to fail, wear out, or become exhausted by making excessive demands on energy, strength, or resources"* [\[9\]](#page-10-8). While there has been considerable attention in the software engineering literature for themes such as job satisfaction [\[10\]](#page-10-9), [\[11\]](#page-10-10), [\[12\]](#page-10-11), there is a surprising paucity of research on burnout. Job burnout has become increasingly relevant in today's discussions on retaining talent. The COVID-19 pandemic caused a major shift in working patterns for knowledge workers starting in March 2020. Many developers felt overwhelmed working from home while also needing to take care of family and children. Others missed human contact with colleagues and support structures available in the office. As the pandemic has started to wind down (at the time of writing), scholars have coined the term "Great Resignation" to refer to initial observations that many workers across a variety of domains are voluntarily resigning from their job; one explanation is that the pandemic has triggered people to rethink their goals and ambitions in life [\[13\]](#page-10-12). As in other fields [\[14\]](#page-10-13), burnout is also likely playing a role in IT staff's decisions to leave an organization.

It is important, therefore, to understand what *causes* burnout and factors that can mitigate it. Following prior studies [\[15\]](#page-10-14), [\[16\]](#page-10-15), we look at how organizational culture relates to burnout. In particular, we unpack this relationship by investigating a number of salient themes that have attracted interest in recent years, including employees' sense of belonging and work satisfaction.

Our goal is to identify the organizational and cultural antecedents that can reduce burnout. To achieve our goal, we defined the following research questions:

*RQ1. How are organizational culture and burnout related?*

*RQ2. Does the relationship between organizational culture and burnout vary by gender and leadership position?*

We answer these questions within the context of software delivery teams in Globant, a large company employing 25,000 people, and a global presence in 36 cities in 17 countries across five continents, which provides services in digital transformation and assisting IT organizations in automation. Globant invests in continuous training of its talent pool on technical and social skills and has several initiatives in place to retain talent and avoid attrition. Globant places the wellbeing of its employees at the forefront, investing in research to identify and proactively implement strategies to reduce employee burnout and attrition.

To answer our research questions, we developed a theoretical model of factors associated with burnout grounded in prior literature and tested it using structural equation modeling, moderation, and multi-group analysis. We tested the model with data collected via an online questionnaire (n=3,281) for current members of software delivery teams who work on different projects at Globant. Fig. [1](#page-1-0) summarizes the study design.

Our results show that Organizational Culture, Climate for Learning, Sense of Belonging, and Inclusiveness are positively associated with Work Satisfaction, which in turn is associated with Reduced Burnout. A Climate for Learning improves Work Satisfaction for employees who do not hold leadership positions as compared to leadership. Team inclusiveness is positively associated with work satisfaction and has a bigger impact on women. Women are 2x more satisfied and less burnt out when their team is inclusive. National culture also plays a role between work satisfaction and burnout. Living in a masculine (and more competitive) culture further helps reduce burnout when men have work satisfaction; national culture does not play a role for women. An understanding of how these factors interplay can help organizations create a welcoming environment that improves developers' well-being and reduces workforce attrition.

## II. BACKGROUND AND HYPOTHESIS DEVELOPMENT

We review prior work related to this study and develop a theoretical model that reflects the interests of Globant managers.

*A. The Role of Organizational Culture in Sense of Belonging, Climate for Learning, and Inclusiveness*

An organization's culture affects people's daily work activities. Organizational culture has been shown to influence software delivery performance [\[17\]](#page-10-16), [\[15\]](#page-10-14), staff well-being, and retention [\[16\]](#page-10-15), while also enticing software developers to support the company's business [\[18\]](#page-10-17). Westrum developed a typology of organizational cultures based on human factors in system safety, particularly in the context of accidents in technological domains, such as aviation and healthcare [\[19\]](#page-10-18). The typology defines three types of organizations in terms of information flow and psychological safety. Pathological organizations exhibit low levels of cooperation across groups

and a culture of blame. Bureaucratic cultures emphasize rules and positions and compartmentalize responsibilities by departments. Generative organizations are performanceoriented, with good information flow, high levels of cooperation and trust, and bridging between teams. The generative level can be achieved by creating cross-functional teams to improve cooperation, holding blameless postmortems, sharing risks and responsibilities, breaking down silos, and encouraging bridging, experimentation, and novelty. An organizational culture where members of the team cooperate with each other and share responsibilities [\[19\]](#page-10-18) creates feelings of membership or being part of a team [\[20\]](#page-10-19). This organizational culture presents the organization as an extended family, leading employees to develop a strong sense of belonging to the organization [\[21\]](#page-10-20). Hence, we posit:

Hypothesis 1 (H1). A Generative Organizational Culture has a positive association with a Sense of Belonging.

An organization that exhibits a climate for learning makes resources available for continued education and offers continuous encouragement to teams to learn by providing them space and time to acquire new knowledge and explore ideas [\[17\]](#page-10-16). Organizational culture fosters the process of learning [\[22\]](#page-10-21). When holding blameless retrospectives and having out-ofbox thinking, a generative organizational culture [\[23\]](#page-10-22) creates a positive Climate for Learning [\[24\]](#page-11-0) as instead of punishing, the team is trained to learn from failures. Thus, our second hypothesis is:

Hypothesis 2 (H2). A Generative Organizational Culture exhibits a Climate for Learning.

When welcoming new ideas, a generative culture brings a positive tone to a welcoming space and a spirit of friendliness that leads to feelings of inclusiveness among the members of a team [\[20\]](#page-10-19). When engaging in organizational culture, team members perceive an inclusive climate that leads to increased work satisfaction [\[25\]](#page-11-1). This leads to our third hypothesis:

Hypothesis 3 (H3). A Generative Organizational Culture exhibits Inclusiveness.

![](_page_1_Figure_13.jpeg)

<span id="page-1-0"></span>Fig. 1. Methodological approach

*B. The Role of Sense of Belonging, Climate for Learning and Inclusiveness in Work Satisfaction*

The need to belong is a powerful, fundamental, and pervasive force that has multiple strong effects on emotional patterns and cognitive processes, across all cultures and different types of people [\[26\]](#page-11-2). Maslow [\[27\]](#page-11-3) positioned 'belonging' as a basic human need, and Hagerty et al. [\[28\]](#page-11-4) posited that a Sense of Belonging represents a unique mental health concept. A sense of belonging is key to work satisfaction [\[29\]](#page-11-5), and productivity [\[26\]](#page-11-2), and can help to avoid attrition [\[30\]](#page-11-6). References to the importance of a sense of belonging are found throughout the psychological, health care, and education literature. On the other hand, a lack of a sense of belonging is linked to a variety of ill effects on health, adjustment, and well-being [\[26\]](#page-11-2). Hence, we propose our fourth hypothesis:

Hypothesis 4 (H4). Sense of belonging has a positive association with Work Satisfaction.

Prior research on software delivery teams has shown that learning is associated with Work Satisfaction for software delivery teams, as learning is a valuable investment into the project's future and also into the employee's own career [\[31\]](#page-11-7). Moreover, satisfying an employee's need for growth requires that the employee is satisfied with the opportunities to learn and advance at work [\[21\]](#page-10-20). Thus we propose:

Hypothesis 5 (H5). Climate for Learning has a positive association with Work Satisfaction.

When feeling included by the team, employees believe they are valued for their unique personal characteristics and recognized as important members of the organization [\[25\]](#page-11-1). A perception of being socially included improves an individual's well-being [\[32\]](#page-11-8) and enhances their self-esteem and work satisfaction [\[33\]](#page-11-9). So, our sixth hypothesis is:

Hypothesis 6 (H6). Inclusiveness has a positive association with Work Satisfaction.

#### *C. The Role of Work Satisfaction in Reducing Burnout*

A decline in work satisfaction could signal burnout [\[34\]](#page-11-10). Indeed, previous research showed that Burnout has an inverse relationship with Work Satisfaction [\[35\]](#page-11-11), [\[36\]](#page-11-12). Thus, we propose:

Hypothesis 7 (H7). Work Satisfaction has a reverse association with Burnout.

## <span id="page-2-0"></span>*D. The Moderating Role of National Cultural Values on the association between Work Satisfaction and Burnout*

An individual's response to stress is embedded within cultural beliefs. Cultural values are being accredited with a prominent role in various work-related predictor-outcome relationships, such as satisfaction, burnout [\[37\]](#page-11-13), and turnover [\[38\]](#page-11-14). Globant has geographically distributed teams and needs to mitigate the social-derived challenges inherent in cultural differences. Various classifications attempt to quantify cultural values such as the work by Hofstede [\[39\]](#page-11-15), Schwartz [\[40\]](#page-11-16), and the GLOBE

study [\[41\]](#page-11-17). In this study, we adopt Hofstede's classification, which was previously used to analyze the culture of software engineers [\[42\]](#page-11-18), to investigate burnout [\[37\]](#page-11-13) and belonging to a community [\[43\]](#page-11-19). Hofstede [\[39\]](#page-11-15) defined the Hofstede's 6-D framework with the following six dimensions of culture per country that assume values from zero to one hundred [\[44\]](#page-11-20):

*Power Distance* refers to authority and hierarchy and expresses the degree to which less powerful members of a society accept and expect that power is distributed unequally. High power distance means an acceptance of hierarchical order in which people have a determined place. Low power distance means a desire for an egalitarian distribution of power [\[44\]](#page-11-20), [\[45\]](#page-11-21). In high power distance cultures, social hierarchy is established and executed clearly and without reason [\[46\]](#page-11-22). Hierarchy in an organization is seen as reflecting inherent inequalities, centralization is popular, subordinates expect to be told what to do, and the ideal boss is a benevolent autocrat [\[44\]](#page-11-20), [\[45\]](#page-11-21). In Hofstede's classification [\[44\]](#page-11-20), Mexico and India are examples of hierarchical societies with high Power Distance.

*Individualism* represents the degree to which people in a society are integrated into groups. High individualism indicates people who take care of only themselves and their immediate families and should not rely (too much) on authorities for support. In contrast, low individualism (collectivism) reflects a closer integration into cohesive in-groups in which people protect each other with unquestioning loyalty [\[44\]](#page-11-20), [\[45\]](#page-11-21). Collectivists mostly pursue group goals and improve group level engagement [\[47\]](#page-11-23). In Hofstede's classification [\[44\]](#page-11-20), the United States is an example of a society with high Individualism.

*Masculinity* is defined as a preference for achievement, heroism, assertiveness, and material rewards for success. While high masculinity societies are materialist and competitive, low masculinity culture (femininity) is more cooperative, consensusoriented, caring for the weak, and prevailing the life quality [\[44\]](#page-11-20), [\[45\]](#page-11-21). Japan is an example of high degree of masculinity in Hofstede's classification [\[44\]](#page-11-20).

*Uncertainty Avoidance* expresses the degree to which people keep away from ambiguity. Cultures high in uncertainty avoidance tend to focus on rules, structured activities, employee security, and stability. Low levels of uncertainty avoidance have a more relaxed attitude in which practice is more important than rules [\[44\]](#page-11-20), [\[45\]](#page-11-21). In Hofstede's classification [\[44\]](#page-11-20), Uruguay is an example of a score in this dimension while China is the opposite.

*Long Term Orientation* measures the degree a culture will keep some links with its own past while dealing with the challenges of the present and the future. A high degree in this index indicates more pragmatic people who have perseverance and patience to prepare for the future. On the contrary, a lower value on this index (indicating short-term orientation) indicates that people have a more narrow-minded focus and sensitivity to immediate outcomes of their actions, tending to value steadfastness, and considering a societal change with suspicion [\[44\]](#page-11-20), [\[45\]](#page-11-21). People in such societies have a strong concern with establishing the absolute truth; they are normative in their thinking, exhibit great respect for traditions, a relatively small propensity to save for the future, and a focus on achieving quick results. Argentina, for example, has a high score in this dimension in Hofstede's classification [44].

Indulgence is related to the degree of freedom the societal norms give citizens to fulfill human desires. A high degree indicates a society that relatively allows free gratification of basic and natural human desires related to hedonism. Conversely, low levels of indulgence (restraint) indicate a society that controls gratification of needs and regulates it using strict social norms [44], [45].

Studies from two decades ago showed that Long Term Orientation [48] and Power distance [49] could help foster organizational well-being. Subordinates who are surrounded by a high power distance cultural value evaluate abusive supervision as irrelevant to their well-being [49]. Individualism could reduce well-being [50], as unpleasant life events are not met with sufficient social support. In workplace contexts, managers face increasingly complex and subtle differences among employees that reflect cultural influences from the country's culture. Thus, we argue that country culture moderates the link between Work Satisfaction and Burnout. Conceptually, we model this as a single moderator (see Fig. 2), but we propose that each of Hofstede's six dimensions has such a moderating role. Thus, we propose:

**Hypothesis 8 (H8).** (a) Power distance, (b) individualism, (c) masculinity, (d) uncertainty avoidance, (e) long-term orientation, and (f) indulgence moderate the effect of Work Satisfaction on Burnout.

Fig. 2 presents the theoretical model.

#### III. RESEARCH DESIGN

Management at Globant was keen to understand the relationships that we proposed in Fig. 2 and obtain an answer to RQ1, which develops an understanding of how organizational culture and burnout in software delivery teams are related. To evaluate the model, we conducted a survey among software delivery team members at Global and analyzed the data using Partial Least Squares (PLS) Structural Equation Modeling (SEM) [51]. SEM facilitates the simultaneous analysis of relationships among constructs, each measured by one or more indicator variables. Then, to answer RQ2, we used a Multi-

Group Analysis (MGA) to establish whether these relationships vary by gender and leadership position.

A recent survey of the use of PLS in software engineering (which also provides an introduction to PLS) revealed that PLS-SEM has been used to study a variety of phenomena in software engineering [52]. For example, it has previously been used to study job satisfaction and turnover intentions of software engineering teams [11] and the success factors of a large-scale Agile Software transformation process [52].

In this section, we discuss the measurement model (how each theoretical construct was measured) and the data collection and analysis.

#### A. Measurement model

The theoretical model comprising the hypotheses is based on a number of theoretical concepts; some of the concepts cannot be directly observed (e.g., Climate for Learning, Organizational Culture, and Work Satisfaction)—these concepts are represented as *latent* variables. A latent variable cannot be directly measured or observed, but instead is measured through a set of indicators or manifest variables. For the latent variables in this study, we adapted existing measurement instruments when possible. We define the constructs below and list the complete questionnaire in the replication package [53].

**Organization Culture** was measured as a latent construct represented by six five-point Likert questions. The questions were adapted from the Westrum Culture [19], which has previously been used as an instrument to measure organizational culture in software delivery teams [54], [15].

**Belonging** was measured using a five-point Likert question to assess aspects of membership, as being part of the team.

Climate for Learning was measured as a latent construct represented by two five-point Likert questions. The questions were inspired by DORA Research Program [17] and designed to evaluate if members of the team perceive that the team considers learning as an investment rather than a cost, and essential for continued progress.

**Inclusiveness** was measured through one question to assess if the team has a safe space for diversity in which everyone is welcomed and treated equally and fairly.

**Work Satisfaction** was measured as a latent construct composed of two Employee Net Promoter 10-scale Score (eNPS) questions [55], [56] and one five-point Likert question

![](_page_3_Figure_17.jpeg)

<span id="page-3-0"></span>Fig. 2. Theoretical model

about enjoyment. The eNPS questions were towards the team and towards the company, which relies on asking the respondent the willingness to recommend the team and the company to friends and colleagues.

Burnout was measured as a latent construct composed of two five-point Likert items. While instruments exist to measure burnout, these are very long, which would result in an overly long survey instrument. We took a pragmatic approach and focused on two statements: (1) the extent to which a team has a manageable workload with sustainable levels of stress, and burnout is not perceived as a significant problem or risk; and (2) the extent to which tasks are assigned in a way that allows enough time to achieve commitments, and team members are able to focus on one process at a time. Both were measured as 'reversed' items, i.e., a strong *disagreement* indicated a higher level of burnout.

National Culture: Based on the respondents' country of residence, we used Hofstede's classification of National Culture as moderators (Sec. [II-D\)](#page-2-0). This classification's sixdimensional approach to cultural variation includes power distance, individualism/collectivism, masculinity/femininity, uncertainty avoidance, long-term/short-term orientation, and indulgence [\[39\]](#page-11-15).

#### *B. Data Collection and Analysis*

We administered an online questionnaire using Globant Glow,[1](#page-4-0) which was answered by members of software delivery teams at Globant.

The survey was sent to respondents by email using a corporate address. The leader of each team encouraged team members to fill the questionnaire out during regular meetings. We received 10,566 responses; however, our analysis techniques require complete responses, and we removed 7,285 responses that contained blanks. Our final sample size has 3,281 responses. Table [I](#page-4-1) presents a summary of the respondents' characteristics.

We used SmartPLS version 4 for the analyses; SmartPLS is a proprietary package for analyzing PLS models. The analysis comprised three steps, with tests and procedures in each step. The first step was to evaluate the measurement model (Sec. [IV\)](#page-4-2), which empirically assesses the relationships between the constructs and indicators. The second step was to evaluate the theoretical model that represents the set of hypotheses (Sec. [V-A\)](#page-5-0). The third step was to evaluate observed heterogeneity by multi-group analysis of gender and leadership position (Sec. [V-B\)](#page-6-0).

PLS does not make assumptions about the distribution (such as a Normal distribution) of the data; without knowing the distribution of the data, parametric tests (which are based on a distribution with certain parameters) cannot be used to establish the standard error and thus significance. Instead, PLS packages employ a 'bootstrapping' procedure: it draws a large number (e.g. 5,000) of random 'subsamples' of the same size as the original sample (using replacement). The model is estimated for each subsample, generating a sampling distribution, which is

TABLE I DEMOGRAPHICS OF RESPONDENTS (N=3,281)

<span id="page-4-1"></span>

| Attribute                     | N     | Percentage |  |  |  |  |  |
|-------------------------------|-------|------------|--|--|--|--|--|
| Gender                        |       |            |  |  |  |  |  |
| Men                           | 2,487 | 74.8%      |  |  |  |  |  |
| Women                         | 794   | 25.2%      |  |  |  |  |  |
| Country of Residence          |       |            |  |  |  |  |  |
| Colombia                      | 789   | 24.0%      |  |  |  |  |  |
| Argentina                     | 721   | 22.0%      |  |  |  |  |  |
| India                         | 581   | 17.7%      |  |  |  |  |  |
| Mexico                        | 515   | 15.7%      |  |  |  |  |  |
| Uruguay                       | 211   | 6.4%       |  |  |  |  |  |
| Chile                         | 197   | 6.0%       |  |  |  |  |  |
| Peru                          | 128   | 3.9%       |  |  |  |  |  |
| USA                           | 55    | 1.7%       |  |  |  |  |  |
| Brazil                        | 53    | 1.6%       |  |  |  |  |  |
| Spain                         | 15    | 0.5%       |  |  |  |  |  |
| Belarus                       | 9     | 0.3%       |  |  |  |  |  |
| Others                        | 7     | 0.3%       |  |  |  |  |  |
| Roles                         |       |            |  |  |  |  |  |
| Leadership Positions          |       |            |  |  |  |  |  |
| Project Manager               | 248   | 7.6%       |  |  |  |  |  |
| Tech Manager                  | 34    | 1.0%       |  |  |  |  |  |
| Product Manager               | 12    | 0.4%       |  |  |  |  |  |
| Other leadership roles        | 5     | 0.2%       |  |  |  |  |  |
| Non-Leadership Positions      |       |            |  |  |  |  |  |
|                               |       |            |  |  |  |  |  |
| Developers                    | 1,723 | 52.5%      |  |  |  |  |  |
| Test/Quality Assurance        | 656   | 20.0%      |  |  |  |  |  |
| Business Analyst/Intelligence | 158   | 4.8%       |  |  |  |  |  |
| ERP Tech/Functional           | 98    | 3.0%       |  |  |  |  |  |
| DevOps Engineer               | 71    | 2.2%       |  |  |  |  |  |
| Designer/Artist               | 65    | 2.0%       |  |  |  |  |  |
| Data Architect/Scientist      | 55    | 1.7%       |  |  |  |  |  |
| SysAdmin/Cloud Engineer       | 45    | 1.3%       |  |  |  |  |  |
| Other non-leader roles        | 111   | 3.3%       |  |  |  |  |  |
| Starting year at the company  |       |            |  |  |  |  |  |
| Between 2021 and 2022         | 1,460 | 44.5%      |  |  |  |  |  |
| Between 2019 and 2020         | 1,081 | 32.9%      |  |  |  |  |  |
| Between 2018 and 2017         | 422   | 12.9%      |  |  |  |  |  |
| Between 2016 and 2015         | 181   | 5.5%       |  |  |  |  |  |
| Between 2014 and 2015         | 137   | 4.2%       |  |  |  |  |  |

used to determine a standard error [\[57\]](#page-11-33), which can subsequently be used to make statistical inferences. The mean path coefficient determined by bootstrapping can differ slightly from the path coefficient calculated directly from the sample.

The online appendix provides results of a variety of additional analyses and validity checks [\[53\]](#page-11-29).

# IV. MEASUREMENT VALIDITY AND MODEL FIT

#### <span id="page-4-2"></span>*A. Measurement Validity*

As a first step, we conducted two recommended tests to ensure that a dataset is suitable for factor analysis, i.e., that the variables in a dataset can be reduced to a smaller number of factors [\[58\]](#page-11-34), [\[59\]](#page-11-35). The first test is Bartlett's test of sphericity [\[58\]](#page-11-34) on all constructs. We found a p-value < .01 (p-values less than .05 indicate that factor analysis may be suitable). Second, we calculated the Kaiser-Meyer-Olkin (KMO) measure

<span id="page-4-0"></span><sup>1</sup><https://os.starmeup.com/en.html>

of sampling adequacy. Our result (.92) is well above the recommended threshold of .60 [\[59\]](#page-11-35).

Afterward, we conducted several tests to validate the measurement of our theoretical concepts, including convergent validity, internal consistency reliability, discriminant validity, and collinearity, as discussed next.

*1) Convergent Validity:* First, we assess the convergent validity of the measurement instrument, i.e., we assess whether the questions (indicators) that represent each latent variable are understood by the respondents in the same way as they were intended by the designers of the questions [\[60\]](#page-11-36). This assessment relates to the degree to which a measure correlates positively with alternative measures of the same construct. Our model contains four latent variables (Climate for Learning, Organizational Culture, Work Satisfaction, and Burnout). Changes in the theoretical, latent construct should be 'reflected' in changes in the indicator variables [\[57\]](#page-11-33); for example, if Work Satisfaction increases, a concept we cannot measure or observe *directly*, we expect to see this change reflected in the values of its indicators that we *can* measure or observe directly.

We used two metrics to assess convergent validity: the Average Variance Extracted (AVE) and the loading of an indicator onto its construct (the outer loading). The AVE is the proportion of variance that is shared across indicators. The AVE should be at least 50%, indicating that it explains most part the variation in its indicators [\[57\]](#page-11-33). All AVE values for the three latent constructs in our model are above this threshold of 50% (see appendix).

A latent variable is measured by two or more indicators; each indicator is expected to have a loading of at least 50%, because the square of the loading indicates the variance in the indicator that is explained, which should be at least 50% (and 70%<sup>2</sup> ≈ 50%) [\[57\]](#page-11-33). All loadings of the indicators of all four latent constructs exceeded this as shown in Figure [3,](#page-5-1) which we considered acceptable.

*2) Internal Consistency Reliability:* Second, we verified how well the different indicators are consistent with one another and able to reliably and consistently measure the constructs. A high degree of consistency means that indicators refer to the same construct. There are several tests to measure internal

consistency reliability. We performed both the Cronbach's α and Composite Reliability tests; Cronbach's α frequently shows lower values, whereas the Composite Reliability (CR) is a more liberal test, which sometimes overestimates the values [\[57\]](#page-11-33). A desirable range of values for both Cronbach's α and CR is between .7 and .9 [\[57\]](#page-11-33). Values below .6 suggest a lack of internal consistency reliability, whereas values over .95 suggest that indicators are too similar and thus are not desirable. All Cronbach α and CR values fell between .7 and .9 (see appendix).

- *3) Discriminant Validity:* Third, we verified whether each construct represents characteristics that are not measured by other constructs, i.e., we assessed the discriminant validity of the constructs. A primary means to assess discriminant validity is to investigate the Heterotrait-monotrait (HTMT) ratio of correlations [\[61\]](#page-11-37). The discriminant validity could be considered problematic if the HTMT ratio exceeds .9 [\[61\]](#page-11-37); some scholars recommend a more conservative cut-off of .85 [\[57\]](#page-11-33). The HTMT ratio between the four latent constructs ranged between .65 and .71 (see appendix).
- *4) Assessing Collinearity:* To ensure that the variables are independent, we calculate their collinearity by means of the Variance Inflation Factor (VIF). In our model all VIF values are below 1.7, well below the cut-off of 5 [\[57\]](#page-11-33) (see appendix).

#### *B. Model Fit*

The overall model was measured through a standardized root mean square residual (SRMR) composite factor model, which should be lower than .08 [\[62\]](#page-11-38). Thus, the values obtained for the complete model (.060), the men's model (.061), the women's model (.061), the leaders' model (.070), and the non-leaders model (.60) have a good fit.

### V. RESULTS

To answer RQ1, we evaluated the hypotheses in the structural model (Sec. [V-A\)](#page-5-0) and, to answer RQ2, we performed a Multi-Group Analysis (Sec. [V-B\)](#page-6-0).

<span id="page-5-0"></span>*A. RQ1. How are organizational culture and burnout in software delivery teams related?*

Table [II](#page-6-1) shows the results for our hypotheses, including the mean of the bootstrap distribution (*B*), the standard deviation (*SD*), the 95% confidence interval, and the p-values.

![](_page_5_Figure_15.jpeg)

<span id="page-5-1"></span>Fig. 3. Path coefficients (p < 0.05 indicated by a full line). Latent constructs are represented as circles.

<span id="page-6-1"></span>TABLE II STANDARIZED PATH COEFFICIENTS, STANDARD DEVIATIONS AND CONFIDENCE INTERVALS. COEFFICIENTS WITH \* ARE LOWER THAN .05

|                                                                                                                                                                                                                                                                                  | B     | SD  | 95% CI       |  |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|-----|--------------|--|
| H1 Organizational Culture→Belonging                                                                                                                                                                                                                                              | .48*  | .02 | (.44, .51)   |  |
| H2 Organizational Culture→Climate for<br>Learning                                                                                                                                                                                                                                | .54*  | .02 | (.51, .57)   |  |
| H3 Organizational Culture→Inclusiveness                                                                                                                                                                                                                                          | .45*  | .02 | (.41, .49)   |  |
| H4 Belonging→Work Satisfaction                                                                                                                                                                                                                                                   | .24*  | .02 | (.20, .27)   |  |
| H5 Climate for Learning→Work<br>Satisfaction                                                                                                                                                                                                                                     | .22*  | .02 | (.18, .25)   |  |
| H6 Inclusiveness→Work Satisfaction                                                                                                                                                                                                                                               | .12*  | .02 | (.08, .16)   |  |
| H7 Work Satisfaction→Burnout                                                                                                                                                                                                                                                     | −.29* | .02 | (−.25, −.33) |  |
| Moderators                                                                                                                                                                                                                                                                       |       |     |              |  |
| H8.a Power Distance × Work<br>Satisfaction→Burnout                                                                                                                                                                                                                               | .08   | .05 | (.19, .00)   |  |
| H8.b Individualism × Work<br>Satisfaction→Burnout<br>H8.c Masculinity × Work<br>Satisfaction→Burnout<br>H8.d Uncertainty Avoidance × Work<br>Satisfaction→Burnout<br>H8.e Long Term Orientation × Work<br>Satisfaction→Burnout<br>H8.f Indulgence × Work<br>Satisfaction→Burnout | .05   | .04 | (.13, .03)   |  |
|                                                                                                                                                                                                                                                                                  | −.02  | .05 | (.07, −.12)  |  |
|                                                                                                                                                                                                                                                                                  | −.01  | .05 | (.08, −.01)  |  |
|                                                                                                                                                                                                                                                                                  | −.09  | .08 | (.05, −.27)  |  |
|                                                                                                                                                                                                                                                                                  | −.02  | .05 | (.08, −.13)  |  |

Path coefficients (*B*) are interpreted as follows in this example for H1: having *B*=.48 means that a unit-change of Organizational Culture's standard deviation triggers a direct change in Belonging of .48 × Belonging's standard deviation.

Results revealed that a Generative Organizational Culture has a positive significant association with Sense of Belonging (H1, *B*=.48), Climate for Learning (H2, *B*=.54), and Inclusiveness (H3, *B*=.45). We also found that a Sense of Belonging to the team (H4, *B*=.24), Climate for Learning (H5, *B*=.22), and Inclusiveness (H6, *B*=.12) have a positive and significant association with Work Satisfaction, which includes feelings of joy and enthusiasm to recommend the team and company as a place to work to friends former colleagues. Finally, Work Satisfaction has a reverse (negative) and significant association with Burnout (H7, *B*=−0.29). Hence, hypotheses H1 to H7 were supported with p-values < 0.001.

We also investigated whether the association between Work Satisfaction and Burnout would change when considering respondents' national culture, as defined by Hofstede's six dimensions (see Sec. [II-D\)](#page-2-0) (H8). This association is not significantly affected (neither increased nor reduced) by any of these six cultural dimensions. Power Distance (H8.a) and Individualism (H8.b) have a positive, but insignificant moderation effect in the association between Work Satisfaction and Burnout. Masculinity (H8.c), Uncertainty Avoidance (H8.d), Long Term Orientation (H8.e), and Indulgence (H8.f) have a negative, but insignificant moderation effect on the association between Work Satisfaction and Burnout. Hence, H8.(a-f) are not supported for the complete dataset.

We assessed the relationship between constructs and the predictive capabilities of the model. The *R* 2 ranges from 0 to 1, with higher values indicating a greater explanatory power. *R* 2 values of .75, .50, and .25 are considered substantial, moderate, and weak, respectively [\[57\]](#page-11-33). However, such thresholds are rather arbitrary and generic, and do not consider the specific context or research area; in some fields, an *R* <sup>2</sup> value as low as .10 is considered satisfactory [\[63\]](#page-11-39). The *R* <sup>2</sup> values of the five endogenous variables in our model (Belonging, Climate for Learning, Inclusiveness, Work Satisfaction, and Burnout) are shown in Table [III](#page-8-0) are acceptable ranging between .20 and .39 (column 'All'; further variation in range emerged after the multi-group analysis, discussed later).

We also assessed the predictive relevance of the model, using the Stone-Geisser *Q* <sup>2</sup> measure. For this, we used the PLSPredict algorithm that is available in the SmartPLS v. 4 package [\[64\]](#page-11-40), [\[65\]](#page-11-41). Values larger than 0 indicate the construct has predictive relevance, while negative values (smaller than zero) indicate that the model does not perform better than the simple average of the endogenous variable would do. The values were all positive, indicating the construct has predictive relevance [\[57\]](#page-11-33).

<span id="page-6-0"></span>*B. RQ2: Does the relationship between organizational culture and burnout vary by gender and leadership position?*

RQ2 seeks to establish whether the theorized relationship between organizational culture and burnout (as investigated for RQ1), varies when we consider gender and leadership position. Are some of the hypothesized links stronger for men than for women, or vice versa? Or are these associations different for people in leadership positions vs. people not in leadership positions? To answer this, we used multi-group analyses splitting by gender and leadership position and exploring differences that can be traced back to observable characteristics and may not be evident when examined as a whole. The multigroup analysis involves running the PLS path model multiple times for different groups, once for each group; groups are captured through categorical variables (in this case, binary variables). Hair et al. [\[62\]](#page-11-38) proposed three steps to conduct such an analysis: (1) group creation; (2) invariance test; and (3) result analysis.

- *1) Step 1. Groups Creation:* We grouped our participants to observe heterogeneity according to two variables: gender (male = 0 and female = 1) and leadership (leadership role = 1 and non-leadership role = 0). We used pre-existing demographic data the company maintains for its reporting requirements under government laws to split the participants into different groups.
- *2) Step 2. Evaluation of measurement invariance of composite models (MICOM):* Measurement invariance is a mechanism to assess whether or not the loadings of the items that represent the latent variables differ significantly across different groups. In other words, we want to assess whether the differences can be attributed to the theoretical constructs and not to how we measured those constructs [\[62\]](#page-11-38). Comparing groupspecific model relationships for significant differences using a multi-group analysis requires establishing configural and compositional invariance [\[66\]](#page-11-42), [\[62\]](#page-11-38). Configural invariance does not include a test and is a qualitative assessment of making sure that all of the composites are equally defined for all of the

groups such as equivalent indicators per measurement model, equivalent treatment of the data, and equivalent algorithm settings or optimization criteria. The configural invariance is established in our model. Following that, compositional invariance exists when the composite scores are the same across both groups, and is statistically tested to assess whether the composite scores differ significantly across the groups. For this purpose, the MICOM procedure examines the correlation between the composite scores of both groups and requires that the correlation equals 1. We ran the permutation test in SmartPLS and verified that compositional invariance is established for all latent variables in the PLS path model. We established partial measurement invariance and thus multigroup analysis is suitable [\[67\]](#page-11-43).

*3) Step 3. Groups Comparison and Analysis:* Path coefficients generated from different samples are usually numerically different, but the question is whether the differences are statistically significant. We analyzed the differences between the coefficients' paths for the groups. If they are significant, they can be interpreted as having moderating effects.

Gender: As Table [III](#page-8-0) shows, Generative Organizational Culture has a strong and significant relationship with Sense of Belonging and Climate for Learning for both men and women. However, although Organizational Culture is also associated with Inclusiveness for both men and women, the association is stronger for women (β = .53) than for men (β = .41). Sense of Belonging and Climate for Learning have a significant and similar relationship with Work Satisfaction for both genders. Although both genders are satisfied by Inclusiveness, women (β = .20) are two times more satisfied when the team is Inclusive compared to men (β = .10). Lastly, the link between Work Satisfaction and Burnout is the same for men and women. However, men (but not women) who live in a competitive national culture, where people want to be the best (i.e., high degree of Masculinity), have even less burnout.

Leadership Position: As Table [III](#page-8-0) shows, Climate for Learning has a strong and significant relationship with Work Satisfaction for those who are not in leadership positions. However, Climate for Learning is not associated with Work Satisfaction for leaders. Lastly, leaders (β = .41) are close to two times more satisfied by a Generative Organizational Culture when compared to those who are not in leadership positions (β = .24).

#### VI. DISCUSSION

Human factors are receiving increasingly more attention in software engineering research and industry. Themes such as work satisfaction have been studied extensively and have been linked to employees' intention to stay with (or leave, when it is lacking) an organization. This has direct effects on organizations' capacity to deliver services and software products.

The past several years have seen dramatic changes in the way people work, driven in large part by the Covid-19 pandemic and the resulting lockdowns, forcing people to work from home. There are numerous studies on how this has affected people in negative ways (e.g. [\[68\]](#page-11-44)). One important theme in this context is Burnout, which is the result of continuous exposure to unhealthy levels of stress. However, there is a paucity of research in software engineering on this topic. Globant, a major provider of software services that has operations across five continents, is reliant on a healthy workforce to conduct its business. Globant is interested in developing better insights into the various factors that might play a role in employee burnout. Thus, in this paper, we report on a large-scale survey at Globant with a primary focus has been on Burnout and its antecedents.

In particular, we sought to understand the role of organizational culture in relation to Burnout. Organizational culture has been shown to be an important factor in the performance of employees and teams, including in software delivery teams [\[54\]](#page-11-30). Our theoretical argument in this paper is that all employees within an organization are exposed to the same organizational culture; while they will experience this differently, we believe other factors play a role in why people might experience burnout. In particular, we looked at three factors: people's Sense of Belonging, whether or not an organization advocates a Climate for Learning, and people experiencing Inclusiveness. Further, rather than having a direct link to Burnout, we believe that these factors affect employees' Work Satisfaction, and this is a major predictor for people's experienced Burnout.

We used questions based on an Organizational Culture typology that is focused on how organizations process information and behave when things are not going well, bringing together not only culture, but also management style. We analyzed Organizational Culture as a latent variable that included attributes about sharing bad news with no fear, considering failures as learning opportunities, encouraging cross-functional collaboration, welcoming new ideas, sharing responsibilities, and actively seeking information when needing it.

We also considered the moderating role of national culture, considering the six dimensions identified by Hofstede. Finally, we conducted our analysis for the whole sample and conducted two different multi-group analyses, distinguishing respondents by gender, and whether or not they are in a leadership role.

Before we discuss the implications of our results, we discuss a number of limitations of this study that should be kept in mind while interpreting the findings.

#### *A. Threats to Validity*

*1) Construct Validity:* We adopted and tailored existing measurement instruments when possible, and developed measurement instruments for some constructs based on prior literature. Our analysis of the measurement model confirmed that our constructs were internally consistent, and scored well on convergent and discriminant validity tests. We defined new a construct called Work Satisfaction that included hedonism and satisfaction towards the team and the company. We acknowledge the fact that Burnout is a construct that can be measured by more complex instruments [\[69\]](#page-11-45). However, many existing instruments contain a large number of items (questions), which would be impractical in organizational

<span id="page-8-0"></span>TABLE III MULTI-GROUP ANALYSIS: COEFFICIENTS MARKED WITH ∗ ARE STATISTICALLY SIGNIFICANT; COEFFICIENTS SET IN BOLDFACE INDICATE THAT THE DIFFERENCE BETWEEN GROUPS (I.E. MALE VS. FEMALE, AND NON-LEADERSHIP VS. LEADERSHIP ROLES) IS STATISTICALLY SIGNIFICANT

|                                                          | Multi-Group Analysis |        |             |         |       |
|----------------------------------------------------------|----------------------|--------|-------------|---------|-------|
|                                                          | Gender               |        | Leadership  |         |       |
|                                                          | Male                 | Female | Non-leaders | Leaders | All   |
| Sample size (N)                                          | 2,487                | 79     | 2,982       | 299     | 3,281 |
| 2<br>Belonging (R<br>)                                   | .23                  | .24    | .22         | .25     | .23   |
| 2<br>Climate for Learning (R<br>)                        | .28                  | .32    | .29         | .31     | .29   |
| 2<br>Inclusiveness (R<br>)                               | .17                  | .28    | .20         | .25     | .20   |
| 2<br>Work Satisfaction (R<br>)                           | .38                  | .41    | .39         | .35     | .39   |
| 2<br>Burnout (R<br>)                                     | .31                  | .37    | .34         | .36     | .33   |
| H1 Organizational Culture → Belonging                    | .48*                 | .49*   | .47*        | .50*    | .48*  |
| H2 Organizational Culture → Climate for Learning         | .53*                 | .57*   | .54*        | .56*    | .54*  |
| H3 Organizational Culture → Inclusiveness                | .41*                 | .53*   | .44*        | .46*    | .45*  |
| H4 Belonging → Work Satisfaction                         | .25*                 | .21*   | .24*        | .20*    | .24*  |
| H5 Climate for Learning → Work Satisfaction              | .22*                 | .21*   | .22*        | .08     | .22*  |
| H6 Inclusiveness→Work Satisfaction                       | .10*                 | .20*   | .13*        | .01*    | .12*  |
| H7 Work Satisfaction→Burnout                             | −.29*                | −.29*  | −.29*       | −.20*   | −.29* |
| Moderators                                               |                      |        |             |         |       |
| H8.a Power Distance × Work Satisfaction→ Burnout         | .01                  | .01    | .11         | .07     | .08   |
| H8.b Individualism × Work Satisfaction→ Burnout          | .08                  | −.01   | .16         | .03     | .05   |
| H8.c Masculinity × Work Satisfaction → Burnout           | −.10*                | .13    | −.17        | .01     | −.02  |
| H8.d Uncertainty Avoidance × Work Satisfaction → Burnout | −.07                 | .18    | −.01        | .01     | −.01  |
| H8.e Long Term Orientation× Work Satisfaction→ Burnout   | −.13                 | −.04   | −.10        | −.06    | −.09  |
| H8.f Indulgence × Work Satisfaction → Burnout            | .03                  | −.18   | .15         | −.04    | −.02  |

settings because this would negatively affect the response rate. In this study we have used respondents' country of residence as a proxy for Power Distance as a dimension of culture as defined by Hofstede [\[44\]](#page-11-20). While also used in other studies [\[70\]](#page-11-46), we acknowledge it is an approximation and not a perfect measure. One potential issue is that we do not know how *long* respondents have lived in their current country of residence. Another potential issue is that contributors' original culture that they grew up with may differ from the culture they now live in. This is why we report the metric as being surrounded by a specific culture instead of having a specific culture. Measuring culture in a more precise way is an important avenue for future work in general.

*2) Internal Validity:* We propose a series of hypotheses as associations between different constructs rather than causal relationships, as the present study is a sample study, rather than an experimental study [\[71\]](#page-11-47). Our overall argument is that employees who perceive their organization to have what Westrum [\[19\]](#page-10-18) labeled a Generative Organizational Culture are satisfied and tend to experience levels of burnout; this line of reasoning is easier to theoretically justify than the suggestion that Burnout leads to a negative organizational culture (what Westrum referred to as a Pathological organization) [\[19\]](#page-10-18). Further, it is likely that other factors are at play. The coefficient of determination (*R* 2 ) of the endogenous variables ranged between .2 and .4 which in the software engineering context can be considered reasonable. Thus, these results represent a useful starting point for future studies.

Respondents are current employees and we did not collect data from past employees. As the company does not offer the same questionnaire to people who are leaving, we would not have the same data to compare the perspectives of current and past employees. The relationship between burnout and intentions to leave, and also the actual act of leaving are of interest for future work.

*3) External Validity:* This survey was conducted within Globant. The response rate numbers are aligned with the overall distribution of the company and therefore can be generalized across the company. Globant is a multi-national company with more than 25,000 employees working in different national cultures. The responses were sufficiently consistent to find full or partial empirical support for the hypotheses. Additional studies that replicate our findings in other companies can further bolster our results.

## *B. Implications of results*

Our analysis highlights several key findings and implications. In the following, we discuss the supported hypotheses.

H1. Generative Organizational Culture → Belonging: Our results align with previous research that showed a sense of belonging emerges from a people-centered culture [\[72\]](#page-11-48) and that openness to innovation and shared responsibility helps to develop organizational belonging [\[73\]](#page-11-49). When working in a team that welcomes new ideas, fosters collaboration, and shares responsibilities [\[19\]](#page-10-18), people understand how their work contributes toward a common goal leading to affective commitment to the team. Our results showed there was no significant difference between the groups for H1, which proposed

a positive association between a Generative Organizational Culture and a Sense of Belonging, as shown in Table [III.](#page-8-0)

H2. Generative Organizational Culture → Climate for Learning: In a generative organizational culture, people do not fear failure because they are trained to learn from mistakes [\[19\]](#page-10-18); learning is a key point, considered essential and an investment. An inspiring culture that encourages and enables employees to bring their best efforts and ideas to the team promotes a Climate for Learning [\[72\]](#page-11-48). We found that a generative organizational culture is positively associated with Climate for Learning and that there is no significant difference between different groups (either in terms of gender or whether or not respondents fulfilled a leadership role) for this association.

H3. Generative Organizational Culture → Inclusiveness: Although the association between Organizational Culture and Inclusiveness is not significantly different according to the leadership position, it is stronger for women (*B*=.53) than for men (*B*=.41). This difference opens a path to discuss what brings Inclusiveness for minority and majority groups. A lot has been researched about providing safe place for diversity so that everyone feels equally welcomed. However, results shed light that different factors bring the feeling of being included for minority and majority groups.

Hypotheses 1-3 show the benefits of a generative organizational culture where employees have the psychological safety to talk about failures and present new ideas. Therefore, companies should reflect on their team and leadership culture to promote the ideas of generative organizational culture.

Changing the way people behave and work changes culture. Teams can identify helpful practices to create a generative culture that fosters information flow and trust by examining the aspects of Westrum's model of organizational culture [\[19\]](#page-10-18), focusing on those behaviors seen in the generative culture:

- Cooperation and bridging. Break down silos and create cross-functional teams that include representatives from each functional area of the software delivery process, so everyone shares the responsibility for the software delivery life-cycle. Encourage informal meetings between people who do not understand (or are frustrated by) each other's work. Ask them to understand each other why they do what they do–and invite people to come up with new ideas together.
- Train the messengers and let failure lead to inquiry. People must be able to take risks and feel safe to fail, and also to bring bad news without fear in order to make improvements. Hold blameless postmortems, so teams surface problems as early as possible, and solve them more effectively. Instead of blaming, ask questions about the root-cause of failures, in order to improve technical systems, processes, and the organizational culture.
- Share risks and responsibilities. Quality, availability, reliability, and security should be everyone's job. One practical example can be ensuring that developers share responsibility for maintaining their code in production.
- Encourage novelty. Encouraging employees to explore new ideas can lead to great outcomes. One example

of this practice can be giving people time each week for experimentation, hosting internal hackathons and conferences to share ideas and collaborate. When releasing employees from habitual pathways and repetitive tasks, they can be creative, bringing new ideas for processes and products.

H4. Sense of Belonging → Work Satisfaction: A Sense of Belonging is a human need [\[26\]](#page-11-2), [\[74\]](#page-12-0), [\[75\]](#page-12-1). Although it has several different antecedents for people, employees from different groups showed higher levels of Work Satisfaction when they feel they are part of a team. Our analysis based on groups showed similar path coefficients for the association between Sense of Belonging and Work Satisfaction, as we present in Table [III.](#page-8-0) This indicates that strategies that focus on making employees feel part of the team or the company, pay off, because this positively influences satisfaction, regardless of the group to which the developers belong. Therefore, companies could invest in cohort building, creating opportunities where developers can socialize and develop an emotional connection. Additionally, belonging can be fostered via a team culture where individuals' contributions are appreciated and they can see how their work fits the team's overall goals.

H5. Climate for Learning → Work Satisfaction: The association between Climate for Learning and Work Satisfaction is significantly different between leaders and nonleaders. While those not in leadership positions are satisfied by having the Climate for Learning, the association was not significant for leaders. There is also no difference when we group developers by their gender. Based on these findings, in order to keep employees satisfied in their work, we recommend that companies offer professional development opportunities, where employees can learn new technology and management skills needed to advance their careers.

H6. Inclusiveness → Work Satisfaction: The association between Inclusiveness and Work Satisfaction holds positively across the whole sample. Additionally, the association showed different strengths when we compared genders. Women are twice more satisfied (*B*=.20) when having a welcoming and safe space for diversity than men (*B*=.10). Women represent one of the gender minorities and face prejudice and challenges in the tech workplace [\[76\]](#page-12-2). A welcoming and safe space allows them to thrive. Companies should evaluate the gender diversity of their tech workforce, expending effort in diversity recruitment and hiring, as well as in training programs that instill diversity and inclusion principles in their teams.

H7. Work Satisfaction→Burnout: Work Satisfaction has a negative association with Burnout, with no significant difference across groups.Burnout is the exhaustion caused by excessive and prolonged workplace stress, which can happen in software delivery teams due to the pressure of deadlines and high performance. However, we showed that Work Satisfaction represents an alleviating factor in reducing Burnout, which is aligned with previous research in software delivery teams [\[34\]](#page-11-10). So, although there were different antecedents to Work Satisfaction when achieved, satisfaction reduces Burnout across the groups of gender and leadership positions.

H8.c. Masculinity × Work Satisfaction → Burnout In a competitive and materialist culture (high levels of Masculinity), there was a great impact of work satisfaction in reducing burnout (This moderation had no effect for women.) According to Hofstede's framework of national cultures [\[44\]](#page-11-20), in Masculine cultures, men "should be" and women "may be" ambitious, work prevails over family, there is an admiration for the strong, fathers deal with facts and mothers with feelings, and girls cry and boys do not. In feminine cultures, fulfilling multiple social roles without social judgment is encouraged, so both men and women receive cultural support for prioritizing family time over time spent on the job [\[44\]](#page-11-20). Finding differences between groups is aligned with previous research that showed that people's well-being is achieved according to their current specific needs [\[21\]](#page-10-20). The result can be interpreted as masculine cultures drive men to strive for achievement and success, and when they perceive that they are successful (satisfied with their work) it reduces the perception of burnout. In feminine societies, men might feel uncomfortable and burn out more. Another possible interpretation is that men can take other measures to avoid burnout in masculine cultures, because the visible expressions of stress behavior may threaten the masculine value of heroism [\[77\]](#page-12-3). Therefore, organizations should consider the national culture where they operate and structure their incentives and career advancement opportunities accordingly.

#### VII. CONCLUSION

Attention to human factors is critical to software development employees' ability to perform. Globant is a large software services organization whose management sought to understand the concept of Burnout among their workforce. In this paper, we report on a theoretical model that seeks to explain how organizational culture and burnout in software delivery teams are associated. A large-scale survey with over 3,000 respondents provided sufficient data to test this model, and to distinguish between different subgroups (i.e., men/women and people on leadership/non-leadership roles). We argue that, given the international nature of this study that also considers the role of national culture (according to the Hofstede 6-D framework), albeit at one company, these findings are of interest to other large multinational organizations. Additionally, there are clear extension points of our study, as well as opportunities to replicate this study, which we think can contribute to a body of knowledge that considers critical human factors such as Burnout.

## ACKNOWLEDGMENTS

We thank all the survey participants for their time and insights. The National Science Foundation partially supports this work under Grant Numbers 1900903, 1901031, 2236198, 2235601, and Science Foundation Ireland grants no. 13/RC/2094-P2 to Lero, the SFI Research Centre for Software, and no. 15/SIRG/3293.

#### REFERENCES

- <span id="page-10-0"></span>[1] D. J. Madigan and L. E. Kim, "Towards an understanding of teacher attrition: A meta-analysis of burnout, job satisfaction, and teachers' intentions to quit," *Teaching and teacher education*, vol. 105, p. 103425, 2021.
- <span id="page-10-1"></span>[2] P. R. Mullen, A. Malone, A. Denney, and S. Santa Dietz, "Job stress, burnout, job satisfaction, and turnover intention among student affairs professionals," *College Student Affairs Journal*, vol. 36, no. 1, pp. 94–108, 2018.
- <span id="page-10-2"></span>[3] K. Mearns, L. Hope, M. T. Ford, and L. E. Tetrick, "Investment in workforce health: Exploring the implications for workforce safety climate and commitment," *Accident Analysis & Prevention*, vol. 42, no. 5, pp. 1445–1454, 2010.
- <span id="page-10-3"></span>[4] J. J. Phillips, P. P. Phillips, and A. Pulliam, *Measuring ROI in Environment, Health, and Safety*. John Wiley & Sons, 2014.
- <span id="page-10-4"></span>[5] N. Unsal, G. Weaver, J. W. Bray, D. Bibeau, and G. Saake, "Return on investment of workplace wellness: Evidence from a long-term care company," *Workplace Health & Safety*, vol. 69, no. 2, pp. 81–90, 2021.
- <span id="page-10-5"></span>[6] Gartner, "Great resignation or not, money won't fix all your talent problems," [https://www.gartner.com/en/articles/](https://www.gartner.com/en/articles/great-resignation-or-not-money-won-t-fix-all-your-talent-problems) [great-resignation-or-not-money-won-t-fix-all-your-talent-problems,](https://www.gartner.com/en/articles/great-resignation-or-not-money-won-t-fix-all-your-talent-problems) 2021.
- <span id="page-10-6"></span>[7] J. Weisberg, "Measuring workers' burnout and intention to leave," *International Journal of Manpower*, 1994.
- <span id="page-10-7"></span>[8] A. Pines and E. Aronson, *Burnout: From tedium to personal growth*. The Free Press, 1981.
- <span id="page-10-8"></span>[9] H. J. Freudenberger, "Staff burn-out," *Journal of Social Issues*, vol. 30, no. 1, pp. 159–165, 1974.
- <span id="page-10-9"></span>[10] C. Franc¸a, F. Q. Da Silva, and H. Sharp, "Motivation and satisfaction of software engineers," *IEEE Transactions on Software Engineering*, vol. 46, no. 2, pp. 118–140, 2018.
- <span id="page-10-10"></span>[11] G. G. Sharma and K.-J. Stol, "Exploring onboarding success, organizational fit, and turnover intention of software professionals," *Journal of Systems and Software*, vol. 159, p. 110442, 2020.
- <span id="page-10-11"></span>[12] K.-J. Stol, M. Schaarschmidt, and S. Goldblit, "Gamification in software engineering: the mediating role of developer engagement and job satisfaction," *Empirical Software Engineering*, vol. 27, no. 2, pp. 1– 34, 2022.
- <span id="page-10-12"></span>[13] A. Serenko, "The great resignation: the great knowledge exodus or the onset of the great knowledge revolution?" *Journal of Knowledge Management*, no. ahead-of-print, 2022.
- <span id="page-10-13"></span>[14] J. Sheather and D. Slattery, "The great resignation—how do we support and retain staff already stretched to their limit?" *BMJ*, p. n2533, Oct. 2021.
- <span id="page-10-14"></span>[15] N. Forsgren and J. Humble, "The role of continuous delivery in it and organizational performance," in *Proceedings of the Western Decision Sciences Institute (WDSI)*, 2016.
- <span id="page-10-15"></span>[16] K. Dora, R. P ´ eter, S. Z. P ´ eter, and C. Andrea, "The effect of organiza- ´ tional culture on employee well-being: Work-related stress, employee identification, turnover intention," *Journal of International Cooperation and Development*, vol. 2, no. 2, pp. 19–19, 2019.
- <span id="page-10-16"></span>[17] Google, "Dora research program," [https://www.devops-research.com/](https://www.devops-research.com/research.html/) [research.html/,](https://www.devops-research.com/research.html/) 2020, [Online; accessed 2022-06-14].
- <span id="page-10-17"></span>[18] C. G. Moreira, B. B. de Franc¸a, and T. U. Conte, "Organizational culture and its impact on the bizdev interface," in *2022 IEEE/ACM 44th International Conference on Software Engineering: Software Engineering in Practice (ICSE-SEIP)*. IEEE, 2022, pp. 209–210.
- <span id="page-10-18"></span>[19] R. Westrum, "A typology of organisational cultures," *BMJ Quality & Safety*, vol. 13, no. suppl 2, pp. ii22–ii27, 2004.
- <span id="page-10-19"></span>[20] K. Jelphs and H. Dickinson, *Working in teams*. Policy Press, 2016.
- <span id="page-10-20"></span>[21] N. Janicijevi ´ c, G. Nik ´ cevi ˇ c, and V. Vasi ´ c, "The influence of organizational ´ culture on job satisfaction," *Economic Annals*, vol. 63, no. 219, pp. 83– 114, 2018.
- <span id="page-10-21"></span>[22] J. Freiling and H. Fichtner, "Organizational culture as the glue between people and organization: A competence-based view on learning and competence building," *German Journal of Human Resource Management*, vol. 24, no. 2, pp. 152–172, 2010.
- <span id="page-10-22"></span>[23] A. Wolbling, K. Kr ¨ amer, C. N. Buss, K. Dribbisch, P. LoBue, and ¨ A. Taherivand, "Design thinking: An innovative concept for developing user-centered software," in *Management for Professionals*. Springer Berlin Heidelberg, 2012, pp. 121–136.

- <span id="page-11-0"></span>[24] P. Lok and J. Crawford, "The effect of organisational culture and leadership style on job satisfaction and organisational commitment: A cross-national comparison," *Journal of management development*, 2004.
- <span id="page-11-1"></span>[25] K. C. Brimhall, "Inclusion is important... but how do i include? examining the effects of leader engagement on inclusion, innovation, job satisfaction, and perceived quality of care in a diverse nonprofit health care organization," *Nonprofit and Voluntary Sector Quarterly*, vol. 48, no. 4, pp. 716–737, 2019.
- <span id="page-11-2"></span>[26] R. F. Baumeister and M. R. Leary, "The need to belong: Desire for interpersonal attachments as a fundamental human motivation," *Interpersonal development*, pp. 57–89, 2017.
- <span id="page-11-3"></span>[27] A. H. Maslow, "A theory of human motivation." *Psychological review*, vol. 50, no. 4, p. 370, 1943.
- <span id="page-11-4"></span>[28] B. M. Hagerty and K. Patusky, "Developing a measure of sense of belonging," *Nursing research*, vol. 44, no. 1, pp. 9–13, 1995.
- <span id="page-11-5"></span>[29] S. Lim, "Job satisfaction of information technology workers in academic libraries," *Library & Information Science Research*, vol. 30, no. 2, pp. 115–121, 2008.
- <span id="page-11-6"></span>[30] K.-A. Allen, "Making sense of belonging," *InPsych*, vol. 41, no. 3, 2019.
- <span id="page-11-7"></span>[31] A. N. Meyer, E. T. Barr, C. Bird, and T. Zimmermann, "Today was a good day: The daily life of software developers," *IEEE Transactions on Software Engineering*, vol. 47, no. 5, pp. 863–880, 2019.
- <span id="page-11-8"></span>[32] W. S. Jansen, M. W. Vos, S. Otten, A. Podsiadlowski, and K. I. van der Zee, "Colorblind or colorful? how diversity approaches affect cultural majority and minority employees," *Journal of Applied Social Psychology*, vol. 46, no. 2, pp. 81–93, 2016.
- <span id="page-11-9"></span>[33] W. S. Jansen, S. Otten, K. I. van der Zee, and L. Jans, "Inclusion: Conceptualization and measurement," *European journal of social psychology*, vol. 44, no. 4, pp. 370–385, 2014.
- <span id="page-11-10"></span>[34] N. Forsgren, M.-A. Storey, C. Maddila, T. Zimmermann, B. Houck, and J. Butler, "The space of developer productivity: There's more to it than you think." *Queue*, vol. 19, no. 1, pp. 20–48, 2021.
- <span id="page-11-11"></span>[35] S. N. Dolan, "The relationship between burnout and job satisfaction in nurses," *Journal of advanced nursing*, vol. 12, no. 1, pp. 3–12, 1987.
- <span id="page-11-12"></span>[36] E. W. Brewer and L. F. Clippard, "Burnout and job satisfaction among student support services personnel," *Human Resource Development Quarterly*, vol. 13, no. 2, pp. 169–186, 2002.
- <span id="page-11-13"></span>[37] L. T. Rattrie, M. G. Kittler, and K. I. Paul, "Culture, burnout, and engagement: A meta-analysis on national cultural values as moderators in jd-r theory," *Applied Psychology*, vol. 69, no. 1, pp. 176–220, 2020.
- <span id="page-11-14"></span>[38] M. C. Sturman, L. Shao, and J. H. Katz, "The effect of culture on the curvilinear relationship between performance and turnover." *Journal of Applied Psychology*, vol. 97, no. 1, p. 46, 2012.
- <span id="page-11-15"></span>[39] G. Hofstede, *Culture's consequences: Comparing values, behaviors, institutions and organizations across nations*. Sage publications, 2001.
- <span id="page-11-16"></span>[40] S. H. Schwartz, "A theory of cultural values and some implications for work," *Applied psychology*, vol. 48, no. 1, pp. 23–47, 1999.
- <span id="page-11-17"></span>[41] J. Chhokar, F. Brodbeck, and R. House, *Culture and leadership across the world*. Psychology Press, 2007.
- <span id="page-11-18"></span>[42] S. Lambiase, G. Catolino, D. A. Tamburri, A. Serebrenik, F. Palomba, and F. Ferrucci, "Good fences make good neighbours? on the impact of cultural and geographical dispersion on community smells," 2022.
- <span id="page-11-19"></span>[43] B. Trinkenreich, K.-J. Stol, A. Sarma, D. German, M. Gerosa, and I. Steinmacher, "Do i belong? modeling sense of virtual community among linux kernel contributors," in *International Conference on Software Engineering (ICSE 2023)*. IEEE, 2023.
- <span id="page-11-20"></span>[44] G. Hofstede, "Dimensionalizing cultures: The hofstede model in context," *Online readings in psychology and culture*, vol. 2, no. 1, pp. 2307–0919, 2011.
- <span id="page-11-21"></span>[45] G. Hofstede, G. J. Hofstede, and M. Minkov, *Cultures and organizations: Software of the mind*. Mcgraw-hill New York, 2005, vol. 2.
- <span id="page-11-22"></span>[46] Y. Gokmen, C. Baskici, and Y. Ercil, "The impact of national culture on the increase of covid-19: A cross-country analysis of european countries," *International Journal of Intercultural Relations*, vol. 81, pp. 1–8, 2021.
- <span id="page-11-23"></span>[47] S. Ronen and M. Mikulincer, "Attachment orientations and job burnout: The mediating roles of team cohesion and organizational fairness," *Journal of Social and Personal Relationships*, vol. 26, no. 4, pp. 549–567, 2009.
- <span id="page-11-24"></span>[48] D. I. Jung, B. M. Bass, and J. J. Sosik, "Bridging leadership and culture: A theoretical consideration of transformational leadership and collectivistic cultures," *Journal of Leadership Studies*, vol. 2, no. 4, pp. 3–18, 1995.
- <span id="page-11-25"></span>[49] W. Lin, L. Wang, and S. Chen, "Abusive supervision and employee wellbeing: The moderating effect of power distance orientation," *Applied Psychology*, vol. 62, no. 2, pp. 308–329, 2013.

- <span id="page-11-26"></span>[50] H. C. Triandis, "Cultural syndromes and subjective well-being," *Culture and subjective well-being*, pp. 13–36, 2000.
- <span id="page-11-27"></span>[51] C. Ringle, D. Da Silva, and D. Bido, "Structural equation modeling with the smartpls," *Bido, D., da Silva, D., & Ringle, C.(2014). Structural Equation Modeling with the Smartpls. Brazilian Journal Of Marketing*, vol. 13, no. 2, 2015.
- <span id="page-11-28"></span>[52] D. Russo and K.-J. Stol, "Pls-sem for software engineering research: An introduction and survey," *ACM Computing Surveys (CSUR)*, vol. 54, no. 4, pp. 1–38, 2021.
- <span id="page-11-29"></span>[53] Blind, "Replication package," [https://figshare.com/s/](https://figshare.com/s/3d6947c4d1676520568f) [3d6947c4d1676520568f,](https://figshare.com/s/3d6947c4d1676520568f) 2022.
- <span id="page-11-30"></span>[54] N. Forsgren, J. Humble, G. Kim, A. Brown, and N. Kersten, "Accelerate: State of devops strategies for a new economy," *Report. DevOps Research & Assessment (DORA)*, 2018.
- <span id="page-11-31"></span>[55] F. F. Reichheld and S. R. Covey, *The ultimate question: Driving good profits and true growth*. Harvard Business School Press Boston, 2006, vol. 211.
- <span id="page-11-32"></span>[56] P. Sedlak, "Employee net promoter score (enps) as a single-item measure of employee work satisfaction. an empirical evidence from companies operating in poland," *Contemporary Organisation and Management. Challenges and Trends, Michałkiewicz A. and Mierzejewska W.(eds), Wydawnictwo Uniwersytetu Łodzkiego, Ł ´ od´* , pp. 347–357, 2020.
- <span id="page-11-33"></span>[57] J. F. Hair, J. J. Risher, M. Sarstedt, and C. M. Ringle, "When to use and how to report the results of pls-sem," *European business review*, 2019.
- <span id="page-11-34"></span>[58] M. S. Bartlett, "Tests of significance in factor analysis." *British journal of psychology*, 1950.
- <span id="page-11-35"></span>[59] J. F. Hair Jr, R. E. Anderson, R. L. Tatham, and W. C. Black, "Multivariate data analysis with readings," 1995.
- <span id="page-11-36"></span>[60] N. Kock, "Advanced mediating effects tests, multi-group analyses, and measurement model assessments in pls-based sem," *International Journal of e-Collaboration (IJeC)*, vol. 10, no. 1, pp. 1–13, 2014.
- <span id="page-11-37"></span>[61] J. Henseler, C. M. Ringle, and M. Sarstedt, "A new criterion for assessing discriminant validity in variance-based structural equation modeling," *Journal of the academy of marketing science*, vol. 43, no. 1, pp. 115–135, 2015.
- <span id="page-11-38"></span>[62] J. F. Hair Jr, M. Sarstedt, C. M. Ringle, and S. P. Gudergan, *Advanced issues in partial least squares structural equation modeling*. saGe publications, 2017.
- <span id="page-11-39"></span>[63] S. Raithel, M. Sarstedt, S. Scharf, and M. Schwaiger, "On the value relevance of customer satisfaction. multiple drivers and multiple markets," *Journal of the Academy of Marketing Science*, vol. 40, no. 4, pp. 509–525, 2012.
- <span id="page-11-40"></span>[64] G. Shmueli, S. Ray, J. M. V. Estrada, and S. B. Chatla, "The elephant in the room: Predictive performance of pls models," *Journal of Business Research*, vol. 69, no. 10, pp. 4552–4564, 2016.
- <span id="page-11-41"></span>[65] G. Shmueli, M. Sarstedt, J. F. Hair, J.-H. Cheah, H. Ting, S. Vaithilingam, and C. M. Ringle, "Predictive model assessment in pls-sem: guidelines for using plspredict," *European journal of marketing*, 2019.
- <span id="page-11-42"></span>[66] J. Henseler, C. M. Ringle, and M. Sarstedt, "Testing measurement invariance of composites using partial least squares," *International marketing review*, 2016.
- <span id="page-11-43"></span>[67] C. M. Ringle and M. Sarstedt, "Gain more insight from your plssem results: The importance-performance map analysis," *Industrial management & data systems*, 2016.
- <span id="page-11-44"></span>[68] P. Ralph, S. Baltes, G. Adisaputri, R. Torkar, V. Kovalenko, M. Kalinowski, N. Novielli, S. Yoo, X. Devroey, X. Tan *et al.*, "Pandemic programming," *Empirical Software Engineering*, vol. 25, no. 6, pp. 4927– 4961, 2020.
- <span id="page-11-45"></span>[69] N. Almen and B. Jansson, "The reliability and factorial validity of ´ different versions of the shirom-melamed burnout measure/questionnaire and normative data for a general swedish sample." *International Journal of Stress Management*, 2021.
- <span id="page-11-46"></span>[70] K. S. Cortina, S. Arel, and J. P. Smith-Darden, "School belonging in different cultures: The effects of individualism and power distance," in *Frontiers in Education*, vol. 2. Frontiers, 2017, p. 56.
- <span id="page-11-47"></span>[71] K.-J. Stol and B. Fitzgerald, "The abc of software engineering research," *ACM Transactions on Software Engineering and Methodology (TOSEM)*, vol. 27, no. 3, p. 11, 2018.
- <span id="page-11-48"></span>[72] S. E. Fawcett, J. C. Brau, G. K. Rhoads, D. Whitlark, and A. M. Fawcett, "Spirituality and organizational culture: Cultivating the abcs of an inspiring workplace," *Intl Journal of Public Administration*, vol. 31, no. 4, pp. 420–438, 2008.
- <span id="page-11-49"></span>[73] S. M. Tabatabaee, A. Koohi, A. Ghandali, and T. Tajik, "The study of relationship between organizational culture and organizational belonging

- in employees of varamin county office of education." *International Education Studies*, vol. 9, no. 5, pp. 183–192, 2016.
- <span id="page-12-0"></span>[74] K.-A. Allen, *The Psychology of Belonging*. Routledge, 2020.
- <span id="page-12-1"></span>[75] K.-A. Allen, M. L. Kern, C. S. Rozek, D. M. McInerney, and G. M. Slavich, "Belonging: A review of conceptual issues, an integrative framework, and directions for future research," *Australian Journal of Psychology*, vol. 73, no. 1, pp. 87–102, 2021.
- <span id="page-12-2"></span>[76] B. Trinkenreich, I. Wiese, A. Sarma, M. Gerosa, and I. Steinmacher, "Women's participation in open source software: A survey of the literature," *ACM Trans Soft Eng Methodol*, vol. 31, no. 4, 2022.
- <span id="page-12-3"></span>[77] P. Tavel, R. Trnka, J. Furstova, N. Kascakova, M. Kuska, and Z. Meier, "Dispositional resilience predicted the perceived stress experienced by psychotherapists during the covid-19 outbreak." *Psychological Services*, 2022.