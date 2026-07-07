# Construction of the Virtual Embodiment Questionnaire (VEQ)

Daniel Roth *Member, IEEE* Marc Erich Latoschik *Member, IEEE*

![](_page_0_Picture_5.jpeg)

![](_page_0_Picture_6.jpeg)

![](_page_0_Picture_7.jpeg)

Fig. 1. **Factors addressed by the VEQ.** Virtual *body ownership* (a) which refers to the perception of perceiving a virtual body as the own, as the source of all sensations; *Agency* (b), which refers to the perception of control over a virtual body, and through that, control over events in the environment; *Change* (c) which refers to the change in the perceived body schema due to the stimulation. The user is depicted in grey; the virtual avatar is depicted in orange.

**Abstract**—User embodiment is important for many virtual reality (VR) applications, for example, in the context of social interaction, therapy, training, or entertainment. However, there is no data-driven and validated instrument to empirically measure the perceptual aspects of embodiment, necessary to reliably evaluate this important phenomenon. To provide a method to assess components of virtual embodiment in a reliable and consistent fashion, we constructed a Virtual Embodiment Questionnaire (VEQ). We reviewed previous literature to identify applicable constructs and questionnaire items, and performed a confirmatory factor analysis (CFA) on the data from three experiments (*N* = 196). The analysis confirmed three factors: (1) ownership of a virtual body, (2) agency over a virtual body, and (3) the perceived change in the body schema. A fourth study (*N* = 22) was conducted to confirm the reliability and validity of the scale, by investigating the impacts of latency and latency jitter present in the simulation. We present the proposed scale and study results and discuss resulting implications.

**Index Terms**—Virtual Embodiment, Body Ownership, Agency, Avatars, Virtual Reality

# **1 INTRODUCTION**

User embodiment can be referred to as "the provision of users with appropriate body images so as to represent them to others (and also to themselves)" [9, p.242]. It became apparent that the relevance of virtual embodiment is not limited to the understanding of cognitive processes. Instead, understanding virtual embodiment has concrete and direct implications for research, design, and development. It is especially relevant for applications that consider therapy [2, 19, 57, 59, 65, 66], entertainment and recreation [41, 51, 63], as well as collaboration and social interaction [8, 44, 45, 73]. Previous research investigated virtual embodiment in various studies, developed individual questions, and proposed questionnaire item collections. However, a consistent and validated instrument for assessing components of virtual embodiment that is based on data driven component analysis, to the best of our knowledge, does not exist.

Previous assessments adapted measures from originating experiments such as the rubber hand illusion (RHI) [13], for example, individual questionnaires and displacement measures. However, the assessment of concepts such as virtual body ownership (VBO) is not consistent, and therefore, the overall comparability of effects is limited. Effects are often assessed with single items, which was argued to be problematic [17]. The reliability of assessments is often not

- *Daniel Roth (corresponding author) is with the Technical University of Munich. e-mail: daniel.roth@tum.de*
- *Marc Erich Latoschik is with the University of Wurzburg. e-mail: ¨ marc.latoschik@uni-wuerzburg.de*

*Manuscript received 18 May 2020; revised 26 July 2020; accepted 17 Aug. 2020. Date of publication 17 Sept. 2020; date of current version 3 Nov. 2020. Digital Object Identifier no. 10.1109/TVCG.2020.3023603*

reported, and approaches to cross-validating different measures often failed (see [39, 72] for discussions). According to Boateng et al. [12], the creation of a rigorous scale undergoes three stages: 1) In the *item development stage*, the domain is identified, and items are theoretically analyzed regarding their content validity. 2) In the *scale development* stage, questions are pre-tested, and hypothesized factors are explored with covariance analysis (e.g., exploratory factor analysis), along with a consecutive reduction of items to an item pool that remains internally consistent, followed by the factor extraction. 3) In the *scale evaluation* phase, the dimensionality is tested with CFA, and consecutively, the reliability (e.g., Cronbach's alpha [18]) and validity (i.e., precision and relation to other constructs and measurements) are evaluated. According to Kline [42], it is necessary to strive for both, internal consistency (presuming some closeness in the item context) and validity (presuming the item set fully covers the underlying construct) are of importance in scale construction. To that regard, he further argues, that despite the dangers of boosting the reliability of a test by using items that are of high similarity, the coefficient alphas should not drop below .7.

Roth et al. point out the importance of instrument standardization and perform an exploratory factor analysis on items previously used in published research [72]. Gonzalez-Franco and Peck also emphasized the request for a standardized questionnaire and review assessments from previous studies [28]. From those, they identify questions to be standardized for embodiment research [28, p. 4] which they organized in six experimental interests (body ownership, agency and motor control, tactile sensations, location of the body, external appearance, and response to external stimuli). According to the literature on scale construction, a scale should be *reliable* (produce repeatable results within and across subjects irrespective of the testing conditions), *valid* (measure the underlying constructs precisely), *sensitive* (discriminate between multiple outcome levels), and *objective* (shielded from third-party variable bias) [55, 91].

Progressing beyond a theoretical approach [28] and exploratory analysis [72], we propose a scale that is data driven, that proceeded all scale development stages (see [12, 23]). Validated instruments foster the replicability of studies in general. Hence, the development of scales is critical to empirical research. In contrast, mere collections of items, that are not confirmed to measure an underlying construct, may bias results and interpretations.

We present the development and initial validation of a questionnaire for assessing three components of virtual embodiment (ownership, agency, and change in perceived body scheme). These components were explored, confirmed, and validated in an initial validation study. We investigated the scale performance by exploring it's relation to related concepts and previous measures applied, and confirm its validity, reliability, and sensitivity. We further provide insights into the impacts of latency and latency jitter that were investigated in the validation study. The resulting questionnaire can be applied to various VR experiments to assess virtual embodiment.

In the following Sect. 2 we review related work and describe previously investigated aspects of embodiment and virtual embodiment. We then describe the scale development, namely the item construction (Sect. 3) and the study methods for the data basis Sect. 4, as well as the results of the CFA Sect. 5 and the relation to related constructs, assessed by correlations Sect. 6. Finally we further present an initial validation study and its results (Sect. 7), before we provide a general discussion in Sect. 8 and our conclusion Sect. 9.

# **2 BACKGROUND AND RELATED WORK**

# **2.1 Embodiment**

Embodiment is a part of self-consciousness and arises through multisensory information processing [25, 48, 50]. Previous literature mainly considered three components of embodiment: A conscious experience of self-identification (body ownership), controlling one's own body movements (agency) [83], and being located at the position of one's body in an environment (self-location) [47, 50]. Research also stresses the importance of the perspective with which one perceives the world with (first-person perspective) [10, 11].

Self-Location may be described as "the experience that the self is localized at the position of our body at a certain position in space" [50, p. 150] following [48]. It should not be confused with the concept of presence, or 'being there' [31], it is rather researched in the context of disrupted body perception, such as out-of-body experiences, or autoscopic hallucinations ( [15, 50]).

Body ownership can be described as the experience and allocation of a bodily self as one's own body, as "my body," the particular perception of one's own body as the source of bodily sensations, unique to oneself so that it is present in one's mental life [24, 82, 83]. A key instrument in investigations of body ownership is the RHI [13]. The experiment stimulates ownership of an artificial body part in the form of a rubber hand by simultaneous tactile stimulation (visually hidden) of the physical hand combined with a parallel visual stimulation of a rubber hand. Caused by the stimulation, participants start to perceive the rubber hand as part of their body.

Agency, meaning the "experience of oneself as the agent of one's own actions - and not of others' actions" ( [20, p. 523,] following [24]) relates to body ownership [15, 83, 84]. Tsakiris et al. described agency as "the sense of intending and executing actions, including the feeling of controlling one's own body movements, and, through them, events in the external environment" [83, p. 424].

Previous work showed that bottom-up accounts (multisensory processing and integration) are an important driver [40, 82], and that topdown processes (e.g., form and appearance matching) at least modulate embodiment [15, 29, 83, 84]. Kilteni et al. [40] reviewed triggers and preventers of body ownership illusions and summarized that crossmodal stimulation, for example, congruent visuomotor and visuotactile stimulation supported ownership illusions. In contrast, incongruencies (thus counter-acting sensorimotor contingencies) hinder ownership. Further, visuoprorioceptive cues, such as perspective shifts or modified distances, as well as semantic modulations can impact ownership illusions [40].

![](_page_1_Picture_12.jpeg)

![](_page_1_Picture_13.jpeg)

![](_page_1_Picture_14.jpeg)

Fig. 2. **Three components of embodiment in the physical world that were identified in the literature: self-location, body ownership, and agency.** Self-location (a) refers to the experience of the self being located at the position of our body [50]. Ownership (b) relates to perceiving the body as the own, as the source of sensations. Agency (c) relates to the feeling of control over one's own actions [83].

# **2.2 Virtual Embodiment**

Virtual embodiment has received ongoing attention in VR research, for example, regarding avatar hand appearance [3, 33, 37] and full body representations [54, 56, 60, 78, 86]. Avatars that represent a user are defined as virtual characters driven by human behavior [6]. Following video-based approaches [48], researchers found that the concept of the RHI also applies to virtual body parts [76], and entire virtual bodies [52, 77, 78].

To investigate and alternate virtual body perception, experimentation has used mirrors in immersive HMD-based simulations [27], and semiimmersive fake (magic) mirror projections [46, 86]. According to Slater et al. [77], the induction time for body ownership illusions varies between about 10 s and 30 min. Kilteni et al. [39] summarized findings and measures regarding self-location, agency, and body ownership, and argue for a continuous measurement approach. Similar to Kilteni et al. [40], Maselli and Slater concluded from their experiments that bottomup factors, like sensorimotor coherence, and a first-person perspective, are driving factors [54]. They argue that appearance moderates the experience insofar as realistic humanoid textures foster body ownership.

With regard to the impacts of user embodiment, it was argued that a self-representation that is of of similar appearance and shows accurate response to the user's movement (e.g., of body, face, and eye motion) foster the perception of presence [75, 85]. Different levels of behavioral realism and accurate motion reconstruction, for example by the fidelity of tracking [67, 70], as well as natural or artificially introduced behaviors [22,69] may therefore also influence the perception of embodiment as such.

An second effect to mention regarding the embodiment through avatars in VR is the Proteus effect [92, 93]. Yee and Bailenson found a change in behavior, self-perception and participants' identity when taking the perspective of an avatar with altered appearance. Participants changed their behavior and attitude according to behavior they attributed to their virtual representation.

In summary, the degree and the precision with which sensory stimulation, appearance, and behavior are rendered, and the presented perspective seem to affect perceptual responses [27, 40, 52, 54, 86, 87]. Design choices, for example, the character type, or the realism of appearance and behavior may thus strongly influence the user perception. In turn, measuring embodiment in a valid way is crucial to draw comparable conclusions for designing embodiment applications.

### **3 SCALE CONSTRUCTION**

Previous assessments often base on the original RHI experiment [13]. A psychometric approach to assessing levels of embodiment toward an artificial physical body part identified the latent variables of ownership, agency, and location [49]. The assessment of location included items focusing on the coherence between sensation and causation, and locational similarities of artificial physical body parts.

![](_page_2_Picture_2.jpeg)

![](_page_2_Picture_3.jpeg)

![](_page_2_Picture_4.jpeg)

Fig. 3. **Apparatus (Study 1).** *Left:* The projection condition. *Center:* The HMD condition. *Right:* The female and male avatars used for Study 1.

Table 1. Proposed items for the generalization and extension.

# *Ownership*

- It felt like the virtual body was my body.
- It felt like the virtual body parts were my body parts.
- The virtual body felt like a human body.
- I felt like the virtual body belonged to someone else.\*†
- It felt like the virtual body belonged to me.†

#### *Agency*

- The movements of the virtual body felt like they were my movements.
- I enjoyed controlling the virtual body.
- I felt like I was controlling the movements of the virtual body.
- I felt like I was causing the movements of the virtual body.
- The movements of the virtual body were in sync with my own movements.†

# *Change (in the perceived body schema)*

- I had the illusion of owning a different body to my own (body).
- I felt like the form or appearance of my own body had changed.
- I felt like I had to check that my own body still looked like I remembered.
- I felt like the weight of my own body had changed.
- I felt like the size (height) of my own body had changed.
- I felt like the width of my own body had changed.

*Note. \* Required recoding,* † *new item.*

Roth et al. [72] presented a proposal to assess virtual embodiment with 13 questions from previous work [4, 13, 21, 27, 38, 49, 52, 58, 61, 78, 80]. A principal component analysis revealed three factors: acceptance (covering the aspect of ownership perception), control (covering the aspect of agency perception), and change (covering the aspect of a perceived change in one's own body schema). The last factor may be especially important for studies that make use of altered body appearances and the Proteus effect [7, 72, 92, 93], such as studies related to therapeutic applications [57, 66]. The instrument showed good reliability in further assessments [45, 86].

In addition to a necessary validation and consistency analysis, two downsides can be identified: 1) The measure is strongly constrained to a "virtual mirror" phrasing which may hinder a standardized application of a questionnaire to different study types and experimental paradigms 2) the components are not balanced regarding the number of items. In particular, the ownership component consists of only three statements, which may reduce the overall assessment quality. We based our scale development on their work and performed necessary improvements.

Regarding the item development, we first generalized the phrasing of the questions to fit generic scenarios and removed the "virtual mirror" reference. Second, we introduced additional items to the item pool in order to examine whether these are of benefit regarding the questionnaire quality, see Table 1. We added questions for *ownership* ("It felt like the virtual body belonged to another person," - adapted from [58], "It felt like the virtual body belonged to me") and *agency* factors ("The movements of the virtual body were in sync with my own movements"), respectively. The items are shown in Table 1.

For the *scale development* a CFA was calculated with the data from three studies (*N* = 196) that assessed the impacts of particular manipulations. Since our paper focuses on the scale construction, the following section describes the general basis of the data collection.

# **4 DATA ACQUISITION**

In the following we report the descriptions of each study that was used for the initial data collection in order to perform the CFA. In each study, we manipulated simulation properties that we suggested to affect the perceived embodiment based on previous works [39, 40, 46, 54, 86], namely, immersion (Study 1), personalization (Study 2), behavior realism (Study 3). In addition to the virtual embodiment questionnaire items proposed for the generalization and extension (see Table 1), we assessed related concepts, which are described in the measures sections of the following descriptions, in order to investigate correlations to the proposed instrument, and to compared the scale performance to related instruments. Participants were individually recruited (i.e., the studies were not performed in block testing fashion) through the recruitment system of the [institution]. All studies were approved by the ethics committee of the [institution].

For the remainder of this section, we will first describe the methods and procedures for all studies in detail, before we present the CFA analysis procedure and results in Sect. 5, as well as the correlations to investigated constructs in Sect. 6.

## **4.1 Study 1: Level of Immersion**

# 4.1.1 Method

In a one-factor (*Medium*) between-subjects design modifying the level of immersion, participants were exposed to either a fake-mirror projection, in which case the participant had a visual reference to her or his physical body, or an immersive simulation displayed with an HMD, in which case the participant saw her or his virtual body from a first-person perspective (Fig. 3). To provoke the perception of virtual embodiment, participants were asked to perform motions and focus their attention, similar to related experiments [46, 86], as described in the following.

Procedure Fig. 5 shows the study procedure. Participants were welcomed and informed, before the pre-study questionnaire with demographics and media usage was assessed. Participants were equipped, calibrated, and given time to about 1 minute time to acclimatize to the simulation. Similar to previous work [46, 86], audio instructions were then presented to the users to induce embodiment with a total duration of 150 s. In these instructions, users were asked to perform actions, meaning to move certain body parts (e.g. "Hold your left arm straight out with your palm facing down."), and further focus on one's own/the avatar body parts, as well as the body parts of their avatar presented in a virtual mirror. ("Look at your left hand." [Pause] "Look at the same hand in the reflection"), followed by a relaxing pose ("Put your arm comfortably back down and look at your reflection"). Following the exposition, the dependent measures were assessed.

Apparatus The scenarios and materials are depicted in Fig. 3. Participants were tracked by an OptiTrack Flex 3 tracking system. A Unity3D simulation displayed the stimulus via a fake mirror projection

![](_page_3_Picture_2.jpeg)

Fig. 4. **Apparatus.** *Left:* Generic characters (Study 2, 3, and Validation Study). *Center:* Character generator. *Right:* Personalization (Study 2).

![](_page_3_Figure_4.jpeg)

Fig. 5. General Study procedure.

or an Oculus Rift CV1 HMD (2160 px × 1200 px, 90 Hz, 120 degrees diagonal field of view). For the projection, the image was rendered using a fish tank VR [89] approach with off-axis stereoscopic projection [14], and displayed by an Acer H6517ST projector (projection size: sized 1.31 m high × 1.46 m width, active stero, 480 px × 1080 px per eye). The virtual projection was calibrated to match the physical projection preferences, thus allowing a physically accurate mirror image. The virtual camera/tracking point was constrained to the avatar head joint while accounting for the distances of the eyes (head-neck model). The baseline motion-to-photon latency was approximated by video measurement and frame counting ( [30, 87]) to 77 ms for the projection setup, assuming slightly lower values for the HMD setup. In the virtual environment, the participant was placed in a living room. A reference point was presented, as well as a virtual mirror (in the projection condition, the projection was the mirror; see Fig. 3). We used avatars created with Autodesk Character Generator (Fig. 3) which were scaled (uniform) according to the participant's height.

Measures We assessed the proposed virtual embodiment questions (see Table 1) and the igroup presence questionnaire (IPQ) [74], which was adapted to fit the presented scenario. The IPQ adaptation

assessed *general presence* ("In the computer-generated world, I had a sense of 'being there"'), *spatial presence* (e.g., " I did not feel present in the virtual space"; α = .786), *involvement* (e.g., "I was not aware of my real environment"; α = .851), and *realness* (e.g., "How real did the virtual world seem to you?"; α = .672). The responses were given using a 7-point Likert-type scale (see the original source for the anchors). Further assessments are not the subject of the present reporting due to page limitations. No severe sickness effects occurred.

Participants We excluded participants when problems or severe tracking errors were noted. The final sample consisted of 50 participants (32 female, 18 male, *Mage* = 22.18, *SDage* = 2.83). Of those, 49 participants were students, and 46 participants had previous experience with VR technologies. The sample was equally distributed (25 per condition).

# **4.2 Study 2: (User-Performed) Personalization**

# 4.2.1 Method

In a one-factor (*Personalization*) between-subjects design, we compared the embodiment with an avatar from a creation tool to a personalized avatar created with the same tool. Participants were represented either as a gender-matched generic avatar (Caucasian–as we expected a Caucasian sample) or by a personalized avatar they created as a representation of themselves (see Fig. 4).

Procedure The procedure followed the general format (Fig. 5). Participants were welcomed and informed, before the pre-study questionnaire was assessed. Participants were then asked to create an avatar (personalized condition) or to inspect the generic avatar (generic avatar condition). In the personalized condition, participants were taught the avatar generator software and provided help. Participants were permitted to modify the virtual character's body measures (form, proportions), facial appearance, and hairstyle in 15 min of preparation time. The clothing was kept similar in the two conditions. Following the avatar creation/inspection, a similarity measure was assessed. Participants were then calibrated and had about 1 minute time to acclimatize to the simulation. Similar to Study 1, audio instructions asking participants to perform movements and focus on body parts were used for the embodiment exposition. In addition to the instructions for Study 1, the participants were specifically instructed to step closer to the mirror and pay attention to features of the character's appearance (e.g., "Look at the eyes of the mirrored self," "Look at the mouth of the mirrored self," "Turn 90 degrees and look at the mirrored self from the side"). The instructions lasted for 180 s.

Apparatus The apparatus consisted of a setup identical to the HMD-based setup of Study 1, except that a FOVE 0 HMD (2560 px × 1440 px, 70 Hz, 100 degrees field of view) was used as the display.

Measures We measured demographic variables, the virtual embodiment items (see Table 1), and affect using the PANAS scale in the short form [81] (PA: α = .840; NA α = .319, dropped from analyses). As we expected that personalization may also have an impact on self-presence, we assessed Ratan and Hasler's self-presence questionnaire [62], adapted to the context of the study (excluded: "To what extent does your avatar's profile info represent some aspect of your personal identity?" and "To what extent does your avatar's name represent some aspect of your personal identity?"). Proto–self-presence

 $(\alpha=.781)$  was assessed with items such as "How much do you feel like your avatar is an extension of your body within the virtual environment?" Core self-presence  $(\alpha=.838)$  was assessed with items such as "When arousing events would happen to your avatar, to what extent do you feel aroused?" Extended self-presence  $(\alpha=.661)$  was assessed with items like "To what extent is your avatar's gender related to some aspect of your personal identity?" (5-point scale, see [62]). To control for the manipulation, we measured the perceived similarity toward the avatar (generic or personalized) before the exposure (desktop monitor), and after the exposure (reflecting the experience): "Please rate how much the virtual character is similar to you on the following scale, where 1 equals no similarity and 11 equals a digital twin." Further measures such as sickness and humanness are not part of the present discussion. No severe sickness effects occurred.

Participants We excluded participants when problems or severe tracking errors were noted. The final sample consisted of 48 participants (generic avatar: N=25, personalized avatar: N=23. 27 female, 21 male,  $M_{age}=21.64$ ,  $SD_{age}=2.25$ ). All participants were students, and 45 participants had previous experience with VR.

# 4.3 Study 3: Behavioral Realism

#### 4.3.1 Method

In a two-factor (*Facial Expressions*, Gaze) between-subjects design, we evaluated the impact of behavioral realism. Participants were represented by generic avatars (see Fig. 4, top) and randomly assigned to one of four conditions: body motion only (BO), body and facial motion replication (BF), body and gaze motion replication (BG), and body, gaze, and face motion replication (BFG).

Procedure The procedure followed the general format (Fig. 5). Participants were welcomed and informed, before we assessed the prestudy questionnaire. Participants were then calibrated and had about 1 minute time to acclimatize to the simulation. Audio instructions then asked participants to perform bodily movements and focus on body parts. In Study 3, the participants were specifically instructed to move closer to another marking in front of the mirror, and let their gaze wander to specific focus points, trying to ensure an influence in perception of the manipulation (e.g., "Fixate on the left eye of your mirrored-self," "Focus on the right ear of your mirrored self" etc.). For the facial expressions, we asked participants to perform certain expressions (e.g., "Open and close your mouth," "Try to express happiness by smiling at your mirrored-self," etc.). The instructions lasted for 219 s. After the exposure, we assessed the dependent measures.

Apparatus We used the same apparatus and generic avatars as in Study 2, and included the tracking of the participant's gaze using the FOVE 0's eye tracking system as well as facial expression tracking performed by a BinaryVR Dev Kit V1. Combining the two individual eye vectors, the FOVE integration calculates the intersection point to estimate the convergence point in the virtual scene, which is the approximate focus point of the user [90]. From this position, we recalculated the eyeball rotation. The BinaryVR Dev Kit was used

![](_page_4_Figure_9.jpeg)

Fig. 6. **Sensing and replication (Study 3).** *a)* Tracking. *b)* Sensory data (exemple images). *c* Replication. *d* Gaze detail example. The figure depicts an independent avatar not related to the studies. The avatars that were used in the study are depicted in Fig. 4.

to gather information about lower facial deformation. The 3D depthsensing device Pico Flexx (up to 45 Hz) was affixed to the HMDs. Its 2D and depth images were processed by the BinaryVR Dev Kit to generate facial deformation parameters [36,95]. Tracked expression parameters were mapped to blendshapes, for example, jaw open, and smile. The body tracking, facial expression, and gaze data was fused in the simulation to drive the avatar (see Fig. 6).

Measures We assessed the proposed virtual embodiment questions, a rating of the avatar assessing humanness, eeriness, and attractiveness ( $\alpha$ s  $\geq$  .688) [32], the self-presence measures previously applied in Study 2 ( $\alpha$ s  $\geq$  .645) [62], as well as affect ( $\alpha$ s  $\geq$  .674) [34,81]. We further asked how real, how natural, and how synchronous the motion behavior of the avatar appeared to the participants: "The movements were realistic," "The movements were in synchrony to my own movements" (1–strongly disagree, 7–strongly agree). Further measures were excluded due to page limitations. No severe sickness effects occurred.

Participants We excluded participants when problems or severe tracking errors were noted. The final sample for the analysis consisted of 70 participants (46 female, 24 male,  $M_{age} = 21.3$ ,  $SD_{age} = 1.82$ , all students), of whom 65 had previous VR experience. 17 participants were assigned to the BO condition, 18 to BF, 18 to BG, and 17 to BFG.

#### 5 CONFIRMATORY FACTOR ANALYSIS

The above described data collection resulted in N = 196 valid samples of the assessment of the proposed scale items (see Table 1). We performed the CFAs using R (lavaan package). The reporting of fit indices is based on the recommendation made by Kline [43]. As the assumption of multivariate normality was violated, we conducted a robust maximum likelihood estimation and computed Satorra-Bentler (SB) corrected test statistics (see [16]). The first attempt did not yield an acceptable model fit, and as the modification indices indicated, there were covariations in the error terms of a particular item loading on several factors ("I had the illusion of owning a different body from my own"). Therefore, this item was dropped. A second attempt yielded an acceptable model fit. However, inspection of the modification indices revealed covariations in the error terms of two items loading on several factors ("I had the feeling that the virtual body belonged to another person," "I enjoyed controlling the virtual body"). Thus, we excluded problematic items. Furthermore, items with a factor loading < .40 were excluded ("I felt the need to check if my body really still looked like what I had in mind"). The third CFA with the remaining 16 items yielded a more parsimonious solution with a good model fit, SB  $\chi^2 = 52.50$ , df = 51, p = .416, root mean square error of approximation AC (RMSEA) = .013, 90% confidence interval of robust root mean square error of approximation [.000; .052], standardized root mean square residual (SRMR) = .047, and a robust comparative fit index (CFI) = .998. Thus, the solution was deemed acceptable to characterize these components of virtual embodiment. Table 2 depicts the standardized coefficients. The reliability values assessed by Cronbach's Alpha for ownership ( $\alpha = .783$ ), agency ( $\alpha = .764$ ), and change  $(\alpha = .765)$  were acceptable. Considering the individual studies, the scale also performed acceptable in Study 1 ( $\alpha \ge .751$ ), Study 2 ( $\alpha$  $\geq$ .744), and Study 3 ( $\alpha \geq$ .732). The resulting scale is depicted in Table 3, its factors are illustrated in Fig 1. The scale was assessed in german. A professional service was consulted for the translation.

# 6 CORRELATIONS TO RELATED CONSTRUCTS

To assess the relation to related constructs, and thus to provide insights into the construct validity [64, see chapter 8.5 for a discussion], we performed bivariate Pearson correlations between the factors and to related measures. Table 4 depicts the results for Study 1, that manipulated the level of immersion. We found significant correlations between *ownership* and *agency*, as well as between ownership and general presence, spatial presence, and realness. The *change* factor was correlated significantly with the general presence assessment. Further, we found correlations within the presence measures.

Table 2. The confirmed embodiment factors (CFA results).

|                       | Ownership | Agency | Change |
|-----------------------|-----------|--------|--------|
| OW1. myBody           | .81       |        |        |
| OW2. myBodyParts      | .73       |        |        |
| OW3. humanness        | .53       |        |        |
| OW4. belongsToMe      | .71       |        |        |
| AG1. myMovement       |           | .80    |        |
| AG2. controlMovements |           | .70    |        |
| AG3. causeMovements   |           | .72    |        |
| AG4. syncMovements    |           | .53    |        |
| CH1. myBodyChange     |           |        | .69    |
| CH2. echoHeavyLight   |           |        | .78    |
| CH3. echoTallSmall    |           |        | .48    |
| CH4. echoLargeThin    |           |        | .72    |

Note. Coefficients represent standardized path coefficients of the CFA. Correlations between factors: Ownership  $\sim$  Agency r=.69, Ownership  $\sim$  Change r=.17, Change  $\sim$  Agency r=-.16.

Bivariate Pearson correlations for Study 2, that modified the avatar personalization are presented in Table 5. The *ownership* factor correlated with *agency* and *change*. *Agency* and *ownership* correlated with the post-exposure similarity measure, whereas the *change* factor did not. All embodiment factors correlated with the proto-self-presence measure. Interestingly, the *agency* factor correlated with a perceived positive affect. No significant correlations were observed for Study 3.

# 7 VALIDATION STUDY: LATENCY AND LATENCY JITTER

An independent fourth study aimed at a first validation of the scale. Previous work suggested that latency negatively impacts virtual embodiment [88]. Thus, we hypothesized H1: *Latency negatively impacts components of virtual embodiment*. Although linear latencies were subject to previous investigations [88], the impact of latency jitter has not been assessed.

#### 7.1 Method

In a one-factor (*Latency Level*) repeated-measures design, we evaluated the impact of latency and latency jitter, meaning the non-periodic spontaneous peaks of latency, on the perception of the factors of the VEQ. Participants were exposed to four conditions of delayed and jitter-delayed simulation display (baseline, LB; small latency, LS; large latency, LL; latency jitter, LJ).

#### 7.1.1 Procedure

The procedure followed the format depicted in Fig. 5 in repeated fashion. We welcomed participants and informed them, before assessing the pre-study questionnaire. The exposure conditions were then presented to the participants in randomized order. In each trial, the participants were calibrated, exposed to the simulation and induction, followed by an assessment of the dependent measures. In the audio instructions, the participants were specifically instructed to perform more rapid and fluid movements (e.g., "Raise your left arm at moderate speed in front of you, and lower it back down next to your hip. Repeat this movement ten times, and focus on your arm while doing so"). The instructions lasted for 282 s.

# 7.1.2 Apparatus

We used a similar apparatus Study 2. By buffering the tracking input data from the motion tracking system, artificial delays were introduced into the simulation by buffering and delaying the replication of the body motion tracking data. We prevented biasing sickness effects and influenced only the delay of the body movements, but did not influence the delay of the virtual camera (head movements, respectively), which, therefore, transformed according to the raw system delay without further modifications. Thus, the body motion was delayed, whereas the camera/head pose was not. We adapted the procedure described by Stauffert et al. [79] to introduce latency jitter, which uses a stochastical model for latency distribution, introducing high-latency spikes into

Table 3. The Resulting Virtual Embodiment Questionnaire (VEQ).

**VEQ Ownership** - Scoring: ([OW1] + [OW2] + [OW3] + [OW4]) / 4 **OW1.** myBody

It felt like the virtual body was my body.

OW2. myBodyParts

It felt like the virtual body parts were my body parts.

OW3. humanness

The virtual body felt like a human body.

OW4. belongsToMe

It felt like the virtual body belonged to me.

**VEQ Agency** - Scoring: ([AG1] + [AG2] + [AG3] + [AG4]) / 4 **AG1.** myMovement

The movements of the virtual body felt like they were my movements.

AG2. controlMovements

I felt like I was controlling the movements of the virtual body.

AG3, causeMovements

I felt like I was causing the movements of the virtual body.

AG4. syncMovements

The movements of the virtual body were in sync with my own movements.

 $VEQ\ Change$  - Scoring: ([CH1] + [CH2] + [CH3] + [CH4]) / 4

CH1. myBodyChange

I felt like the form or appearance of my own body had changed.

CH2. echoHeavyLight

I felt like the weight of my own body had changed.

CH3. echoTallSmall

I felt like the size (height) of my own body had changed.

CH4. echoLargeThin

I felt like the width of my own body had changed.

Note. Participant instructions: Please read each statement and answer on a 1 to 7 scale indicating how much each statement applied to you during the experiment. There are no right or wrong answers. Please answer spontaneously and intuitively. Scale example: 1-strongly disagree, 4-neither agree nor disagree, 7-strongly agree. A professional service was consulted for the translation.

the simulation. Motion-to-photon latency of the resulting simulations was approximated by video frame counting (Canon, 1000 Hz). The measures resulted in M=90.12 ms (SD=16.14 ms) for the simulation baseline  $L_B$ , M=206.93 ms (SD=16.47 ms) for the small delay  $L_S$ , M=353.07 ms (SD=15.38 ms) for the larger delay  $L_L$ , and M=102.58 ms (SD=49.71 ms) for  $L_J$ .  $L_B$ ,  $L_S$ , and  $L_L$  were measured with 60 samples (see Fig. 8). Despite measuring N=165 repetitions in the jitter condition  $L_J$ , the resulting mean and SD may not accurately reflect the induced jitter, due to some spikes that could not be captured using the motion-apex measurement applied. Users were embodied with the generic avatars (see Fig. 4).

## 7.1.3 Measures

We assessed the proposed virtual embodiment questions ( $\alpha$ s  $\geq$  .771) and performed a comparison to the questionnaire developed for RHI experiments by Kalckert and Ehrsson (KE) [38] (partly adapted from [49]), that measures ownership ( $\alpha$ s  $\geq$  .801), ownership control ( $\alpha$ s  $\geq$  .655), agency ( $\alpha$ s  $\geq$  .636), and agency control ( $\alpha$ s between .239 and .563) with a 7-point Likert-type scale (1-strongly disagree, 7-strongly

Table 4. Significant Bivariate Pearson Correlations (r) - Study 1.

|           | AG    | СН | GP   | SP    | IN    | RE    |
|-----------|-------|----|------|-------|-------|-------|
| Ownership | .46** |    | .36* | .34*  |       | .42** |
| Change    |       |    | .30* |       |       |       |
| GP        |       |    |      | .75** | .59** | .53** |
| SP        |       |    |      |       | .63** | .40** |

Note. \*p < .05; \*\*p < .01. AG Agency, CH Change, GP General Presence, SP Spatial Presence, IN Involvement, RE Realness.

Table 5. Significant Bivariate Pearson Correlations (r) – Study 2.

|      | AG    | СН    | PSP   | CSP   | PA    | SPre | SPo   |
|------|-------|-------|-------|-------|-------|------|-------|
| OW   | .51** | .37** | .70** |       |       |      | .33*  |
| AG   |       |       | .65** | .35*  | .43** |      | .31*  |
| CH   |       |       | .30*  |       |       |      |       |
| PSP  |       |       |       | .37*  | .33*  |      | .43** |
| ESP  |       |       |       | .40** |       | .36* | .32*  |
| CSP  |       |       |       |       | .31*  |      | .43** |
| PA   |       |       |       |       |       | .35* | .31*  |
| SPre |       |       |       |       |       |      | .44** |

Note. \* p < .05; \*\* p < .01. OW ownership, AG agency, CH change, PSP proto-self-presence, CSP core self-presence, PA positive affect, SPre similarity pre-exposure, SPo similarity post-exposure.

agree). The questioning of this measure was adapted to fit the scenario (e.g., "The rubber hand moved just like I wanted it to, as if it was obeying my will" = "The virtual body moved just like I wanted it to, as if it was obeying my will"). The scale reliabilities are presented in Table 6. As manipulation control, we asked how realistic, natural, and synchronous the movements of the avatar appeared to the participants: "The movements were realistic," "The movements were in synchrony to my own movements" (1–strongly disagree, 7–strongly agree). Further measures are not part of the present discussion. No severe sickness effects occurred.

#### 7.1.4 Participants

We excluded participants when problems or severe tracking errors occured. The final sample consisted of 22 participants (17 female, 5 male,  $M_{age} = 21.77$ ,  $SD_{age} = 3.62$ , 22 students), of whom 21 had previous experience with VR.

# 7.2 Results

# 7.2.1 Comparisons

We calculated repeated-measures ANOVAs for each dependent variable. Where the assumption of sphericity was violated, we report Greenhouse–Geisser corrected values. Fig. 8 depicts the descriptive results. We found a significant main effect for *ownership*; F(3,63) =3.57, p = .024,  $\eta_p^2 = .138$ . Similarly, agency measure was affected; F(1.741,63.553) = 7.50, p = .003,  $\eta_p^2 = .263$ . No significant impacts were observed for *change*. We did not observe any significant main effects in the agency and ownership measures of the scale adapted from KE [38]. The synchronicity assessment showed a significant main effect F(1.905, 40.005) = 7.077, p = .003,  $\eta_p^2 = .252$ . Table 7 depicts the comparison results of all measures. In contrast, neither the realism, nor the naturalness of behavior showed a significant main effect. The strongest linear latency injection (LL) yielded to the lowest scoring of ownership and agency (see Fig. 8). The jitter condition was similarly affected, but resulted in significantly better ratings than the condition with the largest latency injection. The lower level linear latency (LS) had comparable results to the jitter-injected condition. Similarly, the synchronicity ratings were affected (see Fig. 8).

Table 6. Reliabilities of the Validation Study Measures.

|        | LB (90ms) | LS (207ms) | LL (353ms) | LJ (Jitter) |
|--------|-----------|------------|------------|-------------|
| OW VEQ | .882      | .926       | .865       | .869        |
| AG VEQ | .786      | .777       | .784       | .771        |
| CH VEQ | .870      | .896       | .880       | .865        |
| AG KE  | .747      | .762       | .636       | .835        |
| AC KE  | .497      | .563       | .239       | .479        |
| OW KE  | .831      | .801       | .830       | .884        |
| OC KE  | .814      | .801       | .655       | .739        |

Note. Values depict Cronbach's \alpha

Table 7. Comparisons of Study 4 (Within-Subjects Effects).

|                        | F(df)      | p      | $\eta_p^2$ |
|------------------------|------------|--------|------------|
| OW VEQ                 | 3.36(3.00) | .024   | .138       |
| AG VEQ                 | 7.50(1.74) | < .001 | .263       |
| CH VEQ                 | 0.77(3.00) | .515   | .035       |
| OW KE                  | 1.82(2.02) | .175   | .080       |
| OC KE                  | 1.87(3.00) | .162   | .082       |
| AG KE                  | 1.98(1.74) | .158   | .086       |
| AC KE                  | 0.65(3.00) | .588   | .030       |
| Movement Realism       | 1.62(1.69) | .214   | .072       |
| Movement Naturalism    | 1.18(1.90) | .317   | .053       |
| Movement Synchronicity | 7.08(1.90) | .003   | .252       |

Note. Greenhouse-Geisser corrections were applied where sphericity was violated.

![](_page_6_Figure_17.jpeg)

Fig. 7. Latency manipulation. 60 sample measures of the induced latency assessed by frame counting.

## 7.2.2 Correlations

Pearson correlations are depicted in Table 8. The synchronicity assessment showed large correlations with the *agency* factor of the VEQ and the agency factor of the scale from KE [38]. Furthermore, synchronicity showed a medium to large correlation with the *ownership* factor, and the KE ownership factor. In turn, *ownership* showed medium to large correlations with *agency*, and a large correlation with ownership (KE) and ownership control (KE) across all measures. Interestingly, we did not find stable correlations between the perceived naturalness, synchronicity, and realism of the movement, providing room for further discussion.

#### 7.3 Discussion

The results support H1, that agency is negatively affected by simulation delays, which is in line with previous findings [88]. The descriptive results reveal that a jitter (in the applied spectrum) can result in a significantly decreased perception of agency, that is comparable to an average latency of approximately 207 ms (LS), which emphasizes the negative impact of latency jitter (LJ). However, the total delay of about 353 ms (LL) performed significantly worse than both, the LS and the jitter condition LJ, regarding perceived agency and perceived ownership, which quantifies the impact of jitter to some extent. The correlations confirmed that the VEQ picks up modifications in movement synchronicity. Although we found expected correlations between the agency factor and the additionally assessed agency (KE) and ownership (KE) measures, variance analysis revealed that the VEQ showed greater sensitivity in the present scenario. This may result from the fact that the (KE) questions were developed for the RHI (i.e., physical world body part) scenarios. Further, we adapted their question phrasing slightly to fit the virtual scenario. Although the results confirmed the expected correlations between ownership and agency, we could show that the *change* factor was not affected by modifications in the motion dimension, and thus, the VEQ validly discriminates the factors to this regard. One limitation is that the agency control measure adapted from

![](_page_7_Figure_2.jpeg)

Fig. 8. **Latency impacts.** Descriptive results of the VEQ assessment. *Note. Error bars denote standard errors.* \*\*p < .01; \*p < .05.

the (KE) questionnaire had overall low reliabilities, which is, in turn, a further argument for the proposed VEQ. In conclusion, we found significant impacts of latency and jitter on ownership and agency, and could further quantify the impact of jitter.

#### 8 GENERAL DISCUSSION

Our goal was the construction and initial validation of a questionnaire to assess virtual embodiment. The proposed scale is not merely theoretical, but instead, its factors are statistically confirmed through scale development. The CFA confirmed the previously explored factors (PCA) of virtual body ownership, agency, and change in the perceived body schema [72].

Each factor is assessed with four items, and thus feasible to assess in empirical research, even in in-situ assessments. To the best of our knowledge, this is the first scale presentation with a confirmed factor structure. The latter of which could especially be relevant for VR applications in the context of therapy and disorder treatment [59]. While further studies should perform an exploration and validation of the factor, it could be a predecessor for the Proteus Effect [92], as a difference in appearance or form of the avatar representation of the user is a prerequisite. Future research may investigate potential moderations, e.g., whether higher ownership or agency foster a perceived change of the own body schema (see Fig. 9). These insights would be specifically interesting, considering that avatar appearance realism as well as avatar personalization [1] were argued to have a moderating to substantial impact on embodiment [3, 45, 54, 86]. In turn, this may suggest that alterations (such as used for a proteus effect) would act as antipole. The presented results cannot provide further evidence, to that regard, and future research is needed.

Regarding the performance of the VEQ, acceptable to good **reliabilities** were confirmed with analyses of Cronbach's  $\alpha$  throughout all studies, including the initial validation study. In contrast to previous component identifications [49], the VEQ focuses on virtual experiences. The VEQ *validly* detected manipulations of control and showed higher sensitivity to (virtual) agency manipulations compared to a previous scale constructions [38] that aimed at assessing physical world RHI-like experiments.

We further showed that the proposed measure to part correlates with related constructs of presence or self-presence but discriminates those from virtual embodiment components. By investigating internal correlations of the VEQ, we could also confirm a correlation between agency and ownership as mentioned in previous works (e.g., [15, 83]). The *change* component assessing the perceived change of one's own body schema seems to be separable, in most regards.

Table 8. Significant Bivariate Pearson Correlations - Validation Study.

|                  | OW    | AG    | CH  | AG    | AC   | OW    | OC    |
|------------------|-------|-------|-----|-------|------|-------|-------|
|                  | VEQ   | VEQ   | VEQ | KE    | KE   | KE    | KE    |
| $MR L_B$         |       | .58** |     | .71** |      |       |       |
| $MR L_S$         | .48*  | .50*  |     | .67** |      |       |       |
| $MR L_L$         |       | .49*  |     |       |      |       |       |
| $MR L_J$         | .53*  | .68** |     | .68** |      | .49*  |       |
| $MN L_B$         | .45*  | .51*  |     | .55** |      |       |       |
| $MN L_S$         | .49*  |       |     |       |      |       |       |
| $MN L_L$         |       |       |     |       |      |       | .45*  |
| $MN L_J$         | .66** | .46*  |     | .43*  |      | .59** | .60** |
| $MS L_B$         |       | .57** |     | .80** |      |       |       |
| $MS L_S$         | .61** | .66** |     | .54** |      | .44*  | .50*  |
| $MS L_L$         | .47*  | .80** |     | .66** |      | .62** |       |
| $MS L_J$         | .59** | .77** |     | .55** |      | .61** | .45*  |
| $OW L_B$         |       | .48*  |     |       | .52* | .84** | .71** |
| $OW L_S$         |       | .53*  |     |       | .50* | .88** | .72** |
| $OW L_L$         |       | .44*  |     |       |      | .90** | .62** |
| $OW L_J$         |       | .56** |     |       |      | .93** | .67** |
| $AG L_B$         |       |       |     | .74** |      |       |       |
| $AG L_S$         |       |       |     | .71** |      | .47*  |       |
| $AGL_L$          |       |       |     | .83** |      | .58** |       |
| $AG L_J$         |       |       |     | .79** |      | .53*  |       |
| $\mathrm{CH}L_S$ |       |       |     |       | .48* |       |       |
|                  |       |       |     |       | _    |       |       |

Note. \* p < .05; \*\* p < .01; MR movement realism, MN movement naturalism, MS movement synchronicity, OWVEQ ownership, AGVEQ agency, CHVEQ change; Comparison measures: AGKE agency, ACKE agency control, OWKE ownership, OCKE ownership control, KE adapted from [38].

In contrast to other related factor suggestions [28, 38], the VEQ does not include "agency control", "ownership control", "external appearance," or "response to external stimuli," which could be valid extensions, in the case the factor structure and consistency is kept robust. However, as reviewed in Section 1, the previous literature on physical and virtual embodiment mainly identified body ownership, agency, and self-location as components (e.g. [10, 11, 38, 39, 54, 59]). The VEQ lacks of the assessment of self-location. The initial and updated questionnaire did not strictly concentrate on this factor, due to limited related work that assessed this component through questionnaires. We further interpret from previous literature, that an impact on (disturbed) self-location (self-localization) is a typically present with disorders (paroxysmal illusions) evoking disrupted body perception, such as heautoscopy, out-of-body experiences, or autoscopic hallucinations (see [15,50]). Although self-location discrepancies can be assessed in RHI experiments [13] or out-of-body experiences [5], it is typically not the goal of VR applications to evoke such effects but rather to accurately reassemble the user's location, first-person perspective (see [39] for a discussion), and behavior. Therefore, self-location may be subject to future extensions or alternatively assessed with implicit measures, such as displacement measures [13], or neurophysiological correlates [35]. However, it is yet unclear how to clearly investigate equivalent perceptual discrepancies of self-location in VR, and thus subject to future work, for example, by manipulating the relation of camera pose and body position [22]. The present findings are also limited by the applied scenarios and the collected sample form and size. Future work should consequently assess the reliability and consistency of the VEQ, along with its application mirror scenarios [27, 53] as well as to different (non-mirror) scenarios, such as user-embodying games [51] and activities [22], different extensions of the form of bodily representation [26], and more abstract avatar types with varying form and appearances [68], for example, in social settings [71, 94]. In this regard, we can only assume that the measure is **objective** (i.e., shielded from third-party bias) on the basis of our results, as shown in a multi-study setting.

The questionnaire and description, as well as supplementary material will be made available at virtualembodimentscale.com in multiple languages. The simulation codes are available upon request. We rec-

![](_page_8_Figure_2.jpeg)

Fig. 9. **Potential implications and discussion for future work.** While agency and ownership seem to stand in relation, the causality needs to be further explored. Ownership and agency may affect the perceived change in the own body schema, a factor that should be further validated. In turn, a rational hypothesis to be explored is the assumption of a relation between the perceived change in the own body schema (as a suggested condition) and the proteus effect.

ommend users of the questionnaire to assess using the questions stated in Table 3 with the according participant instructions (see the Note of Table 3). In our studies, we used 7-point scales. These are, feasible, but could be increased to 9 or 11 point measures. The items and resulting scoring for each factor is depicted in Table 3. Due to the factor structer in the VEQ, each factor (e.g., Ownership), could be used individually to address specific assessments of embodiment effects. In order to confirm factor consistency and reliability, users of the questionnaire should consequently assess internal reliability and consider further confirmatory analysis, for example, by using R with the lavaan package.

# **9 CONCLUSION**

In conclusion, we presented a virtual embodiment questionnaire (VEQ) that can be applied to various VR experiments to assess three latent factors of virtual embodiment: virtual body *ownership*, that describes the perception of perceiving a virtual body as the own body, *agency*, which describes the perception of feeling control over a virtual body, and *change*, which describes the perception of a perceived change of the own body schema. The latter of which may be specifically relevant for studies that consider variations in avatar appearance and avatar measures. Future work should further validate the presented factors and investigate potential scale performance, extensions, as well as the correlations to further related constructs.

# **ACKNOWLEDGMENTS**

The authors wish to thank Dominik Gall and Diana Rieger for thoughtful discussions and valuable feedback regarding the item design and during the scale construction. We further thank Jan-Philipp Stauffert for his help in realizing the latency study. We further thank Christopher Gottfert, David Fernes, and Patrick Schulz for their support during ¨ the data collection. This work was supported to part by grants from the Center for Digitalization in Bavaria (ZD.B/Bayern Innovativ), Germany, as well as by the XR Hub Bavaria initiative of the Bavarian State Ministry of Digitalization, Germany.

# **REFERENCES**

- [1] J. Achenbach, T. Waltemate, M. E. Latoschik, and M. Botsch. Fast generation of realistic virtual humans. In *Proceedings of the 23rd ACM Symposium on Virtual Reality Software and Technology*, pp. 1–10, 2017.
- [2] P. L. Anderson, M. Price, S. M. Edwards, M. A. Obasaju, S. K. Schmertz, E. Zimand, and M. R. Calamaras. Virtual reality exposure therapy for social anxiety disorder: A randomized controlled trial. 81(5):751, 2013. doi: 10.1037/a0033559

- [3] F. Argelaguet, L. Hoyet, M. Trico, and A. Lecuyer. The role of interaction ´ in virtual embodiment: Effects of the virtual hand representation. In *2016 IEEE Virtual Reality (VR)*, pp. 3–10. IEEE, 2016. doi: 10.1109/VR.2016. 7504682
- [4] K. C. Armel and V. S. Ramachandran. Projecting sensations to external objects: evidence from skin conductance response. *Proceedings of the Royal Society of London. Series B: Biological Sciences*, 270(1523):1499– 1506, 2003.
- [5] L. Aymerich-Franch, D. Petit, G. Ganesh, and A. Kheddar. Embodiment of a humanoid robot is preserved during partial and delayed control. In *2015 IEEE International Workshop on Advanced Robotics and Its Social Impacts*, 2015. doi: 10.1109/ARSO.2015.7428218
- [6] J. N. Bailenson and J. Blascovich. Avatars, 2004.
- [7] J. O. Bailey, J. N. Bailenson, and D. Casasanto. When does virtual embodiment change our minds? *Presence: Teleoperators and Virtual Environments*, 25(3):222–233, 2016.
- [8] S. Beck, A. Kunert, A. Kulik, and B. Froehlich. Immersive group-to-group telepresence. 19(4):616–625, 2013. doi: 10.1109/TVCG.2013.33
- [9] S. Benford, J. Bowers, L. E. Fahlen, C. Greenhalgh, and D. Snowdon. ´ User embodiment in collaborative virtual environments. In *Proceedings of the SIGCHI Conference on Human Factors in Computing Systems*, pp. 242–249. ACM Press/Addison-Wesley Publishing Co., 1995. doi: 10. 1145/223904.223935
- [10] O. Blanke. Multisensory brain mechanisms of bodily self-consciousness. 13(8):556, 2012. doi: 10/gddnh3
- [11] O. Blanke and T. Metzinger. Full-body illusions and minimal phenomenal selfhood. 13(1):7–13, 2009. doi: 10.1016/j.tics.2008.10.003
- [12] G. O. Boateng, T. B. Neilands, E. A. Frongillo, H. R. Melgar-Quinonez, ˜ and S. L. Young. Best practices for developing and validating scales for health, social, and behavioral research: A primer. *Frontiers in Public Health*, 6:149, 2018. doi: 10.3389/fpubh.2018.00149
- [13] M. Botvinick and J. Cohen. Rubber hands' feel'touch that eyes see. 391(6669):756–756, 1998. doi: 10.1038/35784
- [14] P. Bourke. Calculating Stereo Pairs, 1999.
- [15] N. Braun, S. Debener, N. Spychala, E. Bongartz, P. Soros, H. H. O. M ¨ uller, ¨ and A. Philipsen. The senses of agency and ownership: A review. 9:535, 2018. doi: 10.3389/fpsyg.2018.00535
- [16] T. A. Brown. *Confirmatory Factor Analysis for Applied Research*. Guilford Publications, 2014.
- [17] J. Carifio and R. J. Perla. Ten common misunderstandings, misconceptions, persistent myths and urban legends about Likert scales and Likert response formats and their antidotes. 3(3):106–116, 2007.
- [18] J. M. Cortina. What is coefficient alpha? an examination of theory and applications. *Journal of applied psychology*, 78(1):98, 1993.
- [19] M. Dallaire-Cotˆ e, P. Charbonneau, S. S.-P. C ´ otˆ e, R. Aissaoui, and D. R. ´ Labbe. Animated self-avatars for motor rehabilitation applications that are biomechanically accurate, low-latency and easy to use. In *Virtual Reality (VR), 2016 IEEE*, pp. 167–168. IEEE, 2016. doi: 10.1109/VR. 2016.7504706
- [20] N. David, A. Newen, and K. Vogeley. The "sense of agency" and its underlying cognitive and neural mechanisms. 17(2):523–534, 2008. doi: 10.1016/j.concog.2008.03.004
- [21] H. H. Ehrsson. The experimental induction of out-of-body experiences. 317(5841):1048–1048, 2007. doi: 10/ch9m6b
- [22] R. Fribourg, F. Argelaguet, A. Lecuyer, and L. Hoyet. Avatar and sense of ´ embodiment: Studying the relative preference between appearance, control and point of view. *IEEE Transactions on Visualization and Computer Graphics*, 26(5):2062–2072, 2020.
- [23] M. Furr. *Scale construction and psychometrics for social and personality psychology*. SAGE Publications Ltd, 2011.
- [24] S. Gallagher. Philosophical conceptions of the self: Implications for cognitive science. 4(1):14–21, 2000. doi: 10.1016/S1364-6613(99)01417 -5
- [25] S. Gallagher. *How the Body Shapes the Mind*. Clarendon Press, 2006.
- [26] B. Gao, J. Lee, H. Tu, W. Seong, and H. Kim. The effects of avatar visibility on behavioral response with or without mirror-visual feedback in virtual environments. In *2020 IEEE Conference on Virtual Reality and 3D User Interfaces Abstracts and Workshops (VRW)*, pp. 781–782. IEEE, 2020.

- [27] M. Gonzalez-Franco, D. P ´ erez-Marcos, B. Spanlang, and M. Slater. The ´ contribution of real-time mirror reflections of motor actions on virtual body ownership in an immersive virtual environment. In *Virtual Reality Conference (VR), 2010 IEEE*, pp. 111–114. IEEE, 2010. doi: 10.1109/VR. 2010.5444805
- [28] M. G.-F. Gonzalez-Franco and T. C. Peck. Avatar Embodiment. Towards a Standardized Questionnaire. 5:74, 2018. doi: 10.3389/frobt.2018.00074
- [29] A. Haans, W. A. IJsselsteijn, and Y. A. de Kort. The effect of similarities in skin texture and hand shape on perceived ownership of a fake limb. 5(4):389–394, 2008. doi: 10.1016/j.bodyim.2008.04.003
- [30] D. He, F. Liu, D. Pape, G. Dawe, and D. Sandin. Video-based measurement of system latency. In *International Immersive Projection Technology Workshop*, 2000.
- [31] C. Heeter. Being there: The subjective experience of presence. 1(2):262– 271, 1992.
- [32] C.-C. Ho and K. F. MacDorman. Revisiting the uncanny valley theory: Developing and validating an alternative to the Godspeed indices. 26(6):1508–1518, 2010-11. doi: 10.1016/j.chb.2010.05.015
- [33] L. Hoyet, F. Argelaguet, C. Nicole, and A. Lecuyer. "Wow! i have six ´ Fingers!": Would You accept structural changes of Your hand in Vr? 3:27, 2016. doi: 10.3389/frobt.2016.00027
- [34] S. Janke and A. Glockner-Rist. Deutsche Version der Positive and Negative ¨ Affect Schedule (PANAS). In *Zusammenstellung Sozialwissenschaftlicher Items Und Skalen. Doi*, vol. 10, p. 6102, 2014.
- [35] C. Jeunet, L. Albert, F. Argelaguet, and A. Lecuyer. "do you feel in ´ control?": towards novel approaches to characterise, manipulate and measure the sense of agency in virtual environments. *IEEE transactions on visualization and computer graphics*, 24(4):1486–1495, 2018.
- [36] Y. U. Jihun and P. Jungwoon. Head-mounted display with facial expression detecting capability, 2017-03.
- [37] S. Jung, G. Bruder, P. J. Wisniewski, C. Sandor, and C. E. Hughes. Over my hand: Using a personalized hand in vr to improve object size estimation, body ownership, and presence. In *Proceedings of the Symposium on Spatial User Interaction*, pp. 60–68. ACM, 2018.
- [38] A. Kalckert and H. H. Ehrsson. Moving a rubber hand that feels like your own: A dissociation of ownership and agency. 6, 2012. doi: 10. 3389/fnhum.2012.00040
- [39] K. Kilteni, R. Groten, and M. Slater. The sense of embodiment in virtual reality. 21(4):373–387, 2012. doi: 10.1162/PRES a 00124
- [40] K. Kilteni, A. Maselli, K. P. Kording, and M. Slater. Over my fake body: Body ownership illusions for studying the multisensory basis of own-body perception. 9, 2015. doi: 10.3389/fnhum.2015.00141
- [41] R. Klevjer. Enter the avatar: The phenomenology of prosthetic telepresence in computer games. In *The Philosophy of Computer Games*, pp. 17–38. Springer, 2012.
- [42] P. Kline. *The handbook of psychological testing*. Psychology Press, 2000.
- [43] R. B. Kline. *Principles and Practice of Structural Equation Modeling 3 Rd Ed*. New York, NY, The Guilford Press, 2010.
- [44] A. Kulik, A. Kunert, S. Beck, C.-F. Matthes, A. Schollmeyer, A. Kreskowski, B. Frohlich, S. Cobb, and M. D'Cruz. Virtual Valca- ¨ monica: Collaborative exploration of prehistoric petroglyphs and their surrounding environment in multi-user virtual reality. 26(03):297–321, 2018. doi: 10.1162/pres a 00297
- [45] M. Latoschik, D. Roth, D. Gall, J. Achenbach, T. Waltemate, and M. Botsch. The Effect of Avatar Realism in Immersive Social Virtual Realities. In *Proceedings of ACM Symposium on Virtual Reality Software and Technology*, pp. 39:1–39:10, 2017. doi: 10.1145/3139131.3139156
- [46] M. E. Latoschik, J.-L. Lugrin, and D. Roth. FakeMi: A fake mirror system for avatar embodiment studies. In *Proceedings of the 22nd ACM Conference on Virtual Reality Software and Technology*, pp. 73–76. ACM, 2016. doi: 10.1145/2993369.2993399
- [47] B. Lenggenhager, M. Mouthon, and O. Blanke. Spatial aspects of bodily self-consciousness. *Consciousness and cognition*, 18(1):110–117, 2009.
- [48] B. Lenggenhager, T. Tadi, T. Metzinger, and O. Blanke. Video ergo sum: Manipulating bodily self-consciousness. 317(5841):1096–1099, 2007. doi: 10.1126/science.1143439
- [49] M. R. Longo, F. Schu¨ur, M. P. Kammers, M. Tsakiris, and P. Haggard. ¨ What is embodiment? A psychometric approach. 107(3):978–998, 2008- 06. doi: 10.1016/j.cognition.2007.12.004
- [50] C. Lopez, P. Halje, and O. Blanke. Body ownership and embodiment: Vestibular and multisensory mechanisms. 38(3):149–161, 2008.

- [51] J.-L. Lugrin, M. Ertl, P. Krop, R. Klupfel, S. Stierstorfer, B. Weisz, ¨ M. Ruck, J. Schmitt, N. Schmidt, and M. E. Latoschik. Any "body" ¨ there? avatar visibility effects in a virtual reality game. In *2018 IEEE Conference on Virtual Reality and 3D User Interfaces (VR)*, pp. 17–24. IEEE, 2018.
- [52] J.-L. Lugrin, J. Latt, and M. E. Latoschik. Anthropomorphism and Illusion of Virtual Body Ownership. In *International Conference on Artificial Reality and Telexistence Eurographics Symposium on Virtual Environments*, 2015.
- [53] J.-L. Lugrin, D. Zilch, D. Roth, G. Bente, and M. E. Latoschik. Facebo: Real-time face and body tracking for faithful avatar synthesis. In *2016 IEEE Virtual Reality*, pp. 225–226. IEEE, 2016. doi: 10.1109/VR.2016. 7504735
- [54] A. Maselli and M. Slater. The building blocks of the full body ownership illusion. 7, 2013. doi: 10.3389/fnhum.2013.00083
- [55] M. Meehan, B. Insko, M. Whitton, and F. P. Brooks Jr. Physiological measures of presence in stressful virtual environments. In *Acm transactions on graphics (tog)*, vol. 21, pp. 645–652. ACM, 2002.
- [56] B. J. Mohler, S. H. Creem-Regehr, W. B. Thompson, and H. H. Bulthoff. ¨ The effect of viewing a self-avatar on distance judgments in an hmd-based virtual environment. *Presence: Teleoperators and Virtual Environments*, 19(3):230–242, 2010.
- [57] A. Muhlberger, M. J. Herrmann, G. Wiedemann, H. Ellgring, and P. Pauli. ¨ Repeated exposure of flight phobics to flights in virtual reality. 39(9):1033– 1050, 2001. doi: 10.1016/S0005-7967(00)00076-0
- [58] V. I. Petkova and H. H. Ehrsson. If I were you: Perceptual illusion of body swapping. 3(12):e3832, 2008. doi: 10.1371/journal.pone.0003832
- [59] I. V. Piryankova, H. Y. Wong, S. A. Linkenauger, C. Stinson, M. R. Longo, H. H. Bulthoff, and B. J. Mohler. Owning an overweight or ¨ underweight body: Distinguishing the physical, experienced and virtual body. 9(8):e103428, 2014. doi: 10/gf36rz
- [60] T. Piumsomboon, G. A. Lee, J. D. Hart, B. Ens, R. W. Lindeman, B. H. Thomas, and M. Billinghurst. Mini-Me: An Adaptive Avatar for Mixed Reality Remote Collaboration. In *Proceedings of the 2018 CHI Conference on Human Factors in Computing Systems*, p. 46. ACM, 2018. doi: 10. 1145/3173574.3173620
- [61] A. Powers and S. Kiesler. The advisor robot: Tracing people's mental model from a robot's physical attributes. In *Proceedings of the 1st ACM SIGCHI/SIGART Conference on Human-Robot Interaction*, pp. 218–225. ACM, 2006. doi: 10.1145/1121241.1121280
- [62] R. Ratan and B. S. Hasler. Exploring Self-Presence in Collaborative Virtual Teams. 8(1):11–31, 2010.
- [63] R. Ratan and Y. J. Sah. Leveling up on stereotype threat: The role of avatar customization and avatar embodiment. 50:367–374, 2015. doi: 10. 1016/j.chb.2015.04.010
- [64] T. Raykov and G. A. Marcoulides. *Introduction to psychometric theory*. Routledge, 2011.
- [65] G. Riva, L. Melis, and M. Bolzoni. Treating body-image disturbances. 40(8):69–72, 1997. doi: 10.1145/257874.257890
- [66] A. Rizzo, G. Reger, G. Gahm, J. Difede, and B. O. Rothbaum. Virtual reality exposure therapy for combat-related PTSD. In *Post-Traumatic Stress Disorder*, pp. 375–399. Springer, 2009.
- [67] D. Roth, G. Bente, P. Kullmann, D. Mal, C. F. Purps, K. Vogeley, and M. E. Latoschik. Technologies for social augmentations in user-embodied virtual reality. In *25th ACM Symposium on Virtual Reality Software and Technology*, VRST '19. Association for Computing Machinery, New York, NY, USA, 2019. doi: 10.1145/3359996.3364269
- [68] D. Roth, C. Kleinbeck, T. Feigl, C. Mutschler, and M. E. Latoschik. Beyond Replication: Augmenting Social Behaviors in Multi-User Virtual Realities. In *2018 IEEE Conference on Virtual Reality and 3D User Interfaces (VR)*, pp. 215–222. IEEE, 2018. doi: 10.1109/VR.2018.8447550
- [69] D. Roth, P. Kullmann, G. Bente, D. Gall, and M. E. Latoschik. Effects of hybrid and synthetic social gaze in avatar-mediated interactions. In *2018 IEEE International Symposium on Mixed and Augmented Reality Adjunct (ISMAR-Adjunct)*, pp. 103–108. IEEE, 2018. doi: 10.1109/ISMAR -Adjunct.2018.00044.
- [70] D. Roth, J.-L. Lugrin, J. Buser, G. Bente, A. Fuhrmann, and M. E. ¨ Latoschik. A Simplified Inverse Kinematic Approach for Embodied VR Applications. In *Proceedings of the IEEE Virtual Reality (IEEE VR) Conference 2016*, 2016. doi: 10.1109/VR.2016.7504760

- [71] D. Roth, J.-L. Lugrin, D. Galakhov, A. Hofmann, G. Bente, M. E. Latoschik, and A. Fuhrmann. Avatar Realism and Social Interaction Quality in Virtual Reality. In *2016 IEEE Virtual Reality*, pp. 277–278. IEEE, 2016. doi: 10.1109/VR.2016.7504761
- [72] D. Roth, J.-L. Lugrin, M. E. Latoschik, and S. Huber. Alpha IVBO Construction of a Scale to Measure the Illusion of Virtual Body Ownership. In *Proceedings of the 2017 CHI Conference Extended Abstracts on Human Factors in Computing Systems*, pp. 2875–2883. ACM, 2017. doi: 10.1145/ 3027063.3053272
- [73] R. Schroeder and A.-S. Axelsson. *Avatars at Work and Play: Collaboration and Interaction in Shared Virtual Environments*, vol. 34. Springer, 2006.
- [74] T. W. Schubert. The sense of presence in virtual environments: A threecomponent scale measuring spatial presence, involvement, and realness. 15(2):69–71, 2003. doi: 10.1026//1617-6383.15.2.69
- [75] R. Skarbez, F. P. Brooks, Jr, and M. C. Whitton. A survey of presence and related concepts. *ACM Computing Surveys (CSUR)*, 50(6):1–39, 2017.
- [76] M. Slater, D. Perez Marcos, H. Ehrsson, and M. V. Sanchez-Vives. To- ´ wards a digital body: The virtual arm illusion. 2:6, 2008. doi: 10.3389/ neuro.09.006.2008
- [77] M. Slater, D. Perez Marcos, H. Ehrsson, and M. V. Sanchez-Vives. Induc- ´ ing illusory ownership of a virtual body. 3:29, 2009. doi: 10.3389/neuro. 01.029.2009
- [78] M. Slater, B. Spanlang, M. V. Sanchez-Vives, and O. Blanke. First person experience of body transfer in virtual reality. 5(5):e10564, 2010. doi: 10. 1371/journal.pone.0010564
- [79] J.-P. Stauffert, F. Niebling, and M. E. Latoschik. Effects of Latency Jitter on Simulator Sickness in a Search Task. In *2018 IEEE Conference on Virtual Reality and 3D User Interfaces (VR)*, pp. 121–127. IEEE, 2018. doi: 10.1109/VR.2018.8446195
- [80] W. Steptoe, A. Steed, and M. Slater. Human tails: Ownership and control of extended humanoid avatars. 19(4):583–590, 2013. doi: 10.1109/TVCG .2013.32
- [81] E. R. Thompson. Development and validation of an internationally reliable short-form of the positive and negative affect schedule (PANAS). 38(2):227–242, 2007. doi: 10.1177/0022022106297301
- [82] M. Tsakiris. My body in the brain: A neurocognitive model of bodyownership. 48(3):703–712, 2010. doi: 10.1016/j.neuropsychologia.2009. 09.034
- [83] M. Tsakiris, G. Prabhu, and P. Haggard. Having a body versus moving your body: How agency structures body-ownership. 15(2):423–432, 2006. doi: 10.1016/j.concog.2005.09.004
- [84] M. Tsakiris, S. Schutz-Bosbach, and S. Gallagher. On agency and body- ¨ ownership: Phenomenological and neurocognitive reflections. 16(3):645– 660, 2007. doi: 10.1016/j.concog.2007.05.012
- [85] M. Usoh, E. Catena, S. Arman, and M. Slater. Using presence questionnaires in reality. *Presence: Teleoperators & Virtual Environments*, 9(5):497–503, 2000.
- [86] T. Waltemate, D. Gall, D. Roth, M. Botsch, and M. E. Latoschik. The impact of avatar personalization and immersion on virtual body ownership, presence, and emotional response. 24(4):1643–1652, 2018. doi: 10.1109/ TVCG.2018.2794629
- [87] T. Waltemate, F. Hulsmann, T. Pfeiffer, S. Kopp, and M. Botsch. Realizing ¨ a low-latency virtual reality environment for motor learning. pp. 139–147. ACM Press, 2015. doi: 10.1145/2821592.2821607
- [88] T. Waltemate, I. Senna, F. Hulsmann, M. Rohde, S. Kopp, M. Ernst, and ¨ M. Botsch. The impact of latency on perceptual judgments and motor performance in closed-loop interaction in virtual reality. In *Proceedings of the 22nd ACM Conference on Virtual Reality Software and Technology*, pp. 27–35. ACM, 2016. doi: 10.1145/2993369.2993381
- [89] C. Ware, K. Arthur, and K. S. Booth. Fish tank virtual reality. In *Proceedings of the INTERACT'93 and CHI'93 Conference on Human Factors in Computing Systems*, pp. 37–42. ACM, 1993. doi: 10.1145/169059.169066
- [90] L. Wilson, B. Chou, and K. Seko. Head mounted display, 2017-04.
- [91] B. G. Witmer and M. J. Singer. Measuring presence in virtual environments: A presence questionnaire. 7(3):225–240, 1998. doi: 10.1162/ 105474698565686
- [92] N. Yee. The Proteus Effect: Behavioral Modification via Transformations of Digital Self-Representtation, 2007.
- [93] N. Yee and J. N. Bailenson. Walk a mile in digital shoes: The impact of embodied perspective-taking on the reduction of negative stereotyping in immersive virtual environments. pp. 24–26, 2006.

- [94] B. Yoon, H.-i. Kim, G. A. Lee, M. Billinqhurst, and W. Woo. The effect of avatar appearance on social presence in an augmented reality remote collaboration. In *2019 IEEE Conference on Virtual Reality and 3D User Interfaces (VR)*, pp. 547–556. IEEE, 2019.
- [95] J. Yu and J. Park. Real-time facial tracking in virtual reality. In *SIG-GRAPH ASIA 2016 VR Showcase*, p. 4. ACM, 2016. doi: 10.1145/2996376 .2996390