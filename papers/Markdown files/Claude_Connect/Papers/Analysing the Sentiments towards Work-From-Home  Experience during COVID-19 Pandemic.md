HANDLE: https://hdl.handle.net/10216/126987

DOI: https://doi.org/10.24840/2183-0606\_008.001\_0003

# Analysing the Sentiments towards Work-From-Home Experience during COVID-19 Pandemic

#### Akash D Dubey

drakashddubey@gmail.com | Jaipuria Institute of Management, Jaipur, Rajasthan, India Shreya Tripathi

shreyatripathi13@gmail.com | Amity University, India

# Letter from Academia

Abstract. With almost one third of the world on a lockdown, the corporates and the offices have now rapidly shifted to working from home. Since no specific treatment has been suggested by any medical institution so far, World Health Organization has recommended that the only possible solution to be safe is to self-isolate and stay home. Due to this, the world has come to a screeching halt and the businesses have to be shifted to remote work. Work-from-Home is a very new experience for most of us and hence the perception of the people ranges from being very excited to very hopeless. This study aims to examine the sentiments of the people regarding Work-from-Home concept by analysing twitter activities posted on social media. Total 100,000 tweets were analysed for this study. Results indicate that Work-from-Home concept was taken positively by the people. The emotions associated with most of the tweets were of trust and anticipation indicating that this concept is being welcomed by the people.

Keywords. Work From Home (WFH);COVID-19; Pandemic; Remote Working; Twitter; Sentiment Analysis.

Cite paper as: Dubey, A., Tripathi, S., (2020). Analysing the Sentiments towards Work-From-Home Experience during COVID-19 Pandemic - Letter from Academia, Journal of Innovation Management, www.open-jim.org, 8(1), 13-19.

# 1 Introduction

Sars-CoV-2 or 2019-nCoV was firstly detected in the city of Wuhan, China in December 2019 (Chaolin et al, 2020) and since then this disease has been spreading exponentially. While there were 86,604 patients of COVID-19 on 28th February and 858,361 on 31st March, the number has increased to 2,086,477 on 15th April 2020. COVID-19 has affected 210 countries and 2 international conveyance till now.

As suggested by World Health Organization, in the absence of any specific treatment, one of the ways to stop the spread of COVID-19 is self-quarantine and isolation. This procedure was followed by China in the city of Wuhan and 15 other provinces with positive results.

As per the recommendation of WHO, many countries have opted for complete lockdown of the country. India, France, Italy, New Zealand, Poland and UK opted for one of the largest and restrictive lockdowns that world has witnessed. India, a home to 1.3 billion people locked down the country on 25th April 2020 for three weeks which was later extended till 3rd May 2020. Similarly, one of the worst hit country, Italy, has decided to extend the lockdown till 13th May 2020. On the contrary, the worst hit country till now, USA has gone against the complete lockdown.

Since the lockdown has made people stay at home, most of the businesses have been trying to go for Work-from-Home (WFH) concept. To implement WFH concept, several technical platforms are being used to make sure that the efficiency of the employees remain intact. Several IT companies, academic institutions and other industries have gone completely online and the employees are now expected to work-from-home with a different set of rules and regulations that would suit the organizations.

In these changing times, the employees have to shift their modus operandi completely and that may be a reason of concern considering their perception and eagerness to adapt to the situation. To evaluate the sentiments of Work-from-Home concept among the people worldwide, we have collected 100,000 tweets across the world which ranges between 15th March and 15th April 2020. Twitter has been one of the most important social platforms when it comes to information dissemination and self-documentation (Liu, Cheung, Lee, 2010). It has been a medium for millions to express their views on any issues or topics. During previous events of natural disasters, people have used this platform for expressing their feelings (Soriano et al, 2016; Lent et al, 2017; Nair et al, 2017; Fu et al, 2016).

# 2 Methodology

With a total number of 330 million daily active users, Twitter has found a huge following throughout the world. For this research, we have used the Twitter API for the collection of the tweets over a regular interval of time. In total, we have collected 100,000 tweets worldwide. These tweets either contained the term #WorkFromHome or #WFH.

For the collection of the tweets, RTweet package was used in R. To avoid the duplication of the tweets, retweets were not included in the collection. After the collection of the tweets, the data cleaning was done. During the data cleaning, the white spaces, punctuations and stop words were removed, while covering the whole tweet to lower case. After the data cleaning, NRC Emotion Lexicon (Mohammad SM, Turney PD, 2013) was used for the sentiment analysis to analyse the tweets. For this analysis, Syuzhet package version 1.0.1 (Jockers M, 2017) was used in R. The Syuzhet package classifies the tweets on the basis of sentiments (positive and negative) and also categorizes them into 8 emotions (fear, joy, anticipation, anger, disgust, sadness, surprise, trust). After the scoring process was over, the word cloud was created to analyse the most tweeted words in relation to work-from-home.

# 3 Results and Discussion

![](_page_2_Figure_4.jpeg)

Fig. 1. Sentiment Analysis of Tweets for Work from Home

From the analysis of the sentiments regarding Work-from-Home, it was found that 73.10 % of the tweets had positive sentiments as compared to 26.10% negative sentiments. This signifies that the people had a positive outlook towards the concept of work-from-home. For a more detailed analysis of the tweets, the emotion quotient associated with tweets were analysed. There were total 8 emotions which were evaluated in this analysis which included fear, joy, anticipation, anger, disgust, sadness, surprise and trust.

During the analysis of the emotional quotient of the tweets, it was found that the majority of the tweets across the globe were done with three emotions, Trust, Anticipation and Joy. Figure 1 shows that the tweets with trust emotion were almost one fourth of the total tweets analysed (24.03%). Following the trust emotion was the anticipation emotion which signified that people were looking forward to experiencing Work-from-Home concept. Similarly, the joy emotion was associated with almost 16.45% of the tweets which again strengthens the positive sentiments of the people. Emotions like fear, sadness, anger and disgust had relatively smaller portion of tweets with a share of 10.17%, 8.60%, 6.69% and 4.32% respectively. These results prove that the people had a positive outlook and were looking forward to work-from-home.

For the second phase of analysis, a word cloud was created using the most used words and the emotions that were associated with them. It was found that the word GOOD was tweeted most in context of WFH. As illustrated in figure 2, words GOOD, BREAK and HOPE were used most of the times and related with emotion of surprise. Words like LOVE, SHARE, HAPPY, SAFE and HOME were tweeted frequently with the emotion of joy. Words like TEAM, MANAGE, REMOTEWORK were tweeted frequently with emotions of trust. Words like TIME and START were frequently tweeted with the emotion of anticipation. People also tweeted words like FEEL, BAD and ILL with the emotion of disgust while words like PANDEMIC, ISOLATE and LATE were regularly used with emotions of sadness.

These results signify that majority of the people have a positive outlook towards the work-from-

![](_page_3_Figure_5.jpeg)

Fig. 2. Word Cloud of the Tweets related to Work from Home

home experience. These results become more important especially when a report from Gartner stated that 74% CFOs and Finance leaders are willing to shift least 5% of on-site employees to remote work permanently (Lavelle, 2020).

# 4 Summary

This research work aimed at analysing the sentiments and emotions of the people towards workfrom-home concept during COVID-19. During the study, it was revealed that more than 73% people had a positive sentiment towards work-from-home while almost 27% people had a negative perception towards WFH experience. Also, more than 60% of the people tweeted with emotions of trust, anticipation and joy for work-from-home culture while a few tweeted with fear, sadness, anger and disgust. From the obtained results, it can be concluded the work-from-home experience had a positive perception worldwide. Since the tweets collected were in English, it might be a limitation of the study.

For future works, this study can be used to analyse the changing emotions and sentiments of people and check whether there are major shifts in them over a period of time.

# 5 References

Coronavirus Update. Accessed 20th April 2020. [https://www.worldometers.info/coronavirus/.](https://www.worldometers.info/coronavirus/)

Fu, K. W., Liang, H., Saroha, N., Tse, Z. T. H., Ip, P., & Fung, I. C. H. (2016). How people react to Zika virus outbreaks on Twitter? A computational content analysis. American journal of infection control, 44(12), 1700-1702.

Huang, C., Wang, Y., Li, X., Ren, L., Zhao, J., Hu, Y., & Cheng, Z. (2020). Clinical features of patients infected with 2019 novel coronavirus in Wuhan, China. The Lancet, 395(10223), 497-506.

Jockers, M. (2017). Introduction to the Syuzhet package. Accessed 15th April 2020. [https:](https://cran.r-project.org/web/packages/syuzhet/vignettes/syuzhet-vignette.html) [//cran.r-project.org/web/packages/syuzhet/vignettes/syuzhet-vignette.html](https://cran.r-project.org/web/packages/syuzhet/vignettes/syuzhet-vignette.html)

Lavelle, J., (2020) CFO Survey Reveals 74% Intend to Shift Some Employees to Remote Work Permanently. Gartner. Accessed 20th April 2020. [https://www.gartner.com/en/newsroom/](https://www.gartner.com/en/newsroom/press-releases/2020-04-03-gartner-cfo-surey-reveals-74-percent-of-organizations-to-shift-some-employees-to-remote-work-permanently2) [press-releases/2020-04-03-gartner-cfo-surey-reveals-74-percent-of-organizations-to-shift-some-employees-to-remote-work-permanently2](https://www.gartner.com/en/newsroom/press-releases/2020-04-03-gartner-cfo-surey-reveals-74-percent-of-organizations-to-shift-some-employees-to-remote-work-permanently2)

Liu, I. L., Cheung, C. M., & Lee, M. K. (2010). Understanding Twitter Usage: What Drive People Continue to Tweet. Pacis, 92, 928-939.

Mohammad, S. M., & Turney, P. D. (2013). Crowdsourcing a word–emotion association lexicon. Computational Intelligence, 29(3), 436-465.

Mohammad, S. M., & Turney, P. D. (2013). Nrc emotion lexicon. National Research Council, Canada.

Nair, M. R., Ramya, G. R., & Sivakumar, P. B. (2017). Usage and analysis of Twitter during 2015 Chennai flood towards disaster management. Procedia computer science, 115, 350-358.

Soriano, C. R., Roldan, M. D. G., Cheng, C., & Oco, N. (2016). Social media and civic engagement during calamities: the case of Twitter use during typhoon Yolanda. Philippine Political Science Journal, 37(1), 6-25.

Van Lent, L. G., Sungur, H., Kunneman, F. A., Van De Velde, B., & Das, E. (2017). Too far to care? Measuring public attention and fear for Ebola using Twitter. Journal of medical Internet research, 19(6), e193.

# Biographies

![](_page_6_Picture_3.jpeg)

Akash D Dubey. Dr Akash D Dubey has completed his PhD from Indian Institute of Technology, BHU, India in Artificial Intelligence and Robotics. He is currently working as an Assistant Professor at Jaipuria Institute of Management, Jaipur, Rajasthan, India. Prior to Jaipuria, he has worked as Assistant Professor at Fiji National University in Fiji for four years. He has written several reputed international research articles and international conferences. Dr. Dubey has conducted many workshops and seminars in Fiji and India. His research interest area includes Artificial Intelligence, ICT in education, Social Media and Computational Intelligence.

![](_page_6_Picture_5.jpeg)

Shreya Tripathi. Ms Shreya Tripathi is currently pursuing Master in Business Administration from Amity University, India. Her specialization for MBA is Human Resources. Ms Tripathi has completed her Bachelor in Commerce from Allahabad University, Allahabad, India. Her research area includes Talent Acquisition, Training and Development, Business Law, Entrepreneurship, Economics, Commercial Studies and Performance appraisals.