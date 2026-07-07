# Journal of Public Economics

journal homepage: <www.elsevier.com/locate/jpube>

![](_page_0_Picture_5.jpeg)

# How many jobs can be done at home?☆

Jonathan I. Dingel ⁎, Brent Neiman

University of Chicago, Booth School of Business, NBER, CEPR, United States of America

![](_page_0_Picture_9.jpeg)

## article info abstract

Article history: Received 27 April 2020 Received in revised form 19 June 2020 Accepted 21 June 2020 Available online 9 July 2020

Keywords: Remote work Telecommuting Work from home

Evaluating the economic impact of "social distancing" measures taken to arrest the spread of COVID-19 raises a fundamental question about the modern economy: how many jobs can be performed at home? We classify the feasibility of working at home for all occupations and merge this classification with occupational employment counts. We find that 37% of jobs in the United States can be performed entirely at home, with significant variation across cities and industries. These jobs typically pay more than jobs that cannot be done at home and account for 46% of all US wages. Applying our occupational classification to 85 other countries reveals that lower-income economies have a lower share of jobs that can be done at home.

© 2020 Elsevier B.V. All rights reserved.

## 1. Introduction

Evaluating the economic impact of "social distancing" measures taken to arrest the spread of COVID-19 raises a number of fundamental questions about the modern economy: How many jobs can be performed at home? What share of total wages are paid to such jobs? How does the scope for working from home vary across occupations, cities, industries, and countries?

We use surveys describing the typical experience of US workers in nearly 1000 occupations to classify each occupation as able or unable to be done entirely from home. We find that 37% of jobs in the United States can be performed entirely at home, with significant variation across cities and industries. These jobs typically pay more than jobs that cannot be done at home and account for 46% of all US wages.

Applying our occupational classification to 85 other countries reveals that lower-income economies have a lower share of jobs that can be done at home. Developing and emerging market countries with

E-mail addresses: [jdingel@chicagobooth.edu](mailto:jdingel@chicagobooth.edu) (J.I. Dingel), [brent.neiman@chicagobooth.edu](mailto:brent.neiman@chicagobooth.edu) (B. Neiman).

per capita GDP levels below one-third of US levels may only have half as many jobs that can be done from home.

Our measure, which was constructed using pre-pandemic data, correlates well with early estimates of the share of workers who have in fact worked from home during the crisis. Our online replication package reproduces and details all results summarized in the paper.1 We hope our work proves useful in identifying sectors that can safely operate without spreading the virus, in characterizing which workers face greater economic and health risks, and in pondering the likelihood of a future, after the public health crisis abates, in which remote working is far more common.

We start in Section 2 describing how we construct our work-fromhome measure using surveys from the Occupational Information Network (O\*NET). [Section 3](#page-1-0) reports the results of merging this occupation-level measure with information from the US Bureau of Labor Statistics (BLS) on the prevalence of each occupation in the aggregate US economy as well as in particular metropolitan areas and industries. In [Section 4,](#page-2-0) we merge our classification with occupational employment data for many countries provided by the International Labour Organization (ILO) to reveal a positive relationship between the share of jobs that can be done at home and a country's level of economic development. [Section 5](#page-3-0) reviews the related literature, including recent efforts to measure work-fromhome behavior during the initial months of the crisis. [Section 6](#page-5-0) concludes.

## 2. Classification of occupations

We classify the feasibility of working at home for all occupations using the responses to two surveys included in release 24.2 of the

<sup>☆</sup> We thank Menglu Xu and Mingjie Zhu for research assistance. A preliminary version of this research reporting results only for the United States appeared in the first issue of CEPR's Covid Economics: Vetted and Real-Time Papers. We are grateful to Megan Fasules for invaluable feedback on that version. In a subsequent version, we added results for 85 other countries and discussed related subsequent research. We thank the editor and three anonymous referees for suggestions that improved our presentation of our classification procedure and resulting geographic variation across US cities. Dingel thanks the James S. Kemper Foundation Faculty Research Fund at the University of Chicago Booth School of Business. Neiman thanks the William Ladany Faculty Foundation at the University of Chicago Booth School of Business and the Becker Friedman Institute at the University of Chicago for financial support.

<sup>⁎</sup> Corresponding author.

<sup>1</sup> All code and data are available at [https://github.com/jdingel/DingelNeiman](https://github.com/jdingel/DingelNeiman-workathome)[workathome](https://github.com/jdingel/DingelNeiman-workathome). Our code makes it easy for users to explore alternative assumptions about whether any given occupation can be done from home.

<span id="page-1-0"></span>database administered by O\*NET, a program sponsored by the US Department of Labor to improve our understanding of the nature of work and the workforce. The O\*NET database contains hundreds of standardized and occupation-specific descriptors on almost 1000 occupations. The first survey is called the Work Context Questionnaire and includes questions aiming to capture the "physical and social factors that influence the nature of work" such as interpersonal relationships, physical work conditions, and structural job characteristics. The second survey is called the Generalized Work Activities Questionnaire and includes questions aiming to capture the "general types of job behaviors occurring on multiple jobs" such as the input of information, interaction with others, mental processes, and work output. The median occupation had 26 respondents for each Work Context question and 25 respondents for each Generalized Work Activities question.

If any of the following conditions in the Work Context survey responses are true for an occupation, we code that occupation as one that cannot be performed at home:

- Average respondent says they use email less than once per month (Q4)
- Average respondent says they deal with violent people at least once a week (Q14)
- Majority of respondents say they work outdoors every day (Q17 & Q18)
- Average respondent says they are exposed to diseases or infection at least once a week (Q29)
- Average respondent says they are exposed to minor burns, cuts, bites, or stings at least once a week (Q33)
- Average respondent says they spent majority of time walking or running (Q37)
- Average respondent says they spent majority of time wearing common or specialized protective or safety equipment (Q43 & Q44)

If any of the following conditions in the Generalized Work Activities survey responses are true, we code the occupation as one that cannot be performed at home:

- Performing General Physical Activities is very important (Q16A)
- Handling and Moving Objects is very important (Q17A)
- Controlling Machines and Processes [not computers nor vehicles] is very important (Q18A)
- Operating Vehicles, Mechanized Devices, or Equipment is very important (Q20A)
- Performing for or Working Directly with the Public is very important (Q32A)
- Repairing and Maintaining Mechanical Equipment is very important (Q22A)
- Repairing and Maintaining Electronic Equipment is very important (Q23A)
- Inspecting Equipment, Structures, or Materials is very important (Q4A)

We then merge this information with BLS data on the number and wages of workers in each standard occupational classification (SOC) code in the country as a whole as well as in metropolitan areas and industries.

[Table A.1](#page-5-0) in [Appendix A](#page-5-0) summarizes the contribution of each O\*NET survey question to our classification of which occupations can be done from home in two ways. First, the columns labeled "Cannot do at home" report the shares of jobs (unweighted and weighted by their wages) that satisfy each condition causing us to classify an occupation as unable to be performed entirely at home. "Majority of time walking or running" and "majority of time wearing protective or safety equipment" are the two conditions that are satisfied most frequently. Multiple conditions can hold for any single occupation, so the sum of these shares far exceeds the share of jobs that we infer cannot be performed entirely at home. Second, the columns labeled "Sole condition" consider the 14% of employment held by occupations where a single condition alone renders the occupation unable to be done from home. Among those cases, "performing or working directly with the public" is the condition that mostly commonly causes this classification.

To check the sensibility of our algorithm, we each manually assigned values of 0, 0.5, or 1 to each 5-digit SOC code based on introspection and then averaged our judgments. Our two assessments about whether an occupation could be done at home or not agreed in about 85% of the cases, and our disagreements were only rarely greater than 0.5. The scores generated by this manual assignment are highly correlated with our O\*NETderived classification, though we manually assigned slightly fewer occupations as able to work from home. Appendix [Table A.2](#page-6-0) reports the 5 digit occupation codes for which the two measures differ by 0.8 or more.

## 3. Results for the United States

Our classification implies that 37% of US jobs can plausibly be performed at home. Our classification uses job characteristics that clearly rule out the possibility of working entirely from home and neglects many characteristics that would merely make working from home difficult.<sup>2</sup> It is, therefore, an upper bound on what might be feasible and greatly exceeds the share of jobs that in fact have been performed entirely at home in recent years. According to the 2018 American Time Use Survey, less than a quarter of all full-time workers work at all from home on an average day, and even those workers typically spend well less than half of their working hours at home.

[Table 1](#page-2-0) reports the share of jobs that can be performed at home when we aggregate our occupational classification to the major group (2-digit) level. There is significant variation across occupations. Managers, educators, and those working in computers, finance, and law are largely able to work from home. Farm, construction, and production workers cannot.

Workers in occupations that can be performed at home typically earn more. If we assume all occupations involve the same number of hours of work, the 37% of US jobs that can plausibly be performed at home account for 46% of all wages. [Fig. 1](#page-2-0) plots the share of jobs that can be done at home in each major occupation group against its median hourly wage.3 There is a clear positive relationship between our workfrom-home measure and the typical hourly earnings at the occupation level. [Mongey et al. \(2020\)](#page-7-0) use a variant of our occupational classification to study the characteristics of individuals who cannot work at home. They find that these individuals are more likely to be lowerincome, lack a college degree, rent their dwellings, be non-white, and lack employer-provided health insurance.

There is significant variation in the share of jobs that can be done at home across US cities. The first two columns in [Table 2](#page-3-0) report the top ten and bottom ten metropolitan statistical areas (from among the 100 largest, by employment) in terms of the share of jobs (unweighted and weighted by wage) that could be done at home. More than 45% of jobs in San Francisco, San Jose, and Washington, DC could be performed at home, whereas this is the case for 30% or less of the jobs in Fort Myers, Grand Rapids, and Las Vegas. [Fig. A.1](#page-7-0) in [Appendix A](#page-5-0) depicts the geographic distribution of our unweighted measure of the share of jobs that can be done at home across metropolitan areas.

The last four columns of [Table 2](#page-3-0) list for each city the characteristics analyzed by [Mongey et al. \(2020\)](#page-7-0). Across all metropolitan areas, the share of jobs that can be performed at home is strongly positively correlated with median household income (0.53) and its share of residents who attained a college degree (0.71) and negatively correlated with its home ownership rate (−0.31) and its share of residents who are

<sup>2</sup> For example, our classification codes 98% of the 8.8 million teachers in the United States as able to work from home, which seems sensible given the large number of schools currently employing remote learning. Re-coding these teaching jobs as unable to be performed from home would, in the aggregate, reduce our estimate of the share of jobs that can be done at home by about six percentage points.

<sup>3</sup> In an earlier blogpost, [Avdiu and Nayyar \(2020\)](#page-7-0) plotted an equivalent relationship between our measure of the share of jobs that can be done at home and the occupation's income decile. [Costa Dias et al. \(2020\)](#page-7-0) provide related evidence for the United Kingdom.

<span id="page-2-0"></span>Table 1 Share of jobs that can be done at home, by occupation's major group.

| Occupation |                                                            | O*NET-derived baseline | Manual assignment |
|------------|------------------------------------------------------------|------------------------|-------------------|
| 15         | Computer and Mathematical Occupations                      | 1.00                   | 1.00              |
| 25         | Education, Training, and Library Occupations               | 0.98                   | 0.85              |
| 23         | Legal Occupations                                          | 0.97                   | 0.84              |
| 13         | Business and Financial Operations Occupations              | 0.88                   | 0.92              |
| 11         | Management Occupations                                     | 0.87                   | 0.84              |
| 27         | Arts, Design, Entertainment, Sports, and Media Occupations | 0.76                   | 0.57              |
| 43         | Office and Administrative Support Occupations              | 0.65                   | 0.51              |
| 17         | Architecture and Engineering Occupations                   | 0.61                   | 0.88              |
| 19         | Life, Physical, and Social Science Occupations             | 0.54                   | 0.36              |
| 21         | Community and Social Service Occupations                   | 0.37                   | 0.50              |
| 41         | Sales and Related Occupations                              | 0.28                   | 0.21              |
| 39         | Personal Care and Service Occupations                      | 0.26                   | 0.00              |
| 33         | Protective Service Occupations                             | 0.06                   | 0.00              |
| 29         | Healthcare Practitioners and Technical Occupations         | 0.05                   | 0.06              |
| 53         | Transportation and Material Moving Occupations             | 0.03                   | 0.00              |
| 31         | Healthcare Support Occupations                             | 0.02                   | 0.00              |
| 45         | Farming, Fishing, and Forestry Occupations                 | 0.01                   | 0.00              |
| 51         | Production Occupations                                     | 0.01                   | 0.00              |
| 49         | Installation, Maintenance, and Repair Occupations          | 0.01                   | 0.00              |
| 47         | Construction and Extraction Occupations                    | 0.00                   | 0.00              |
| 35         | Food Preparation and Serving Related Occupations           | 0.00                   | 0.00              |
| 37         | Building and Grounds Cleaning and Maintenance Occupations  | 0.00                   | 0.00              |

NOTES: This table reports the share of jobs that can be done at home for each 2-digit SOC major group. We aggregate our 6-digit SOC classification using the employment counts in the BLS's 2018 Occupational Employment Statistics. The O\*NET-derived classification in the first column is the basis for all subsequent results reported in this paper. The results using the manual assignment, reported in the second column, are available in our replication package.

white (−0.12). The fact that the latter two cross-city correlations have the opposite sign of the corresponding cross-individual correlations reported by [Mongey et al. \(2020\)](#page-7-0) underlines the importance of distinguishing between people and places when describing variation in economic conditions.

[Table 3](#page-3-0) aggregates our classification to the 2-digit industry level. Whereas most jobs in finance, corporate management, and professional and scientific services could plausibly be performed at home, very few jobs in agriculture, hotels and restaurants, or retail could be.

## 4. Results for countries other than the United States

To produce estimates for other countries, we merge our work-fromhome classification of each 6-digit SOC based on the US O\*NET surveys with the 2008 edition of the international standard classification of occupations (ISCO) at the 2-digit level. The ISCO standard for classifying occupations was adopted by the ILO, which compiles information on employment in each 2-digit ISCO for a large number of countries. We employ a crosswalk between the SOC and ISCO schemes from the US BLS.

The mapping of (6-digit) SOCs to (2-digit) ISCOs is many-tomany, so determining the share of jobs that can be done from home in any ISCO is not trivial. To summarize, our classification of whether a 6-digit SOC can be done at home is determined entirely using only US data, our mapping of 6-digit SOCs to 2 digit ISCOs is common to all countries, and the weighted average for each 2-digit ISCO is country-specific. For more details, see [Appendix A.](#page-5-0)

![](_page_2_Figure_11.jpeg)

Fig. 1. Jobs that can be done at home typically earn higher wages. NOTES: This graph depicts the median hourly wage and share of jobs that can be done at home for each 2-digit SOC major group. We compute these shares using our O\*NET-derived classification of occupations that can be done at home and employment counts in the BLS's 2018 Occupational Employment Statistics. The latter is the source of median hourly wages.

<span id="page-3-0"></span>Table 2 Share of jobs that can be done at home, by metropolitan area.

|                                              | Share of jobs |                  | Metropolitan characteristics |               |             |             |
|----------------------------------------------|---------------|------------------|------------------------------|---------------|-------------|-------------|
|                                              | Unweighted    | Weighted by wage | BA share                     | Median income | White share | Owner share |
| Top ten                                      |               |                  |                              |               |             |             |
| San Jose-Sunnyvale-Santa Clara, CA           | 0.51          | 0.66             | 0.50                         | 115           | 0.46        | 0.57        |
| Washington-Arlington-Alexandria, DC-VA-MD-WV | 0.50          | 0.64             | 0.51                         | 101           | 0.54        | 0.63        |
| Durham-Chapel Hill, NC                       | 0.46          | 0.57             | 0.47                         | 60            | 0.62        | 0.60        |
| Austin-Round Rock, TX                        | 0.46          | 0.58             | 0.44                         | 73            | 0.77        | 0.58        |
| San Francisco-Oakland-Hayward, CA            | 0.45          | 0.58             | 0.49                         | 100           | 0.50        | 0.54        |
| Boston-Cambridge-Nashua, MA-NH               | 0.44          | 0.55             | 0.47                         | 86            | 0.76        | 0.62        |
| Bridgeport-Stamford-Norwalk, CT              | 0.44          | 0.58             | 0.47                         | 93            | 0.73        | 0.67        |
| Hartford-West Hartford-East Hartford, CT     | 0.44          | 0.53             | 0.39                         | 76            | 0.76        | 0.67        |
| Salt Lake City, UT                           | 0.43          | 0.53             | 0.34                         | 71            | 0.80        | 0.67        |
| Des Moines-West Des Moines, IA               | 0.43          | 0.53             | 0.37                         | 69            | 0.87        | 0.69        |
| Bottom ten                                   |               |                  |                              |               |             |             |
| Baton Rouge, LA                              | 0.30          | 0.36             | 0.28                         | 57            | 0.59        | 0.68        |
| Las Vegas-Henderson-Paradise, NV             | 0.30          | 0.37             | 0.24                         | 57            | 0.61        | 0.53        |
| Riverside-San Bernardino-Ontario, CA         | 0.30          | 0.35             | 0.21                         | 62            | 0.61        | 0.63        |
| Scranton–Wilkes-Barre–Hazleton, PA           | 0.30          | 0.36             | 0.25                         | 52            | 0.90        | 0.68        |
| McAllen-Edinburg-Mission, TX                 | 0.30          | 0.31             | 0.18                         | 38            | 0.88        | 0.68        |
| Grand Rapids-Wyoming, MI                     | 0.29          | 0.37             | 0.32                         | 61            | 0.84        | 0.73        |
| Lancaster, PA                                | 0.29          | 0.36             | 0.27                         | 64            | 0.89        | 0.68        |
| Bakersfield, CA                              | 0.29          | 0.36             | 0.16                         | 52            | 0.75        | 0.58        |
| Stockton-Lodi, CA                            | 0.29          | 0.33             | 0.18                         | 61            | 0.56        | 0.56        |
| Cape Coral-Fort Myers, FL                    | 0.28          | 0.34             | 0.28                         | 55            | 0.85        | 0.71        |

NOTES: This table reports the metropolitan areas with the largest and smallest shares of jobs that can be done at home among the 100 largest metropolitan areas (as ranked by total employment). The first two columns report these shares unweighted and weighted by average wages. The remaining four columns report the metropolitan areas' fraction of population 25 years or older whose educational attainment is bachelor's degree or higher (series B15003), median household income in thousands of (2018) US dollars (B19013), fraction of residents whose race is "white alone" (B02001), and fraction of housing units that are owner-occupied (B25003), as reported in the American Community Survey 2014–2018 5-Year Estimates for metropolitan areas.

[Fig. 2\(](#page-4-0)a) plots our measure of the share of jobs that can be done at home in each country against its per capita income. We compute the jobs share using the most recent employment data available from the ILO after restricting attention to countries that report employment data for 2015 or later. The income measure is GDP per capita in 2019 adjusted for purchasing power parity (PPP). The figure reveals a clear positive relationship between income levels and the shares of jobs that can be done from home. While fewer than 25% of jobs in Mexico and Turkey could be performed at home, this share exceeds 40% in Sweden and the

Table 3 Share of jobs that can be done at home, by industry.

|                                                                             | Unweighted | Weighted<br>by wage |
|-----------------------------------------------------------------------------|------------|---------------------|
| Educational Services                                                        | 0.83       | 0.71                |
| Professional, Scientific, and Technical Services                            | 0.80       | 0.86                |
| Management of Companies and Enterprises                                     | 0.79       | 0.86                |
| Finance and Insurance                                                       | 0.76       | 0.85                |
| Information                                                                 | 0.72       | 0.80                |
| Wholesale Trade                                                             | 0.52       | 0.67                |
| Real Estate and Rental and Leasing                                          | 0.42       | 0.54                |
| Federal, State, and Local Government                                        | 0.41       | 0.47                |
| Utilities                                                                   | 0.37       | 0.41                |
| Other Services (except Public Administration)                               | 0.31       | 0.43                |
| Administrative and Support and Waste Management<br>and Remediation Services | 0.31       | 0.43                |
| Arts, Entertainment, and Recreation                                         | 0.30       | 0.36                |
| Mining, Quarrying, and Oil and Gas Extraction                               | 0.25       | 0.37                |
| Health Care and Social Assistance                                           | 0.25       | 0.24                |
| Manufacturing                                                               | 0.22       | 0.36                |
| Transportation and Warehousing                                              | 0.19       | 0.25                |
| Construction                                                                | 0.19       | 0.22                |
| Retail Trade                                                                | 0.14       | 0.22                |
| Agriculture, Forestry, Fishing and Hunting                                  | 0.08       | 0.13                |
| Accommodation and Food Services                                             | 0.04       | 0.07                |

NOTES: This table reports the share of jobs that can be done at home in each 2-digit NAICS sector. We compute these shares using our O\*NET-derived classification of occupations that can be done at home and the occupational composition of each 2-digit sector's employment by 6-digit SOC in the BLS's 2018 Occupational Employment Statistics.

United Kingdom.4 Note that our classification assesses the ability to perform a particular occupation from home based on US data and that the nature of an occupation likely varies across economies with different income levels. With that caveat, the striking pattern in [Fig. 2\(](#page-4-0)a) suggests that developing economies and emerging markets may face an even greater challenge in continuing to work during periods of stringent social distancing.

## 5. Related literature and real-time measures

Our coding of occupational characteristics to determine how flexibly certain jobs can be relocated has clear roots in the exercise in [Blinder](#page-7-0) [\(2009\)](#page-7-0) that assessed the "offshorability" of jobs. While our approach is similar, we cannot simply use Blinder's index because the feasibility of working from home is quite distinct from offshorability. For example, [Blinder and Krueger \(2013\)](#page-7-0) write, "we know that all textile manufacturing jobs in the United States are offshorable." Textile manufacturing jobs, of course, cannot be performed at home using current production technologies.

Several papers document the prevalence and consequences of working from home. [Oettinger \(2011\)](#page-7-0) investigates the growth in home-based work from 1980 to 2000, as reported in the US Census of Population, and relates these changes to the frequency of faceto-face interactions, as measured in an O\*NET survey. [Bloom et al.](#page-7-0) [\(2015\)](#page-7-0) estimate the effects of home-based work on employees' productivity using a randomized controlled trial within a Chinese travel agency. [Mas and Pallais \(2020\)](#page-7-0) offer a detailed and helpful overview of the prevalence, features, and demand for alternative working arrangements, including the ability to work from home. Citing the Quality of Worklife Survey and the Understanding American Study, they report that less than 13% of full- and part-time jobs have a formal "work-from-home" arrangement, even though twice that

<sup>4</sup> The share for the United States in [Fig. 2\(](#page-4-0)a) is 41%. This differs from the 37% reported in the main text due to the different weights implicit in our use of ILO data rather than BLS data.

<span id="page-4-0"></span>![](_page_4_Figure_2.jpeg)

![](_page_4_Figure_4.jpeg)

Fig. 2. Cross-country variation in share of jobs that can be done at home. NOTES: Panel (a) depicts the share of jobs that can be done at home and GDP per capita for 86 economies. The shares are computed by mapping our classification of 6-digit SOC codes to 2-digit ISCO codes using country-specific weights as described in [Appendix A.](#page-5-0) We use the most recent 2-digit ISCO employment counts available from the ILO for 2015 or later. GDP per capita in 2019 (at current prices and translated into international dollars using PPP exchange rates) comes from the International Monetary Fund. Panel (b) compares our country-level measures to the share of Eurofound survey respondents in 26 European countries reporting that they started to work from home due to COVID-19.

amount work often from home.<sup>5</sup> According to Mas and Pallais, the "median worker reports that only 6 percent of their job could be feasibly done from home," but plenty of jobs, including those in "computer and

<sup>5</sup> United Kingdom Offi[ce for National Statistics \(2020\)](#page-7-0) surveys conducted in 2019 found that while 27% of the U.K. workforce said they've previously worked from home, only about 5% said they mainly work from home. Whether people have actually worked from home differs conceptually from the focal question of this paper, which is whether these people could feasibly work from home.

mathematical" and "business and financial operations" can do a majority of their work from home. We note that, in the context of the response to COVID-19, there is an important distinction between being able to do most and all of one's work at home.

[Saltiel \(2020\)](#page-7-0) estimates the share of jobs that can be done from home in ten developing economies using surveys of occupations in those ten lower-income contexts. Following our approach, he uses information on workers' tasks in the Skills Toward Employability and Productivity (STEP) survey to define the feasibility of working from home. <span id="page-5-0"></span>The advantage of using these data is that it addresses the concerns raised by defining the feasibility of performing a job at home based on the US economic context.<sup>6</sup> [Saltiel \(2020\)](#page-7-0) finds that few jobs can be done at home, ranging from 5% to 23% across the ten economies, and reports a positive correlation between this share and GDP per capita. Five of the economies covered by [Saltiel \(2020\)](#page-7-0) also appear in our [Section 4](#page-2-0) results. Our results for Bolivia, Georgia, and Macedonia are within a few percentage points of the numbers Saltiel reports. Our results for Ghana and Laos are notably higher, 14% and 21% versus roughly 5% and 9%, respectively. In addition to differences in the O\*NET and STEP survey questions, these differences may be attributable to the ILO data and STEP survey differing in temporal (2017 vs 2012–2013) and geographic (national vs urban) coverage.

In addition to characterizing who works in the jobs that can be done at home, [Mongey et al. \(2020\)](#page-7-0) use O\*NET data to produce job-level measures of physical proximity in the workplace. [Baker \(2020\)](#page-7-0) and [Koren and Petö \(2020\)](#page-7-0) also use O\*NET survey data to construct measures of which occupations cannot be done at home or will be affected by social distancing.

Recent research uses surveys to produce real-time measures of working from home. For the United States, [Brynjolfsson et al. \(2020\)](#page-7-0) report that nearly half of the individuals they surveyed said they were working from home during the first week of April 2020, while [Bick](#page-7-0) [et al. \(2020\)](#page-7-0) report that 35% of their US respondents worked entirely from home in May 2020. Examining cross-industry variation, [Bick](#page-7-0) [et al. \(2020\)](#page-7-0) find that the share of respondents in an industry working from home in May is highly correlated with our estimate of the feasible share for that industry. The Decision Maker Panel, an entity set up by the Bank of England, conducts a real-time survey of U.K. firms and shows that 37% of employees were reported to be working from home in both April and May 2020.7 Finally, [Eurofound \(2020\)](#page-7-0) tabulates results from a survey of more than 85,000 people and reports for 26 European Union countries the share of employees who started working from home as a result of COVID-19. [Fig. 2\(](#page-4-0)b) plots these results against our country-level estimates discussed in [Section 4](#page-2-0) and shows a very close correspondence.

### 6. Conclusion

Due to COVID-19, many employees are unable to travel to work. Identifying which jobs cannot be performed from home is useful as policymakers try to target social insurance payments to those that most need them. Likewise, the share of jobs that could be performed at home is an important input to predicting the economy's performance during this or subsequent periods of social distancing.8 We note, however, that it is not straightforward to use these values to estimate the share of output that would be produced under stringent stay-at-home policies. An individual worker's productivity may differ considerably when working at home rather than her usual workplace. More importantly, there are likely important complementarities between jobs that can be performed at home and those that cannot. Incorporating our measures together with these richer considerations is a fruitful avenue for future research.

## Appendix A

This Appendix describes how we map 6-digit SOC codes to 2-digit ISCO codes for our analysis of countries other than the United States. It also presents one figure and two tables that are mentioned in the main text.

## A.1. Mapping to international occupational codes

This section describes how we map 6-digit SOCs to 2-digit ISCOs. Ideally, each SOC would map to a unique ISCO, so that we could simply calculate the ISCO share as a weighted average of SOC shares, using the SOCs' US employment counts as the weights. However, given the many-to-many mapping, this approach would put disproportionate weight on those SOCs that happen to map to a larger number of ISCOs. To address this issue, when an SOC maps to multiple ISCOs, we allocate the SOC's US employment weight across the ISCOs in proportion to the ISCOs' employment shares in the "target" country. For instance, if a particular SOC has 100 US employees and is associated with two ISCOs that have respective totals of 3000 and 1000 employees in a country, we allocate 75 of the SOC's US employees to the larger ISCO and 25 to the smaller one. Those values of 75 and 25 are then used as that SOC's weight when calculating the average across all SOCs within each ISCO for that country. Since 2-digit ISCO employment shares vary by country, the reported share of jobs that can be done from home in each 2-digit ISCO differs across countries.

## A.2. Additional exhibits

Table A.1

| O*NET survey condition                                                    | Cannot do at home |       | Sole condition |       |
|---------------------------------------------------------------------------|-------------------|-------|----------------|-------|
| Contributions of O*NET survey questions to classification of occupations. | Jobs              | Wages | Jobs           | Wages |
| GWA23: Repairing and Maintaining Electronic Equipment                     | 0.01              | 0.01  | 0.000          | 0.000 |
| WC14: Deal with violent people weekly                                     | 0.01              | 0.01  | 0.003          | 0.003 |
| GWA22: Repairing and Maintaining Mechanical Equipment                     | 0.02              | 0.02  | 0.000          | 0.000 |
| WC33: Exposed to minor burns, cuts, bites, or stings weekly               | 0.02              | 0.02  | 0.000          | 0.000 |
| WC17/18: Majority of respondents say outdoors every day                   | 0.04              | 0.04  | 0.000          | 0.000 |
| GWA18: Controlling Machines and Processes                                 | 0.05              | 0.04  | 0.000          | 0.000 |

<sup>6</sup> [Gottlieb et al. \(2020\)](#page-7-0) apply our classification of occupations to labor force and household surveys in 57 countries. In line with our findings, they report that smaller shares of jobs can be done at home in poorer economies. They note, however, that small family farms in principle could operate while limiting social interactions and obeying stay-at-home orders. Classifying all farming jobs as such substantially increases the estimated share of jobs that can be done at home in some poor economies with large agricultural employment shares. [Stratton \(2020\)](#page-7-0) applies our classification to data for Australia. [Barbieri et al. \(2020\)](#page-7-0) use the Italian equivalent of the O\*NET surveys and a similar set of questions to produce a work-from-home measure for Italy. [Boeri et al. \(2020\)](#page-7-0) combine O\*NET information, a survey of the Italian Statistical Office and INAP, and their own assessment to estimate how many jobs can potentially be carried out remotely for six European economies.

<sup>7</sup> [Adams-Prassl et al. \(2020\)](#page-7-0) also used surveys in Germany, the United Kingdom, and the United States to conclude that workers that are less able to do tasks at home are more likely to experience reduced hours, lower earnings, and job losses. [Cajner et al. \(2020\)](#page-7-0) use payroll-processing data for the United States and find a more modest correlation between an industry's job losses and our measure of the feasibility of working from home.

<sup>8</sup> Our or similar measures of the capacity for working from home are used to calibrate quantitative models of the pandemic including [Bonadio et al. \(2020\),](#page-7-0) [Jones et al. \(2020\)](#page-7-0), [Kaplan](#page-7-0) [et al. \(2020\),](#page-7-0) and [Rampini \(2020\)](#page-7-0).

<span id="page-6-0"></span>Table A.1 (continued)

| O*NET survey condition                                           | Cannot do at home |       | Sole condition |       |
|------------------------------------------------------------------|-------------------|-------|----------------|-------|
|                                                                  | Jobs              | Wages | Jobs           | Wages |
| GWA20: Operating Vehicles, Mechanized Devices, or Equipment      | 0.06              | 0.06  | 0.010          | 0.007 |
| WC29: Exposed to diseases or infection weekly                    | 0.08              | 0.11  | 0.001          | 0.004 |
| GWA17: Handling and Moving Objects                               | 0.09              | 0.07  | 0.001          | 0.001 |
| GWA16: Performing General Physical Activities                    | 0.11              | 0.09  | 0.002          | 0.002 |
| GWA4: Inspecting Equipment, Structures, or Materials             | 0.11              | 0.12  | 0.000          | 0.000 |
| WC4: Use email less than once per month                          | 0.17              | 0.11  | 0.006          | 0.003 |
| GWA32: Performing for or Working Directly with the Public        | 0.22              | 0.18  | 0.086          | 0.063 |
| WC37: Majority of time walking or running                        | 0.29              | 0.20  | 0.001          | 0.001 |
| WC43/44: Majority of time wearing protective or safety equipment | 0.39              | 0.35  | 0.027          | 0.033 |

NOTES: This table summarizes the contribution of each O\*NET survey question to our classification of occupations. The questions come from the Work Context ("WC") and Generalized Work Activities ("GWA") survey. For each question, the first two columns report the fraction of employment and wage-weighted employment that the survey question says cannot be performed entirely at home. Multiple conditions can hold for any single occupation, so the sum of these shares far exceeds the 63% of jobs that we infer cannot be performed entirely at home. The third and fourth columns report the fraction of employment and wage-weighted employment for which the survey question is the only question indicating that these occupations cannot be performed entirely at home. In total, 14% of employment is in occupations that a single survey condition implies cannot be performed at home. All employment and wage data are from the BLS's 2018 Occupational Employment Statistics.

Table A.2 Occupations for which O\*NET-derived and manual measures differ considerably.

| Occupation |                                                                     | O*NET-derived | Manual<br>assignment |
|------------|---------------------------------------------------------------------|---------------|----------------------|
|            |                                                                     | Baseline      |                      |
| 13-113     | Fundraisers                                                         | 0.00          | 1                    |
| 13-208     | Tax Examiners, Collectors and Preparers, and Revenue Agents         | 0.00          | 1                    |
| 19-305     | Urban and Regional Planners                                         | 0.00          | 1                    |
| 41-304     | Travel Agents                                                       | 0.00          | 1                    |
| 43-202     | Telephone Operators                                                 | 0.00          | 1                    |
| 43-418     | Reservation and Transportation Ticket Agents and Travel Clerks      | 0.00          | 1                    |
| 13-207     | Credit Counselors and Loan Officers                                 | 0.10          | 1                    |
| 17-302     | Engineering Technicians, Except Drafters                            | 0.17          | 1                    |
| 39-301     | Gaming Services Workers                                             | 0.85          | 0                    |
| 25-205     | Special Education Teachers                                          | 0.92          | 0                    |
| 27-202     | Athletes, Coaches, Umpires, and Related Workers                     | 0.93          | 0                    |
| 25-201     | Preschool and Kindergarten Teachers                                 | 1.00          | 0                    |
| 25-402     | Librarians                                                          | 1.00          | 0                    |
| 25-403     | Library Technicians                                                 | 1.00          | 0                    |
| 27-402     | Photographers                                                       | 1.00          | 0                    |
| 33-902     | Private Detectives and Investigators                                | 1.00          | 0                    |
| 39-303     | Ushers, Lobby Attendants, and Ticket Takers                         | 1.00          | 0                    |
| 39-901     | Childcare Workers                                                   | 1.00          | 0                    |
| 39-904     | Residential Advisors                                                | 1.00          | 0                    |
| 43-101     | First-Line Supervisors of Office and Administrative Support Workers | 1.00          | 0                    |
| 43-502     | Couriers and Messengers                                             | 1.00          | 0                    |
| 43-905     | Mail Clerks and Mail Machine Operators, Except Postal Service       | 1.00          | 0                    |
| 43-907     | Office Machine Operators, Except Computer                           | 1.00          | 0                    |

NOTES: This table reports all 5-digit SOC codes for which the O\*NET-derived classification and our manual assignment differ by 0.8 or more. Since the O\*NET-derived measure is defined for 6-digit occupations, this measure is not necessarily 0 or 1 at the 5-digit level. We aggregate 6-digit occupations weighting by employment counts in the BLS's 2018 Occupational Employment Statistics.

<span id="page-7-0"></span>![](_page_7_Figure_2.jpeg)

Fig. A.1. Share of jobs that can be done at home Notes: This map depicts the share of jobs that can be done at home for 388 core-based statistical areas (CBSAs). We compute these shares using our O\*NET-derived classification of occupations that can be done at home and the occupational composition of each CBSA's employment by 6-digit SOC in the BLS's 2018 Occupational Employment Statistics. The map depicts CBSAs based on 2013 definitions.

### References

Adams-Prassl, Abi, Boneva, Teodora, Golin, Marta, Rauh, Christopher, 2020, Inequality in the Impact of the Coronavirus Shock: Evidence from Real Time Surveys.

Avdiu, Besart, Nayyar, Gaurav, 2020. When Face-to-face Interactions Become an Occupational Hazard: Jobs in the Time of COVID-19 (Brookings Future Development Blog).

Baker, Marissa G. 2020. "Characterizing occupations that cannot work from home: a means to identify susceptible worker groups during the COVID-19 pandemic." medRxiv.

Barbieri, Teresa, Gaetano Basso, and Sergio Scicchitano. 2020. "Italian Workers at Risk during the COVID-19 Epidemic." https://doi.org/10.2139/ssrn.3572065.

Bick, Alexander, Blandin, Adam, Mertens, Karel, 2020. Work From Home After the COVID-19 Outbreak

Blinder, Alan, 2009, How many US jobs might be offshorable? World Econ, 10 (2), 41–78. Blinder, Alan S., Krueger, Alan B., 2013. Alternative measures of offshorability: a survey approach. J. Labor Econ. 31 (S1), 97-128.

Bloom, Nicholas, Liang, James, Roberts, John, Ying, Zhichun Jenny, 2015. Does working from home work? Evidence from a Chinese experiment. Q. J. Econ. 130 (1), 165-218.

Boeri, Tito, Caiumi, Alessandro, Paccagnella, Marco, 2020. Mitigating the work-safety trade-off. Covid Economics: Vetted and Real-Time Papers 1 (2), 60-66.

Bonadio, Barthélémy, Huo, Zhen, Levchenko, Andrei A., Pandalai-Nayar, Nitya, 2020. Global Supply Chains in the Pandemic. National Bureau of Economic Research working paper 27224.

Brynjolfsson, Erik, John Horton, Adam Ozimek, Daniel Rock, Garima Sharma, and Hong Yi Tu Ye. 2020. "COVID-19 and Remote Work: An Early Look at US Data." 8 April mimeo. Cajner, Tomaz, Leland D Crane, Ryan A Decker, John Grigsby, Adrian Hamins-Puertolas, Erik Hurst, Christopher Kurz, and Ahu Yildirmaz. 2020. "The U.S. Labor Market during

the Beginning of the Pandemic Recession." National Bureau of Economic Research Working Paper 27159.

Costa Dias, Monica, Christine Farguharson, Rachel Griffith, Robert Joyce, and Peter Levell. 2020. "Getting people back into work."
Eurofound. 2020. "Living, working and COVID-19: first findings, April 2020."

Gottlieb, Charles, Ian Grobovsek, and Markus Poschke, 2020, "Working From Home across Countries." 15 April mimeo.

Jones, Callum J., Philippon, Thomas, Venkateswaran, Venky, 2020. Optimal Mitigation Policies in a Pandemic: Social Distancing and Working from Home. National Bureau of Economic Research working paper 26984.

Kaplan, Greg, Benjamin Moll, and Gianluca Violante. 2020. "Pandemics according to HANK." May 4 slidedeck.

Koren, Miklós, Petö, Rita, 2020. Business disruptions from social distancing. Covid Economics: Vetted and Real-Time Papers 1 (2), 13-31.

Mas, Alexandre, Pallais, Amanda, 2020. Alternative Work Arrangements. Annual Review of Economics, Annual Reviews,

Mongey, Simon, Pilossoph, Laura, Weinberg, Alex, 2020. Which Workers Bear the Burden of Social Distancing Policies? Becker Friedman Institute white paper

Oettinger, Gerald S., 2011. The incidence and wage consequences of home-based work in the United States, 1980-2000, J. Hum, Resour, 46 (2), 237-260,

Rampini, Adriano A., 2020. Sequential Lifting of covid-19 Interventions with Population Heterogeneity. National Bureau of Economic Research working paper 27063.

Saltiel, Fernando, 2020. "Who Can Work From Home in Developing Countries?" 6 April Mimeo.

Stratton, James, 2020. How Many Australians Can Work From Home? An Application of Dingel and Neiman (2020) to Australian Occupation Data.

United Kingdom Office for National Statistics. 2020. "Coronavirus and homeworking in the UK labour market: 2019."