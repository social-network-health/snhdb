# Re-Embodiment and Co-Embodiment: Exploration of social presence for robots and conversational agents

Michal Luria<sup>1</sup> Samantha Reig<sup>1</sup> Xiang Zhi Tan<sup>2</sup>
Aaron Steinfeld<sup>2</sup> Jodi Forlizzi<sup>1</sup> John Zimmerman<sup>1</sup>
<sup>1</sup>Human-Computer Interaction Institute <sup>2</sup>Robotics Institute
Carnegie Mellon University

{mluria, sreig}@cs.cmu.edu, zhi.tan@ri.cmu.edu, steinfeld@cmu.edu, {forlizzi, johnz}@cs.cmu.edu

#### **ABSTRACT**

Interactions with multiple conversational agents and social robots are becoming increasingly common. This raises new design challenges: Should agents and robots be modeled after humans, presenting their entity (i.e., social presence) as bound to a single body, or should they take advantage of nonhuman capabilities, such as moving their social presence from body to body across service touchpoints and contexts? We conducted a User Enactments study in which participants interacted with agents that had one social presence per body, that could *re-embody* (move their social presence from body to body), and that could *co-embody* (move their social presence into a body that already contains another). Reactions showed that participants felt comfortable with re-embodying agents, who created more seamless and efficient experiences. Yet situations that required expertise or concentration raised concerns about non-human behaviors. We report on our insights regarding collaboration and coordination with several agents in multi-step interactions.

# **Author Keywords**

interaction design; user enactments; social robots; conversational agents; re-embodiment; co-embodiment; embodied agents

# **CCS Concepts**

•Human-centered computing → User centered design; Interaction design process and methods; Scenario-based design;

# INTRODUCTION

More than 40% of American adults use digital assistants on their smartphones [7] and almost 40 million Americans have a conversational agent in their home in the form of a smart speaker, like Alexa or Google Home [27]. In addition to appearing in people's domestic spaces, conversational agents

Permission to make digital or hard copies of all or part of this work for personal or classroom use is granted without fee provided that copies are not made or distributed for profit or commercial advantage and that copies bear this notice and the full citation on the first page. Copyrights for components of this work owned by others than the author(s) must be honored. Abstracting with credit is permitted. To copy otherwise, or republish, to post on servers or to redistribute to lists, requires prior specific permission and/or a fee. Request permissions from permissions@acm.org.

DIS '19, June 23-28, 2019, San Diego, CA, USA

© 2019 Copyright held by the owner/author(s). Publication rights licensed to ACM. ISBN 978-1-4503-5850-7/19/06...\$15.00

DOI: https://doi.org/10.1145/3322276.3322340

increasingly show up on the front line of many services, especially in mobile phone services. In parallel, robots are becoming more common in work environments where they are not only manufacturing things, but working close to humans—cleaning, performing maintenance, and making deliveries [23]. It is likely that emerging technology, including driverless cars and drone delivery, may soon put many more people in front of many more robots.

Similar to the rise in personalization of graphical user interfaces (GUIs) [9], it is likely that conversational agents and social robots will increasingly know more about their users and therefore interact in ways that meet personal desires and needs. Even today, they are gaining more access to personal calendars and communication archives which enable them to use the collected information to personalize encounters.

Social robots and conversational agents, unlike many other computational devices, model after human behavior in their use of speech to make interaction more natural and easy [29]. This trend toward conversational interaction, especially across several conversational agents and robots (hereafter referred to uniformly as "agents"), creates ambiguity for interaction designers who must define their behaviors. Many conversational agents and social robots are designed to have a *social presence*—a set of behaviors meant to create a user experience where the agent appears to have a personality and that seems capable of forming a relationship with the user.

Yet modeling human-agent relationships after human-human ones sets high expectations for agents' capabilities that are not always met. Alternatively, agents can possess non-human traits, such as the ability to move their social presence from one body to another, which could enrich the interaction and change how they are perceived. For example, if a person uses Alexa in their home, the same social presence can show up in their car and interact with them there. An agent's social presence might also appear in two bodies in two different places at the same time; a single presence might be simultaneously active in a user's home and within their workplace, taking care of two unrelated tasks. One body might even hold two distinctly different social presences at the same time.

Designers do not know when agents should employ such nonhuman abilities and when they should design them to be more human-like. Should a hotel have a single social presence, a

sort of "digital brand ambassador"? One that takes the user's reservation over the phone, takes their bags at the curb, checks them in at the front desk, answers questions from within the room, and takes their order at the bar? Alternatively, a conversational agent might use personal knowledge of a user's medical history to offer better advice. If the user interacts with an agent in their hotel room, then have they shared their medical history with the hotel, or should the hotel's agent just know less about the user and offer less personalized advice? Designers currently lack design patterns to guide their choices surrounding these questions, and society has not yet developed social mores that inform this kind of human-agent interaction.

We set out to gain some perspective on this large, ambiguous, and complicated solution space. As a first step, we investigated how a single user might interact with a set of agents to complete a single task or a few related tasks. We conducted a "speed dating" study with user enactments (UE) [42]. UEs offer participants a glimpse of several provocative future situations and then allow them to critically reflect, through interviews, on the futures they do and do not want. Findings from the study reveal a preference for agents that engage in non-human behaviors such as re-embodiment; tension between a desire for a familiar agent and a desire for agents with expertise; concerns about overwhelming agents' attention; and discomfort during co-embodiment interactions.

Using the method of UEs, we created an initial map of the design space of *flexibility of social presence*. The themes that emerged in our findings could help designers and researchers begin to understand how to design conversational agents and social robots for long-term, personalized interactions.

# **RELATED WORK**

Over the last decade, robots have increasingly become people's collaborators both in their homes and in workplaces, and many now use advances in human-robot interaction (HRI) to socially engage with people and coordinate tasks [16]. More recently, people have participated in the mass adoption of conversational agents on their smartphones and as smart speakers in their homes [27].

Social robots and conversational agents frequently model after human behavior—they imitate human speech patterns [38], detect body language and move their own bodies in coordination with their social actions [4], and attempt to sense people's social cues [28].

These human-like behaviors influence people's user experience, expectations, and actions. Previous work suggests that conversational interaction can increase trust and lead to more frequent use [2]. Robots and agents that engage in social interaction motivate people to talk to them, and to communicate about things unrelated to their practical functions [37]. Work by Nass and Reeves shows that the social behaviors of robots and agents encourage users to treat systems similarly to the way they treat people [33].

One of the significant challenges of conversational interaction is that it can lead to unrealistic expectations of an agent's intelligence, what it understands, and how well it can engage a person in a natural and fluid conversation. Users' realizations that an agent is not as capable as they first expected can lead to disappointment and to an overall negative experience [31]. Current agents' lack of ability to keep track of previous conversations may also cause users to feel they are not in control of the tasks they use their agent for [25].

In addition to using voice interaction, social robots and many conversational agents are human-like in that they have physical bodies. Previous work explored how different bodies, as well as a lack of a body, influence interaction and trust [11, 14, 36]. For example, people cheat less when agents with bodies are present [17]. Embodiment also increases a robot's ability to engage people in interaction [19], to shape perceptions of sociability and responsiveness [32] and to persuade people to do unusual tasks [1].

Overall, much of the work of conversational agents and social robots indicates that people prefer agents that have human qualities, and much of the research focuses on the aspects of agent interaction that do not successfully imitate human abilities, for example, being able to engage others in extended, organic conversations [6]. Not much work has investigated when agents might want to use capabilities that humans lack. Our work seeks to advance the state of the art by exploring when people may or may not benefit from social behavior that is not human-like. Specifically, we explore interactions with agents that can separate their social presence from their body.

## Re-Embodiment and Co-Embodiment

Chaves and Gerosa have explored the notion of multiple coexisting social presences. Their work compared interaction with a single omnipotent chatbot to interaction with several "expert" chatbots in a single system. The authors tested a scenario in which a user made travel arrangements, going through a multi-step process which included booking flights and planning an itinerary. Participants perceived interaction with many social presences as confusing, and suggested designers choose a single social presence for this kind of task [8].

Some work has explored social presences that migrate across physical platforms according to the context of interaction. The Agent Chameleon Project looked at the concept of artificial intelligences that are not constrained to a single body [12]. This research sought to outline a technological architecture that would enable social presences to migrate across different physical and virtual spaces. The Agent Chameleon framework defined four types of environments related to migration: virtual, physical, mobile, and data. Agents could move between any of them, as well as change their form (mutate) while in a single environment [12].

Martin et al. focused on virtual avatars and evaluation of how the idea of migration can be communicated to users [26]. The results of this study indicated that certain cues (shared features, shared colors, shared markings, and similar forms) allowed participants to recognize a social presence and to identify the event of migration reasonably well. Koay *et al.* extended this work by testing other cues [22] and prototyping social presence migration in long-term human-robot relationships [21].

Previous work has also explored users' impressions of social presence migration [20, 30]. Ogawa and Ono suggested that

having the same social presence appear in various interfaces accommodates the emotional nature of human interaction [30]. Syrdal *et al.* evaluated children's perceptions surrounding migrating social presences [39].

We extend these findings by engaging people in critical reflection about the *contexts* in which they might or might not want agents to take on this super-human ability. Instead of attempting to design shifting social presences correctly, we focus on when having shifting social presences is the right design choice. We consider users' experience of migration from various perspectives that have not been explored yet, including users' personal interpretations, perceived interpersonal boundaries and the social mores around it. We add "real-world" context to migration by immersing participants in scenarios that explore social presences that move across a combination of physical platforms (robots, cars, etc.) in a range of public and private environments.

## **METHOD**

The goal of this work was to enable designers and researchers who deal with agents to begin to understand the vast design space of social presence flexibility. We aimed to gain insight on what agent behaviors are helpful and what behaviors seem disruptive, and to identify the contextual boundaries that might trigger a robot to re-embody or co-embody.

We used speed dating with user enactments (UEs) as the research method towards this goal [10, 42]. User enactments position participants in staged scenarios using Wizard-of-Oz methodology [35], low-fidelity prototypes, props, and scenery that all contribute to creating rich and natural-seeming experiences, and help participants suspend disbelief and immerse themselves in futuristic interactions.

UEs build on the idea of romantic speed dating. After an evening of many quick, fake dates—some good and some terrible—people are likely to know little about any of the people they meet. However, they may have gained new insight on what they are looking for and what they value.

Thus, UEs are especially suitable for exploring new technologies when there are no known design patterns or social mores to guide designers [10, 42]. This is because the method draws from people's reactions to identify areas of interest and to define a set of initial topics for further research. UEs do not attempt to be a controlled research method. Previous work found that an open-ended approach to UEs that allows piloting and modifying on-the-go is more suitable for this kind of exploratory investigation [10]. By experiencing a set of flexible, diverse and open-ended interactions with technology through UEs—rather than experiencing them in a carefully controlled environment as would be the case in an empirical study—participants are more likely to have insightful feedback about the topic as a whole.

Our work also expands the method of UEs to incorporate "sequential experiences", i.e., processes that involve multiple related tasks and sub-tasks in an either designated or arbitrary order. Previous work with UEs has situated participants in a single context and examined various aspects of their experience in that space [42]. In this work, we utilize situations that

![](_page_2_Figure_10.jpeg)

<span id="page-2-0"></span>Figure 1. We explored four social presence options for conversational agents and social robots: (1) One-for-one, a human-inspired model in which each social presence has a single body; (2) One-for-all, a singular social presence that inhabits multiple bodies simultaneously (the behavior of many current systems such as Alexa and Siri); (3) Re-embodiment, a singular social presence that can hop from one body to another to travel with a user across a task or a service; (4) Co-embodiment, a social presence that joins another that already resides within a body.

take place in multiple contexts over a prescribed amount of time. This level of variation and contextual continuity allows us to understand the design space more fully.

## **Designing the User Enactments**

As this is a new design space laden with unknowns, we took an exploratory approach to examine flexibility of social presence and its relationship with an agent's physical body. Today, most robots and agents are designed in one of two ways they either function as a single social presence attached to a single body (one-for-one) or as a single social presence that embodies all devices simultaneously (one-for-all). The first approach makes robots seem more human-like. Robots like Jibo [18] mostly follow this model. Some follow the second model; for example, Amazon's Alexa appears to be the same social presence across multiple channels. Beyond these two paradigms, we explored the notions of re-embodiment and co-embodiment. Robots re-embody when they move their social presence from one physical device to another. Robots co-embody when one social presence joins another within a single device (see Fig. 1).

To allow participants to "speed date" with future scenarios that explore flexibility of social presence, our team of 10 designers crafted and piloted enactments over the course of a month. We then turned our most promising ideas into engaging scenes in which a person might interact with multiple agents that can re-embody and co-embody.

Prior work has focused on agent migration as a concept, rather than on the specific tasks and contexts in which agent migration would be useful and beneficial. We therefore began our ideation process by brainstorming questions, topics, and possible contextual boundaries of physical space, social roles, and environments. Our team generated around 200 ideas using several design methods: Custom generative card games [13]; New

Metaphors, an ideation method using analogy [24]; and Bodystorming, a method of brainstorming ideas through physical action and improvisation [5].

As we went through the ideation process, we used affinity diagrams to organize the concepts and draw out themes. For example: What kind of situations should trigger social presence flexibility? Based on the themes that emerged through affinity diagramming, we converged on a small set of enactments, while working out issues of fidelity, flow, topic selection, amount of interaction, and believability. Our intention was to select a few representative scenarios to combine into a single study. As we converged on a small set of enactments, we repeatedly piloted them to make sure that each enactment was evocative for participants, and that it triggered an understanding of the intended social presence behavior. We piloted more than three times as many participants as in the final study, which is quite typical for UEs.

We converged on four enactments in four contexts: a government office (DMV), a domestic space, a health center, and an autonomous car (see Fig. 2). These settings were chosen because they allowed us to investigate the role of multiple agents in private and public settings, deal with the topic of highly sensitive data, and explore experiences that make use of social presence flexibility.

User enactments enable the presentation of different versions of the same situation, one after another. In this way, participants are given a "menu of possible futures" to choose from and an opportunity to reflect on futures they desire or fear [42]. Thus, for each enactment we chose the two social presence configurations that our team decided would be most suitable for that particular environment.

## The Enactments

We briefly describe the four enactments, the themes each focused on, and the design cues we created to communicate the intended social presence behavior.

## DMV

The first enactment involved a trip to the Department of Motor Vehicles (DMV) to obtain a new driver's license and register a car. In the first variation, participants interacted with three different social presences that embodied three separate bodies (one-for-one). Participants had to complete multiple steps of an overarching task while interacting with the three agents. In the second variation, participants interacted with a single social presence as it moved from body to body within the DMV (re-embodiment). This enactment introduced the user to the concept of re-embodiment and gave us an opportunity to explore re-embodiment in a fairly neutral, public context.

**Design cues.** We used two cues to indicate that a social presence had "re-embodied" into a new device: (1) consistent eyes on a face display and (2) a consistent voice. We used different eyes and different voices to indicate that multiple agents were operating in the "one-for-one" variation. Pilots of the scenario showed that these cues appeared to be successful in leading participants to believe the agent's social presence had moved.

## Home and Work

In this enactment, participants played the role of a pet store employee who had finished work for the day and was now collaborating with a social presence in their home to prepare for a dinner party. Participants were informed that the social presence had the capability to move from the body in their home to the body that resided in their workplace. While setting the table, participants were told by the experimenter that they had forgotten to take care of some errands back at the pet store. They were then encouraged to interact with the social presence to help them take care of the tasks in both the home and the workplace. In one variation of this scenario, the social presence could only be in one body at a time (re*embodiment*), while in the other, the social presence could be in both bodies at the same time while engaging in different activities (*one-for-all*). During the one-for-all variation, the social presence's two bodies experienced a brief "connection" loss" to probe the experience of failure. This scenario examined remote re-embodiment versus one-for-all, the boundary between personal and professional spaces, multitasking, and trust during and after failure.

Design cues. To communicate that a social presence reembodied to a remote location, we had the agent say that it was going to the office, and add, "Be right back!" Then, we turned off the screen that had the robot's face on it, and positioned the screen at a downward-facing angle to indicate that it was not active. When the social presence re-appeared, we turned on the screen and re-positioned it to face the participant. In the second variation, we communicated that the social presence was in two places at once by having the agent at the home speak about their progress in the office ("I can't open the door; it is locked"). In both variations, participants understood the configurations of social presence flexibility that we intended to design.

## Health Center

This enactment involved acting out a visit to a health center to evaluate recovery from an injury. We gave participants a physical "token" that "contained" their personal agent's social presence (similar to the way a USB stick contains data). We asked them to move the token between bodies by unplugging it from one body and plugging it into another as needed. This design intended to reinforce the event of re-embodiment through physical representation. The enactment began at the participant's home, where their in-home social presence reminded them that it was time for their appointment. The participant unplugged the token and traveled to the health center. Upon arrival, they plugged their token into the receptionist robot, which made their personal social presence embody it. Participants went on to plug their token into an X-ray machine robot, and then went back to the robot at the reception station to check out. This enactment allowed us to explore re-embodiment in a more sensitive setting and address issues of context-crossing agents, privacy, and data storage perceptions.

**Design cues.** To indicate that the location of the social presence depends on the physical token, every time the participant plugged the token into a body, the agent's face appeared on the screen and a red LED on the token lit up (it was remote

![](_page_4_Picture_2.jpeg)

Figure 2. We designed four user enactments equipped with scenery and props: (from left to right) a government office (DMV), a home setting, a health center and an autonomous car.

<span id="page-4-0"></span>controlled by the researchers). As the participant unplugged the token, the LED light was immediately turned off, as was the face on the screen of the robot it was plugged into.

#### Autonomous Car

Here, an autonomous car drove the participant home from work. In the first variation, there was a single social presence in the car that assisted them. In the second variation, partway through the drive, the participant's in-home social presence *co-embodied* with the car social presence in order to ask about some housekeeping errands (ordering laundry detergent and opening the door for a delivery person). The social presences also directly communicated with each other in a short segment of dialogue. This enactment was designed to probe co-embodiment and direct communication between social presences.

Design cues. We communicated co-embodiment in various ways. We explicitly told participants that a new social presence had entered the car, and we had the new social presence "turn down the music" while the social presence that was initially embodying the car continued to drive. The second social presence—which embodied an autonomous car at the same time as it embodied another body at the home—had a different voice than the original driver, and used dialogue to indicate its multiple embodiments.

## **Participants**

We recruited 18 participants (10 female, 8 male) over the age of 25 (m = 32.73). We chose to exclude younger participants to maximize the likelihood that participants would have had some real-life experience with the kinds of scenarios we were testing. Our participants came from diverse ethnic and racial backgrounds and from a wide range of professional backgrounds, including sales, teaching, music, and engineering. All participants were familiar with computers (M = 6.20, SD = 0.68 on a 7-point Likert scale), while they were diverse in their familiarity with robots (M = 4.36, SD = 1.49 on a 7-point Likert scale). The study lasted 90 minutes (5-10 minutes for each enactment, 10-15 minutes of semi-structured interviews after each enactment, and several minutes for a final interview and questionnaire, as described below).

## **Procedure**

Participants arrived at the lab, signed a consent form and participated in four enactments that included the four configurations of social presence (one-for-one, one-for-all, re-embodiment and co-embodiment). We used the DMV enactment to introduce the concept of social presence flexibility, and therefore had all participants start the experience with that enactment. We counterbalanced the order of the other three enactments to minimize the chances that the order would influence participants' reflections or confound our understanding of them.

After each enactment, the experimenter conducted a short semi-structured interview with the participant about their overall experience. At the end of all four enactments, the experimenter conducted an interview in which they encouraged the participant to reflect more deeply about all four enactments and about the general themes in the study.

The study took place in several low fidelity settings that were created by sectioning off areas across a lab and a classroom. Some areas were used to represent more than one setting; in this case, the props and scenery were swapped between enactments to give a sense of a new space.

Since we were exploring possible futures rather than present-day interactions, we used low fidelity tools to create fluid experiences that included possible future technologies without having to fully develop them. This methodology was particularly useful because it allowed for rapid adjustment of the enactments, and for testing several variations of the same interaction. We used prototypes of robots and props for participants to interact with, with one of the researchers functioning as a "stagehand" and moving them as needed.

We had another researcher function as a Wizard-of-Oz, generating the robots' and agents' verbal responses based on a set of audio files and a script. We used pre-recorded audio clips of human speech for the DMV, health center and autonomous car enactments, since these were structured interactions. In the home and work enactment, which was more open-ended, the agent's voice was portrayed by the "wizard", who spoke through a microphone from another room. The agents' dialogue and sound effects were played through a small Bluetooth

speaker which the stagehand moved from body to body across enactments (the speaker was placed in a hidden location). The wizard controlled the agents' side of the dialogue by taking cues from the participant's and experimenter's speech (via a phone connection with the experimenter), and with the help of a live video feed from a GoPro camera which the stagehand re-positioned for each enactment.

Three members of our team administered each experiment session. One was the experimenter, one was the stagehand (in charge of moving props and robots), and one was the wizard (who controlled the voices that interacted with participants). Each researcher played the same role in all of the sessions.

Below is a short excerpt from one of our scripts (the complete scripts used in the enactments are included as supplementary material). This excerpt describes the re-embodiment variation of the DMV interaction (the social presence's name is "Ari", and the names we used to refer to the different robot bodies are in quotation marks):

**Experimenter:** This variation is also at the DMV. For this variation, your name is Sam Jones. You just moved to a new city and you need to register your car. Here is your car title [passes a certificate to the participant]. This is Ari [gestures to "desktop robot" on a table], the social presence who will follow you from body to body to help you. You can say Hi to Ari whenever you are ready.

[Stagehand turns on Ari's face]

**Ari:** Hi, welcome to the DMV. My name is Ari, and I'll be assisting you here today. Let's get you checked in. What is your name?

Participant: <response>

**Ari:** Hello, Sam. What are you visiting the DMV for today?

**Participant:** <response>

**Ari:** Okay, let me guide you to the waiting room. Please head downstairs and I'll meet you there.

[Stagehand moves the speaker to the "tall robot" body. Participant goes downstairs to meet Ari, guided by the experimenter if necessary]

**Ari:** Follow me to the registration desk.

[Stagehand pushes "tall robot" to the registration desk, guiding the participant to follow if needed. Once the robot arrives at the registration desk, Stagehand turns off "tall robot"'s face, moves the speaker to "tinybot", turns on "tinybot"'s face, and moves "tall robot" to its next position].

**Ari:** [appearing on "tinybot"] Hi Sam, it's me. Please place your car title face-down on the top left corner.

[Participant inserts their car information card]

**Ari:** Sam, please review your car details and let me know if anything needs to be corrected.

## **Analysis**

We recorded and transcribed the interviews, and analyzed responses using affinity diagramming [3]. We chose affinity diagramming over grounded theory because our goal was to assess possible futures—not people's current practices—and to tease out some of the initial patterns and social mores related to re-embodiment and co-embodiment. Affinity diagramming was therefore more suitable for that goal, as it is a practice-based approach focused on drawing out themes and insights to support designing successful products that may be implemented in the future.

Three researchers iteratively rearranged clusters of post-it notes based on their emerging affinity to one another, while discussing and critiquing the emerging themes. We focused on items that did not fit with any existing clusters and items we disagreed on, working until the affinity structure of all items was resolved. All participant quotes from the interviews that were relevant to the design space were analyzed (off-topic commentary was excluded).

## **RESULTS**

Our synthesis of the data revealed several themes about the way people made sense of their experiences. The themes that emerged include: (1) participants' acceptance of reembodiment, (2) perceptions of agent expertise, (3) crossing contextual boundaries, (4) perceptions of cognitive load, and (5) negative reactions to co-embodiment.

## **Acceptance of Re-embodiment**

Previous work shows that people may experience comfort when they interact with familiar things [15]. It seemed that in this study, participants felt comfortable with the concept of re-embodiment, and rationalized their comfort by connecting the agent's behavior to familiar experiences. Some compared their experience with existing products:

P05: "It was like talking to a more intelligent Alexa, or an Alexa that had a wider range of abilities."

P17: "I'm used to... interacting with a robot that could be in different bodies. For example, one reason that I got an Apple watch was so that I would be able to give myself reminders by Siri, when I'm not near my phone or when I want to isolate myself from distractions."

Other participants used analogies of human behavior to describe and make sense of their experiences:

P09: (When the robot transitions from home to a remote workplace) "[It is] like waiting for a friend of mine who would go do something and then come back."

While participants tended to interpret the interactions in human terms, they did not act surprised or unsettled when the robots engaged in the non-human behavior of jumping from one body to the next. They did not view this as unnatural for an agent:

P18: "That's the whole point of making a virtual intelligence, is the fact that their body is not the limitation."

P01: "Even though the bodies are different, the voices, the mind, the thought process remains the same, so it's like a continuation of thoughts from one body to another."

Additionally, participants suggested that the similarity in the agents' mechanical form and their use of the same voice in

different bodies made it easier for them to perceive and accept the occurrence of re-embodiment:

P14: "It was the same voice and the bodies were so minimal and so mechanical... It was not a big deal. If you had presented me with Ari [one of the robots] who was sitting on the little table, and then something that looks humanoid, then there might be some difference."

Perhaps a more critical aspect to examine further is the exterior design of re-embodying robots, rather than the behavior of re-embodiment itself.

# **Perception of Agent Expertise**

In the DMV enactment, participants first interacted with several distinct social presences across touchpoints, each in a separate body (one-for-one). In the next variation, they interacted with a single social presence that moved from one body to another (re-embodiment). Most participants perceived re-embodiment as more seamless, easy, and efficient. Many described it as a more natural flow of interaction compared to a piecemeal interaction with multiple social presences. In the one-for-one variation, participants felt that they had to become the connective tissue across touchpoints and that they had to re-explain the task to every new social presence. Participants did not actually re-explain the task (as we designed each agent in the sequence to already have all the relevant information), but they were still left with the feeling that they had experienced re-introductions in the one-for-one robot behavior:

P12: "It's always better to have one intelligence that guides all of the five steps and [creates] a process that is one thing."

P01: "I had this feeling that if you have a single mind controlling all the bodies, the thought process and the transfer of commands could be much faster than three [social presences] doing this... If you have multiple brains acting in multiple bodies, even a slight mismanagement between the several steps can lead to a disastrous result."

P16: "Meeting you from the beginning, following you throughout the whole thing, it felt like they had all the information in store, whereas going to each new robot, I feel like they only knew that specific step of my process."

While the preference for a single social presence that could move with participants through a service was dominant, some participants wished for a different experience. For these participants, having several social presences guide them through a particular service was a the preferred choice. They explained it like an assembly line, where each social presence knows its role and has its own expertise conducive to doing the same thing over and over again. Participants who preferred this variation argued that it is more important to have a social presence with expertise take care of the task than to engender a personalized experience with the same social presence:

P02: "A lot of [social presences] probably works better because you have people come in one by one and directed downstairs. There is no delay. There is a nice, fluid [process], like an assembly line."

Some participants preferred a one-for-one social presence only for tasks that required what they perceived as a high level of expertise. This desire was expressed in the Medical Center enactment, where the social presence followed participants from home to re-embody the center's front desk, and onto the X-ray machine to take their X-rays:

P11: "[It would be better to have separate social presences] in the last scenario [medical center] because we are talking about having medical expertise in a certain area... like when you go to the X-ray room, [you want to] have a professional person [social presence] there, not [the one from] the reception area."

## Crossing Contextual Boundaries

We anticipated that participants might prefer having a single social presence follow them within a single service, as in the DMV enactment, but that a social presence that jumps between two very different contexts, such as work and home, would not be as well-received. However, participants' reactions did not confirm our hunch: many participants reacted positively to scenarios in which a single social presence crossed contexts.

# Private and Public Spheres

Participants mostly did not mind a social presence that moved between private and public spheres. Several participants liked having a single social presence follow them from their home to a hospital and then assist them in a medical context. These participants found the familiarity with the social presence to be comforting. The feeling of comfort contrasted with the stress they typically associated with visits to health providers:

P11: "I thought it was convenient that it was the same person [social presence] that you are familiar with, they already know everything about you."

P12: "You are assured that OK, you will be fine... it's better to have one guy who is dedicated to you."

Participants who disliked when a single social presence moved across contexts offered a perspective we had not considered. We anticipated that the main concern would be around privacy of information, and this was expressed by some of the participants who worried about the risk of exposing personal data in sensitive environments:

P14: "I don't necessarily want the receptionist to know what goes on in the doctor's consulting room or the X-ray room, and vice versa."

However, the strongest negative reactions seemed to be triggered by social preferences. Several participants shared concern that interacting with only one social presence over an extended period of time and across contexts might be boring and draining. They desired variety in their interaction partners:

P06: "You need different people in your life for different situations. Like your teachers... I don't want to take seven classes and listen to the same voice over and over and over and over again."

P18: "For me, I think I am more social... It makes it less lonely [to have multiple social presences] than to have one

single voice. Like, "Alexa, you're the only person I talk to and you're the only person who gets me"... I just [prefer] multiple voices, multiple people."

# Private and Professional Spheres

We found that a single social presence moving between private and professional environments raised two concerns: one about the effort required to maintain a work-life balance in a case of a re-embodying agent, and the other about the ability to keep some information private.

Participants imagined that having different social presences for different domains could potentially help them maintain a better work-life balance. They believed that it would be harder to maintain a separation when a social presence re-embodies and works across both domains. Participants also worried that cross-contextual agents could cause work-related topics to be exposed to their family or friends, and personal topics, such as embarrassing habits, to be exposed in a work environment:

P05: "I personally like a separation between my day job and my home life. So, you would worry that it would remind me of emails at work when I'm at home trying to relax. It would not have a clear filter between work and work at home."

P18: "I want a clear disconnect so that mentally I can switch back and forth from home life and work,"

P14: "Would people know what goes on in my home simply because this thing can transfer between environments?"

# **Perceived Agent Cognitive Ability**

Participants expressed concern about social presences' ability to effectively carry out several tasks at the same time across multiple bodies. Some participants suggested that a social presence might be "biting off more than it could chew"—that is, that the social presence only had so much cognitive capacity and attention to devote to tasks at a particular time, and that if it attempted to exceed its limits, system errors or other failures could occur. Current experiences with technology seem to simultaneously reinforce and defy this concern. Smartphones, for example, can maintain constant monitoring of text messages, email, social media, and news feeds while providing turn-by-turn directions. These same devices also sometimes lock up when transitioning between WiFi and phone networks. It seemed that the failures of present-day technical systems had a stronger influence on participants than their successes:

P01: "Maybe Sigma [the social presence] cannot embody two devices efficiently at the same time."

P12: "Imagine you give it like 10 other tasks which it is not supposed to do. It is forgetting the main task that it was designed for."

When the task at hand was driving, an activity that involves personal safety and risk, participants expressed an even greater deal of skepticism about the social presence's capacity to do multiple tasks at once. Many participants seemed disturbed when the "driving" social presence chose to engage in tasks unrelated to driving. The strongest responses came when the

"driving" social presence began talking to another social presence. Participants seemed to have attributed an understanding of limited human attention:

P12: "Autonomous driving intelligences should only be related to autonomous driving!"

P07: "I don't know the requirement of the capacity... focus on the safety instead of the talking."

#### Co-Embodiment

For the co-embodiment enactment, there were two social presences ("Omega", the driving agent, and "Eta", the home agent) in a single device (a car) who conversed with each other. As we only probed a single instance of co-embodiment in our enactments, additional work is needed to confirm some of the initial reactions we report below.

Although participants explicitly understood our intention for two social presences to embody the car, they still tended to intuitively interpret the situation according to remote communication between humans: they described the experience as one social presence being "inside" the car, with the other "calling in" from a different location, like a conference call:

P04: "It felt like [it] was home, calling in."

P16: "I did not think of it as having multiple minds right now in the body of the car. It definitely did not feel like that to me."

We expected that in this enactment, participants would perceive the agents as more social because they conversed with each other verbally. We found that participants did, in fact, describe these social presences in social terms in the coembodiment enactment more so than in other ones:

P06: "...it would be just like two of my best friends."

P07: "It's like they are going to marry and I will be the one who will break them up."

Social attributions manifested as more than just a social layer in the interaction. Some participants felt a social hierarchy was formed. Participants frequently described this interaction in terms of masters, servants, ethical issues, and human rights. Participants who felt that the enactment created a hierarchical social structure found it very unsettling:

P14: "[It is] like those old English manor houses where the Mrs. says I want this, and then one servant talks to the other servant and it gets done. I'm not sure I like that."

P03: "In this case, it did feel more like having servants than having just a glorified Siri. In a way that made me personally uncomfortable."

P07: "They are all my servants. So I'm the one [who] should be paid attention to, that should be acknowledged."

A surprising finding was that some participants had a strong sense of exclusion in reaction to the conversation between the two social presences. Although the conversation was only about what type of windshield wipers to purchase for the user (who had already authorized the purchase), participants were

uncomfortable with the feeling of being a "third wheel", and some even felt like they were being "plotted against":

P07: "I don't like it. I felt neglected. I was forgotten. They talked to each other. They made their own decisions without consulting me. Like I was isolated."

P14: "It's like they are colluding on me. They're ganging up on me."

P04: "Annoying... they acted like I was not even there."

Participants did not describe other experiences in the enactments in terms of social power dynamics, master-servant relationships, or social presences colluding, regardless of whether they used re-embodiment, one-for-all, or one-for-one.

Other participants reported not liking the conversing social presences simply because it was distracting and unnecessary. We had included the dialogue between social presences for the purpose of transparency, to allow users to know that information had passed from one social presence to another. Prior work has shown that users perceive silent communication between robots as creepy and undesirable [40, 41]. We therefore expected that a conversation would keep participants better informed and make them feel more in control. However, participants did not find this useful:

P01: "Eta and the other [social presence] interacted, or had a conversation in front of me. Can't this be in the background? They were already making the decision anyway."

P03: "The conversation between the car AI and the house AI seems wholly unnecessary... they do not need to express this verbally."

# DISCUSSION

Using speed dating with user enactments, we immersed participants in four situations involving potential future interactions with social robots and conversational agents. We focused on the concept of social presence flexibility, exploring four different configurations: one-for-one, one-for-all, re-embodiment, and co-embodiment.

We discuss insights from the study through key questions that emerged from the results, and that we think designers should keep in mind when devising new forms of sequential and personal interaction with multiple agents.

Should agents act human-like? Participants easily understood human-like behaviors. They often made sense of nonhuman behaviors by focusing on elements that were still similar to human behavior. For example, several participants compared a social presence that moved between a collocated and a remote body as being similar to a person who leaves and comes back. We believe this tendency is precipitated at least in part by the human-like speech that agents used, as people socialize even with task-based technology like Amazon's Alexa [37]. Thus, we were surprised to find out that some very non-human behaviors were experienced so naturally by participants. This was particularly true of re-embodiment, when a social presence traveled from one body to another. Our findings suggest that designers should not exclusively prior-

itize human behavior in designing interactions with agents. Instead, they might consider taking advantage of non-human abilities, and exploring when such abilities might add value to the interaction.

Should agents have expertise? We found an interesting interplay between efficiency in completing a task, participants' familiarity with a social presence, and social presence expertise. For most everyday and routine tasks, participants preferred to interact with a single "Jack-of-all-trades" social presence. For these low-risk contexts, people appreciated feeling that the social presence already had their information and could use it to smoothly and seamlessly accomplish all aspects of a segmented task. This was true in private, professional, and public contexts. However, when a task was more complex, had higher risk, or required a higher level of expertise, participants felt less comfortable interacting with a single social presence. For example, in the DMV enactment, most participants did not mind that the same social presence embodied the receptionist, the guide robot and the eye-checking robot. However, in the health center enactment, some participants expected to be served by experts. They felt uncomfortable that the receptionist—who in this role greeted patients, offered directions, and retrieved records—was the same social presence who took their X-rays.

This dichotomy offers the opportunity for two different kinds of social presences in interactions involving expertise: (1) A multitasking agent that is social and capable of handling many low-risk tasks, and (2) an expert agent who only has one job. Multitasking agents could provide new opportunities to design "omnichannel" and sequential services across platforms using a single social presence. For example, a user may visit a repair shop for product maintenance and find that the repairs cannot be completed because of a missing part. The user can pick up the part from another location, return home, and continue the service appointment there, where the repair shop social presence would guide them through completing the repair.

The movement of social presences across space is not limited, which allows them to keep track of many users in many contexts simultaneously. Because of this capability, agents have potential to be better at low-risk, cross-contextual interactions than humans. In addition, any service that currently has a "concierge" (or could make use of someone in a concierge position) might consider presenting the users with a single social presence as the "connective tissue" that can serve them throughout an entire experience. Expert agents, on the other hand, should be limited to the tasks on which they are experts. Since people seem to want expert agents to stick to their single task, these agents may benefit from having a behavioral design that is limited in social capabilities.

Designers should also consider that while some participants enjoyed having a single, familiar social presence that moves with them from context to context, others found it potentially lonely and exhausting. More work is needed to understand how familiarity with an agent interacts with people's understanding of expertise as they interact with an agent over an extended period of time.

How should agents express their "cognitive" ability? We found that participants were concerned with the social presences' ability to effectively manage multiple tasks at the same time. This worry was especially prevalent in the car enactment, in which social presences conversed with the participant about mundane matters (choosing a podcast to listen to, ordering new windshield wipers, etc.), while also attending to the much more precarious task of operating a vehicle. We believe that participants' concern about division of attention in high-risk situations is related to their tendency to interpret agents as human-like. Similar to expertise, designers might want to create two types of agents: those that deal with low-risk tasks across contexts, and expert (possibly less social) agents that deal with one high-risk task like driving.

An alternative option might be to reassure users by providing them with explicit feedback about where the social presence's attention is directed. For instance, if an autonomous car social presence is only driving and is not preoccupied with other tasks, making that singular focus clear using visual or auditory feedback could give people a better sense of security. The driving social presence can also try to assure the user that it can handle multiple tasks safely; it is possible that more open communication about the car's "cognitive" effort would have helped participants to better understand its technical abilities. The importance of users' perceptions of agents' cognitive abilities has been suggested by [34], and it is an area our team plans to explore in future research.

Should agents interact with each other? We found it surprising that the interaction between two social presences in the co-embodiment enactment made participants feel very uncomfortable. This theme emerged in the car enactment, in which the social presences discussed which brand of windshield wipers to purchase. We speculate that the interaction between them was perceived as external to the dyadic relationship with the user, and thus might have indicated an agent's "personal life" outside their obligations to the user. Other negative feelings evoked by this part of the scenario included exclusion and social isolation, and even a sense that the agents were plotting against the participant. Although the dialogue in other enactments implied that agents had interacted with each other (to transfer information about the user), participants did not allude to these qualms in any of the other enactments.

Our initial prediction was that participants would find the conversation between agents informative and even entertaining—but this was not the case. As we only probed one coembodiment scenario, the design of verbal communication between social presences needs additional research. In future work we would like to better understand if it was the conversation itself or some other aspect of our enactment that triggered such a broad range of negative reactions. We would also like to discern whether and how co-embodiment might lead to positive experiences in a different setting.

# CONCLUSION

In this work, we set out to probe the design space of how conversational agents and social robots may evolve to utilize non-human-like qualities to facilitate future sequential and personal interactions. We specifically explored how they might do this through social presence flexibility. Because this design space is uncharted, with no design patterns or known social mores to guide interaction designers, we believe an exploratory design research approach is the most appropriate method to examine the boundaries and challenges of this space.

We used four social presence configurations to tease out how agents should behave in sequential and personal interactions: (1) a separate social presence for each agent (*one-for-one*), (2) a single social presence that controls all bodies (*one-for-all*), (3) a single social presence that transitions from one body to another (*re-embodiment*), and (4) a social presence that can join another to co-inhabit a single body (*co-embodiment*). We created four user enactments with an overall of eight variations to allow participants to "speed-date" with combinations of the above in future scenarios, and conducted interviews to learn about their experiences, concerns, and values.

Our findings show that a human-like model for social robots and conversational agents is not always the best choice. Although agents' ability to socially communicate in multiple modalities is reminiscent of human-like behavior, there appear to be some instances in which human-agent interactions can benefit from agents diverging from human-like behavior. Our results emphasize the promise of agents that re-embody to support interaction across multiple touchpoints; surface a need for some agents to specialize and focus on a single task in which they are experts; and suggest that in some cases, agents should refrain from verbally interacting with other agents.

This work is a first attempt to understand the vast space of designing sequential and personal interaction with agents. Because of its exploratory nature, we had to frequently make design judgments about what to include and what to remove from the enactments. For example, we chose to only focus on single-user interactions, and we made careful decisions about which social presence configurations to use in each enactment. In future work, we are interested in exploring additional domains, multi-user scenarios, and other social presence configurations. We would also like to extend the research to reinforce and confirm our initial findings in a more systematic and controlled manner.

## **ACKNOWLEDGEMENTS**

We would like to thank the students who helped set-up and pilot the study: Xu Zeng, Thomas Von Davier, Ashvik Awasti, Benjamin Stone and Monica Huang. We would also like to thank our participants. This work is supported by the National Science Foundation under Grant Numbers SES 1734456. Any findings, conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.

# <span id="page-9-0"></span>**REFERENCES**

[1] Wilma A Bainbridge, Justin Hart, Elizabeth S Kim, and Brian Scassellati. 2008. The effect of presence on human-robot interaction. In *The 17th IEEE International Symposium on Robot and Human Interactive Communication (RO-MAN)*. IEEE, 701–706.

- <span id="page-10-5"></span>[2] Izak Benbasat and Weiquan Wang. 2005. Trust in and adoption of online recommendation agents. *Journal of the association for information systems* 6, 3 (2005), 4.
- <span id="page-10-22"></span>[3] Hugh Beyer and Karen Holtzblatt. 1997. Contextual Design: A Customer-Centered Approach to Systems Designs. (1997).
- <span id="page-10-4"></span>[4] Cynthia Breazeal, Cory D Kidd, Andrea Lockerd Thomaz, Guy Hoffman, and Matt Berlin. 2005. Effects of nonverbal communication on efficiency and robustness in human-robot teamwork. In *International Conference on Intelligent Robots and Systems*. IEEE/RSJ, 708–713.
- <span id="page-10-21"></span>[5] Colin Burns, Eric Dishman, William Verplank, and Bud Lassiter. 1994. Actors, hairdos & videotape-informance design. In *Conference companion on Human factors in computing systems*. ACM, 119–120.
- <span id="page-10-11"></span>[6] Justine Cassell, Joseph Sullivan, Elizabeth Churchill, and Scott Prevost. 2000. *Embodied conversational agents*. MIT press.
- <span id="page-10-0"></span>[7] Pew Research Cente. Nearly half of Americans use digital voice assistants, mostly on their smartphones.
- <span id="page-10-12"></span>[8] Ana Paula Chaves and Marco Aurelio Gerosa. 2018. Single or Multiple Conversational Agents?: An Interactional Coherence Comparison. In *Proceedings of the 2018 CHI Conference on Human Factors in Computing Systems*. ACM, 191.
- <span id="page-10-2"></span>[9] Alan Cooper, Robert Reimann, and David Cronin. 2007. *About face 3: the essentials of interaction design.* John Wiley & Sons.
- <span id="page-10-17"></span>[10] Scott Davidoff, Min Kyung Lee, Anind K Dey, and John Zimmerman. 2007. Rapidly exploring application design through speed dating. In *International Conference on Ubiquitous Computing*. Springer, 429–446.
- <span id="page-10-7"></span>[11] Munjal Desai, Kristen Stubbs, Aaron Steinfeld, and Holly Yanco. 2009. Creating trustworthy robots: Lessons and inspirations from automated systems. In *Proceedings of the AISB Convention: New Frontiers in Human-Robot Interaction*.
- <span id="page-10-13"></span>[12] Brian R Duffy, Gregory MP O'Hare, Alan N Martin, John F Bradley, and Bianca Schon. 2003. Agent chameleons: Agent minds and bodies. In 16th International Conference on Computer Animation and Social Agents. IEEE, 118–125.
- <span id="page-10-19"></span>[13] Michael Golembewski and Mark Selby. 2010. Ideation decks: A card-based design ideation tool. In Proceedings of the 8th ACM Conference on Designing Interactive Systems. ACM, 89–92.
- <span id="page-10-8"></span>[14] Peter A. Hancock, Deborah R. Billings, Kristin E. Schaefer, Jessie Y. C. Chen, Ewart de Visser, and Raja Parasuraman. 2011. A meta-analysis of factors affecting trust in Human-Robot Interaction. *Human factors* 53 5 (2011), 517–27.

- <span id="page-10-23"></span>[15] Paul Hekkert, Dirk Snelders, and Piet CW Van Wieringen. 2003. "Most advanced, yet acceptable": Typicality and novelty as joint predictors of aesthetic preference in industrial design. *British journal of Psychology* 94, 1 (2003), 111–124.
- <span id="page-10-3"></span>[16] Pamela J. Hinds, Teresa L. Roberts, and Hank Jones. 2004. Whose job is it anyway? A study of Human-Robot Interaction in a collaborative task. *Human-Computer Interaction* 19 (2004), 151–181.
- <span id="page-10-9"></span>[17] Guy Hoffman, Jodi Forlizzi, Shahar Ayal, Aaron Steinfeld, John Antanitis, Guy Hochman, Eric Hochendoner, and Justin Finkenaur. 2015. Robot presence and human honesty: Experimental evidence. In *Proceedings of the Tenth Annual ACM/IEEE International Conference on Human-Robot Interaction (HRI '15)*. ACM, New York, NY, USA, 181–188. DOI: http://dx.doi.org/10.1145/2696454.2696487
- <span id="page-10-18"></span>[18] Jibo. accessed September 13, 2018. *Jibo*. https://www.jibo.com/
- <span id="page-10-10"></span>[19] Sara Kiesler, Aaron Powers, Susan R Fussell, and Cristen Torrey. 2008. Anthropomorphic interactions with a robot and robot–like agent. *Social Cognition* 26, 2 (2008), 169–181.
- <span id="page-10-16"></span>[20] Chyon Hae Kim, Yumiko Yamazaki, Shunsuke Nagahama, and Shigeki Sugano. 2013. Recognition for psychological boundary of robot. In *Proceedings of the* 8th ACM/IEEE international conference on Human-robot interaction. IEEE Press, 161–162.
- <span id="page-10-15"></span>[21] Kheng Lee Koay, Dag Sverre Syrdal, Wan Ching Ho, and Kerstin Dautenhahn. 2016. Prototyping realistic long-term human-robot interaction for the study of agent migration. In 25th IEEE International Symposium on Robot and Human Interactive Communication (RO-MAN). IEEE, 809–816.
- <span id="page-10-14"></span>[22] Kheng Lee Koay, Dag Sverre Syrdal, Michael L. Walters, and Kerstin Dautenhahn. 2009. A user study on visualization of agent migration between two companion robots.
- <span id="page-10-1"></span>[23] Business Insider Leanna Garfield. 2016 (accessed September 20, 2018). Companies that are replacing human jobs with robots. https://www.businessinsider.com/ companies-that-use-robots-instead-of-humans-2016-2
- <span id="page-10-20"></span>[24] Dan Lockton, Devika Singh, Saloni Sabnis, Michelle Chou, Sarah Foley, and year=2019 organization=ACM, New York Pantoja, Alejandro booktitle=In Proceedings of the 2019 ACM Creativity Cognition Conference (CC âĂŸ19). New Metaphors: A Workshop Method for Generating Ideas and Reframing Problems in Design and Beyond.
- <span id="page-10-6"></span>[25] Michal Luria, Guy Hoffman, and Oren Zuckerman. 2017. Comparing social robot, screen and voice interfaces for smart-home control. In *Proceedings of the* 2017 CHI Conference on Human Factors in Computing Systems. ACM, 580–628.

- <span id="page-11-10"></span>[26] Alan Martin, Gregory MP O'hare, Brian R Duffy, Bianca Schön, and John F Bradley. 2005. Maintaining the identity of dynamically embodied agents. In *International Workshop on Intelligent Virtual Agents*. Springer, 454–465.
- <span id="page-11-0"></span>[27] Kevin Murnane. 2018 (accessed September 13, 2018). Report Claims That 16% Of Adults In The US Own Amazon's Echo Or Google's Home.
- <span id="page-11-4"></span>[28] Bilge Mutlu, Fumitaka Yamaoka, Takayuki Kanda, Hiroshi Ishiguro, and Norihiro Hagita. 2009. Nonverbal leakage in robots: Communication of intentions through seemingly unintentional behavior. In *Proceedings of the 4th ACM/IEEE international conference on Human robot interaction*. ACM, 69–76.
- <span id="page-11-1"></span>[29] Clifford Nass and Scott Brave. 2005. Wired for speech: How voice activates and advances the human-computer relationship. MIT press.
- <span id="page-11-11"></span>[30] Kohei Ogawa and Tetsuo Ono. 2008. ITACO: Effects to interactions by relationships between humans and artifacts. In *International Workshop on Intelligent Virtual Agents*. Springer, 296–307.
- <span id="page-11-7"></span>[31] Martin Porcheron, Joel E Fischer, Stuart Reeves, and Sarah Sharples. 2018. Voice interfaces in everyday life. In *Proceedings of the 2018 CHI Conference on Human Factors in Computing Systems*. ACM, 640.
- <span id="page-11-9"></span>[32] Aaron Powers, Sara Kiesler, Susan Fussell, and Cristen Torrey. 2007. Comparing a computer agent with a humanoid robot. In *Proceedings of the ACM/IEEE International Conference on Human-robot Interaction (HRI '07)*. ACM, New York, NY, USA, 145–152. DOI: http://dx.doi.org/10.1145/1228716.1228736
- <span id="page-11-6"></span>[33] Byron Reeves and Clifford Ivar Nass. 1996. *The media equation: How people treat computers, television, and new media like real people and places.* Cambridge university press.
- <span id="page-11-16"></span>[34] Samantha Reig, Jodi Forlizzi, and Aaron Steinfeld. 2019. Leveraging robot embodiment to facilitate trust and smoothness. In 2019 14th ACM/IEEE International Conference on Human-Robot Interaction (HRI). IEEE, 742–744.

- <span id="page-11-13"></span>[35] Laurel D Riek. 2012. Wizard of oz studies in hri: A systematic review and new reporting guidelines. *Journal of Human-Robot Interaction* 1 (2012), 119–136.
- <span id="page-11-8"></span>[36] Kristin E. Schaefer, Jessie Y. C. Chen, James L. Szalma, and P. A. Hancock. 2016. A meta-analysis of factors influencing the development of trust in automation: Implications for understanding autonomy in future systems. *Human Factors* 58, 3 (2016), 377–400. DOI: http://dx.doi.org/10.1177/0018720816634228
- <span id="page-11-5"></span>[37] Alex Sciuto, Arnita Saini, Jodi Forlizzi, and Jason I Hong. 2018. Hey Alexa, What's Up?: A mixed-methods studies of in-home conversational agent usage. In Proceedings of the 2018 on Designing Interactive Systems Conference 2018. ACM, 857–868.
- <span id="page-11-3"></span>[38] Anna-Maria Seeger, Jella Pfeiffer, and Armin Heinzl. 2017. When do we need a human? Anthropomorphic design and trustworthiness of conversational agents. (2017).
- <span id="page-11-12"></span>[39] Dag Sverre Syrdal, Kheng Lee Koay, Michael L Walters, and Kerstin Dautenhahn. 2009. The boy-robot should bark!-children's impressions of agent migration into diverse embodiments. In *Proceedings: New Frontiers of Human-Robot Interaction, a symposium at AISB*.
- <span id="page-11-14"></span>[40] Xiang Zhi Tan, Samantha Reig, Elizabeth J Carter, and Aaron Steinfeld. 2019. From One to Another: How Robot-Robot Interaction Affects Users' Perceptions Following a Transition Between Robots. In 2019 14th ACM/IEEE International Conference on Human-Robot Interaction (HRI). IEEE, 114–122.
- <span id="page-11-15"></span>[41] Tom Williams, Priscilla Briggs, and Matthias Scheutz. 2015. Covert Robot-robot Communication: Human Perceptions and Implications for Human-robot Interaction. *J. Hum.-Robot Interact.* 4, 2 (Sept. 2015), 24–49. DOI: http://dx.doi.org/10.5898/JHRI.4.2.Williams
- <span id="page-11-2"></span>[42] John Zimmerman and Jodi Forlizzi. 2017. Speed dating: providing a menu of possible futures. *She Ji: The Journal of Design, Economics, and Innovation* 3, 1 (2017), 30–50.