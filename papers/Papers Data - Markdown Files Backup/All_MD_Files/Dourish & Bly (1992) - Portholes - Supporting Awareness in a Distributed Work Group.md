![](_page_0_Picture_2.jpeg)

# Portholes: Supporting Awareness in a Distributed Work Group

Paul Dourish

Rank Xerox EuroPARC 61 Regent St Cambridge CB2 lAB UK . (0223) 341512 dourish@europarc. xerox .com

Sara Bly

Xerox PARC 3333 Coyote Hill Road Palo Alto, CA 94304 (415) 8124360 bly@parc.xerox.com

# ABSTRACT

We are investigating ways in which media space technologies can support distributed work groups through access to information that supports general awareness. Awareness involves knowing who is "around", what activities are cxcurring, who is talking with whom, it provides a view of one another in the daily work environments. Awareness may lead to informal interactions, spontaneous connections, and the development of shared cultures-all important aspects of maintaining working relationships which are denied to groups distributed across multiple sites.

The Portholes project, at Rank Xerox EuroPARC in Cambridge, England, and Xerox PARC in Palo Alto, California, demonstrates that awareness can be supported across distance. A data network provides a shared database of image information that is regularly updated and available at all sites. Initial experiences of the system in use at EuroPARC and PARC suggest that Portholes both supports shared awareness and helps to build a "sense of community".

KEVVVORDS: group spaces, distributed awareness. work, collaboration, CSCW, media workgroups, informal interaction,

# INTRODUCTION AND MOTIVATIONS

Reports on the use of media space technology (e.g. [3], [5], [61, [81, [101, [111) typically focus on the use of direct audio and video connections as an aid to collaboration among remotely located individuals. The emphaws on real-time connections is not suqxising; such uses are highly visible and identifiable mechanisms through which remote

Permission to copy without fee all or part of this material IS granted provided that the copies are not made or distributed for direct commercial advantage, the ACM copyright notice and the tltleof the publication and its date appear, and notice is given that copying ISby permission of the Association for Computing Machinery. To copy otherwwe, or to republish, requires a fee and/or speclflc permission,

@ 1992 ACM 0-89791-513-5/92/0005-0541 1.50

collaboration can be enhanced. However, our experiences of using media space technology at Rank Xerox EuroPARC [4] and at Xerox PARC [9] have also pointed to the importance of a different style of comection. We find that, when their video equipment is otherwise unused, many of our media space users like to observe activities in public areas; they report that they find these connections useful in order to see "what's going on" as members of the group gather for meetings, check their mail, collect coffee, etc. These background connections are used very differently from those of direct connections; in particular, they tend to be long-term and non-engaged. Unlike information which might be gleaned from a direct connection with a colleague, here it is being gathered passively, while other workplace activities progress.

This use of video technology is very similar to the typical awareness activities which occur in a shared physical environment. While sitting at a desk, we are aware of activities going on around us—we hear the sounds of conversations in corridors, see people as they pass by, notice people in offices as we walk down a hallway, and so forth. The Polyscope system at EuroPARC [2] and the hmger system at PARC were attempts to capture some of this information in the respective media spaces. The basic approach that each took was to present regularly-updated digitised video images from locations around the media space on the workstation screen. These images show activities in public areas and offices. Our media space infrastructures provide the technological base for these applications—users of the awareness services are "inhabitants" of our media spaces.

Following on from positive experiences with Polyscope and Imager, we wished to extend the notion of "awareness" outside a single physical location, and thus support awareness for distributed work groups. Such groups, by their nature, are denied the infomml information gathered from a physically shared workspace and the proxunity whtch is an important factor in collaboration between colleagues ([1], [7]). We expect that a shared awareness space can be a basis for providing similar information. In addition, awareness services can be achieved with less bandwidth than the usual "live video" connections of existing media spaces. Thus, we

![](_page_1_Figure_2.jpeg)

FIGURE 1. A window dump of the '>vc" client to Portholes. The first eight images show EuroPARC nodes; the last seven show PARC nodes. All images were taken at approximately the same time.

could explore the utility of awareness for ttuly distributed groups without large investment in a technological infrastructure.

Ours ystem for distributed awareness is called "Portholes". A multi-site awareness service tackles a number of new issues, including data distribution techniques and the interface problems of dealing with shared information. Portholes consists of a cooperating group of servers which jointly manage a distributed data space. In addition, Portholes includes clients which present the Portholes information in a variety of ways giving users the ability to process and use the information. Figure 1 shows a typical interface to Portholes with images of colleagues who share research interests and projects in both Cambridge and Palo Alto,

This paper focuses on Portholes as an example of the kind of system we think might support our notion of distributed awareness. We will describe Portholes and its existing clients, offer some initial observations of its use, and discuss issues that we consider central to developing an understanding of the role of awareness in everyday work activities and in using technologies to enable that awareness in distributed groups.

# DESIGN CONSTRAINTS AND ARCHITECTIJRE

Portholes is basically a system for maintaining image information which is both generated and consumed at a number of sites connected via an intemet. Essentially, the technical problem is timely distribution of information so that it can be usefully presented to a user, while keeping within the constraints of available network bandwidth. Since we wish to support multiple interfaces and interface styles, we make a strong distinction between the two major system components—a server component, which is responsible for maintaining the database, and one or more clienl components, which present the information to users.

#### interface Requirements

Interface requirements drive a great deal of the server design, and so it is worth considering what sorts of facilities they might provide, and hence the requirements they impose, An interfaee client of the Portholes infomlat ion base will generally be an interactive program rurming on a user's workstation. It might display not only images, but also information about the image itself (for example, when it was taken). The interface might well provide other information about the source of the image (generally a person), such as office number and e-mail address. In designing the system, we also wanted to allow the image information to be used to access other, externally-provided services (e-mail is an obvious example), and these might well involve some kind of manipulation of the image itself or its associated information. All these needs must be catered for by the server.

Again, the primary problem to be overcome is latency in transmitted information. A single interface will typically

<sup>1,</sup> Our infrastructure, of course, is based on an existing media space.In the absence of such a facility, individual Portholes nodes can be set up with separatevidea cameras and frame-grabbers. Adequate quality can be achieved with relatively inexpensive equipment.

![](_page_2_Picture_2.jpeg)

FIGURE 2. The structure of the Portholes system. Portholes consists of a number of cooperating information servers linked by a network. Client programs communicate only with their local servers, although they may display remote information. Servers use local image-processing facilities.

show information from multiple sites, and network access to remote sites will be many orders of magnitude slower than access to local information. We can tolerate a certain amount of latency; image updates may only occur every ten minutes, and so the user will not expect up-to-the-second information. However, latency must not be reflected in the *manipulation* of information in the interface, which must have good interactive response. Thus, all manipulations of image information must result in, at most, an interaction with a *local* information server, rather than with a server at the generating site, possibly thousands of miles away. The image information must be *replicated*, so that a local copy can always be made available when needed.

#### The Portholes Architecture

#### Components

The basic architecture of Portholes comprises a set of cooperating information servers, each of which has particular responsibility for a domain, typically a media space at one site. A domain contains a number of sources of regularly updated awareness information, as well as client programs which *consume* that information. Each server is responsible for distributing information generated by sources in its domain, and for ensuring that information required by client programs within that domain is at-hand. Clients access the shared information base through their closest server. Information flows between the domain servers as required by the various client programs. Client programs access the information space as if it were all located centrally; they need not even be aware that the information is not generated locally. The server, for its part, deals purely with the information distribution, and has no knowledge of the way in which information is presented by

the clients. Thus multiple, very different, client interfaces can present the same information from a single server. The relationship between clients and servers is illustrated in Figure 2.

As well as image information, a source also has a set of properties, which hold other information associated with that source. In effect, the image is only a single source property. These other properties then allow clients to perform more useful manipulations based on the awareness data. For instance, most of our clients take advantage of an "e-mail address" property which can be used to provide a user with a mechanism for sending an e-mail message to someone directly from their image in a Portholes window. We can also be more creative, for example by adding audio snippets via the property mechanism.

#### Data Flow

There are two data sets within Portholes—domain data (e.g. what domains are available, and how they can be reached) and source data (images and property information). The distribution strategy for these two sets is different, because of the way in which they are used.

Although a user will typically only look at a subset of the available source information, browsing all of the domain information is a common activity (e.g. when selecting which of the available sources to display). Therefore, while source information is transmitted only on an as-needed basis, domain data is actively propagated to all sites. This means that domain data is always immediately accessible to the user for browsing and manipulation. Delays in source data, however, can be tolerated, which helps us achieve our goal of keeping network throughput low.

Our clients make use of all these server facilities. Domain information is continually available to the user, so that it is easy to select which images will be displayed. The display space, though, is flat, with no reference made to domains; interfaces typically present images in a single "awareness space". Properties carry information which may be intended for the user directly, for processing by a client, or for interserver communication. Thus our architecture provides an efficient way of providing multiple interfaces to the awareness information.

### PRESENTING PORTHOLES INFORMATION

To date, we have been working with three clients, all of which are variations of one another. The bawc client, PVC, is an application running under the X Window System, which displays one or more of the available images, automatically updating the images every few minutes. The user can select which images are displayed using an init@lisation file or with a menu when the application is running. Another client, edison, has the capabilities of pvc and also associates digital audio messages (or "snippets") with images. It allows users to record their audio snippets and listen to those recorded by other Portholes users. Finally, a client viewmaster is provided for public use, It is like pvc but with the constraint that the only images available are public spaces; no office nodes are included.

Referring back to Figure 1, note that there are images from both EuroPARC and PARC all taken at approximately the same moment in real-time (all times are presented in the local user's timezone-the times in the figure are British Summer Time). Clicking on an image brings up a dialog box with the properties available for that image (name, phone number, etc.) and a set of action buttons. In pvc, these actions are E-MAIL and GLANCE; edison has an additional action LISTEN for those images with associated audio messages. Clicking on E.MArL causes a mail system window to open with the To: field appropriately completed with the name of the person associated with the selected image, Clickin on <sup>5</sup> GLANCE will invoke <sup>a</sup> media space glance action at EuroPARC (this feature is not implemented at PARC). Clicking on LISTEN will play the associated audio snippet.

All of the existing clients operate primarily in a broadcast mode. By broadcast, we mean that all users of the system ha~e access to all information within the system, Thus, if a user records a voice message in edison, that message may be played by all edison users. Ultimately we believe that Portholes clients will integrate both broadcast and directed information. By directed, we mean specifying particular users to be recipients of the information. Note that directed information may come from Portholes (for example, an audio snippet sent only to one recipient) or it may come as an interface to an existing directed system (such as e-mail).

# PORTHOLES IN USE

Just as we believe in an iterative process of design and development, we practice an iterative process of use as well. We begin by using our prototypes ourselves; as we understand ways in which the system can be used and as we stabilise the system itself, we expand our user base. When we feel a prototype is ready for more in-depth analysis, we employ a variety of study methods. Our goal is to reach a point at which our prototypes can be a part of an everyday working environment outside our own research labs.

We are in the early stages of using Portholes. At the time of this writing, the system has been under development for slightly more than a year, and the clients have been available on and off for the last 8-10 months. When clients are available, Portholes has seen regular use at our two sites, and we have grown to include 10 users at PARC and 12 at EuroPARC. All are members of our respective media spaces, and have office nodes comprising video cameras, momtors, microphones and speakers, In addition to the images of the offices of the users, Pofiholes also has images available from several public areas: the commons area at EuroPARC, a view out to the green behind EuroPARC (called Parker's Piece), a common area at PARC used by many of the Media Space participants, a view of the construction site for another Xerox facility near PARC, and the PARC media lab.

The Portholes users form a distributed work group. Most have met face-to-face and share research interests, and a few subgroups have on-going collaborations across the two sites. Nevertheless, despite knowing each other and having shared research interests, colleagues typically have relatively few interactions across sites, In addition, a summer student working on Portholes at PARC (who wrote the edison interface) has never met any of the EuroPARC users except through Portholes.

During the earlier development phase, we had a core user group of around 10; since then, others have asked to join, and so our user base has expanded to the 22 people mentioned above. We have noted our own observations regarding the use of Portholes over the past few months, and we have asked our users for feedback. The results indicate that Portholes appears to be playing an active role in providing a basis for distributed awareness.

#### Initial Observations

Our first informal and anecdotaJ observations have generally fallen into two categories. The first includes user-suggested modifications or enhancements to the Portholes service; for instance, colour is a frequently-requested feature. The second is user references to people and/or events that have occurred "in Portholes". It is not at all uncommon to hear a user refer to some person that he or she "saw" tcday, when in fact that person was at the remote site, and only available through Portholes. Such "sightings" are especially common when some unusual activity occurs at the other site. Some examples give a flavour of these:

<sup>2.</sup> Glance provides a one-way video connection of a few seconds' duration to a specific media space node.

- Recently a participant at PARC was spending many late nights working in his office; his presence was not only noted by EuroPARC participants but also led them to be quite aware of his dissertation progress!
- " Another late night worker at PARC was pleased to tell his local colleagues that he had watched the sun rise in England (over Parker's Piece). Similarly, a EuroPARCer says she likes to "watch the day begin" at PARC.
- Recently a EuroPARCer came in late on a Saturday, prompting a PARC Saturday worker to press E-MAIL in edison and say "I see you". The response back from EuroPARC was "It's nice to know I'm not completely alone!"
- Cross-site visits area particular source of sightings. For instance, a PARC visitor to EuroPARC was amused to notice a EuroPARC visitor to PARC using her "home" workstation to demonstrate software.
- " Our summer student at PARC, not having met his colleagues at the other site, nevertheless feels as though he "knows" some of the Portholes users thele, and recognises personal characteristics (snippets of favourite music being one form of the edison audio messages).

# User Feedback

In order to get more detailed feedback on the use of, and reactions to, our prototype Portholes system, we asked a group of fifteen users to note their usage of Portholes over a three-day period and to fill out an electronic questionnaire. The questionnaire also asked open-ended questions regarding features they liked and disliked.

We received eleven responses by electronic mail. While we do not believe we're ready to "quantify" the effects of awareness, we can observe some patterns in the typical use of Portholes.

# Basic Usage

All but one of our questionnaire respondents reported using pvc and/or edison3 at least a few times a day through the questionnaire period; e-mail and audio snippets were used only occasionally. As we would expect, there are some problems at this stage with the dependability, accessibility, and amount of information. Particular trOUbleS included:

theeratic performance and unreliable images {eg. when were these really taken?)

[that the pvc window] takes up too much space on my screen to be up continually so it's overhead to see it

lhat not much happens; the turn around for new information is so slow that I'm not 100 motivatt'd 10 use it; I'm never guaranteed of seeing much

Despite problems our group was (and is) quite positive about having the system. We've found two main modes of use using the system as a lightweight information tool and using it as a shared space or community.

# Portholes as an Information Tool

As an information tool, Portholes offers a lightweight means of finding out the availability of a colleague and in offering quick reports that are not time-urgent:

I remember seeing [a colleague] in his ojice and going down to ask him something–checking for [that colleague] over pvc is a common event.

The sense of general awareness which helps save time on wasted visits or phone calls to empty ojices. The information it provides also allows you to predict when people will be free, or certain implications for yourselj such as "[A colleague is] talking to a visitor this morning so I won't get to see him until ajler lunch."

...1 notice that [a remote colleagues's] message is an informal bug report.

#### Portholes as a Community

In providing a shared space for a community of users, Portholes offers the opportunity to see colleagues who are remote as well as those who are local. Portholes also provides a place for sharing the serious and the whimsical:

I remember seeing people arrive, and leme, people passing through others' ofices...

n remember seeing a few people at the remote site]– like [a colleague] whom Z've never met.

Z also liked [a colleague's] message where he sang happy birthday to himself..

the sense of whether people were around and seeing my j?iends; knowing who's around; feeling some connection to folks at [the remote site] (sharing a "community" with them)

[1 like the fact that pvcledison] Brings everybody together, both within [my local site] as wel/ as between the labs,

# DISCUSSION: CURRENT RESULTS AND ISSUES

Portholes is meant to provide an awareness of remote colleagues. The image information is intended to be available without necessary actions from the users; other information is intended to be available in a lightweight (without much user involvement) manner. Thus, evaluations are difficult; people are not likely to remember specific experiences, and asking them to think about them too much changes their experiences. In order to understand the system

<sup>3.</sup> Differences in hardware platforms meant that the audio facilities were not available to all users.These users had to use pvc instead of edison.

and to plan for future work, we want to consider three different issues:

- 1. the effect of awareness information in supporting a work group generally;
- 2. the ability of Portholes to provide meaningful awareness information; and
- 3. the design of interfaces to present this information usefully.

Although there is considerable attention paid to the value of work group familiarity and proximity in a shared physical space, there has been little research into support of these in a media space environment. Furthermore, there is little research on what role passive awareness itself plays in group work activity and cohesion. We have observed participants in media spaces and in Portholes routinely using these systems for background information. Developing an understanding of how this awareness information is being used in Portholes and what effect it has on the work group interactions will lead to a better understanding of its role in maintaining work group relations generally.

Secondly, the form of the Portholes awareness information should be considered in light of our evolving understanding of awareness itself. As our user observations suggested, the notion of awareness as exemplified in Portholes currently seems to provide a basis for an information tool (community access) and for a shared space (community building). We are exploring the value of other media in providing information in support of both awareness and community building. For instance, audio snippets do not provide awareness in the same sense as the automatic images; both sender and receiver must initiate explicit actions to effect the information exchange, making it neither passive nor "background". However, audio snippets do appear to contribute to the sense of community through the awareness they provide of a colleague's personality and nature, and we are interested in exploring this form of information.

Thirdly, the interfaces to systems such as Portholes will have a significant impact on how the information is used. If awareness is a passive and background notion, then the interfaces must be particularly lightweight. At the same time, if the awareness is a basis for more interactive exchanges, then the interface must provide those capabilities. We have already observed with Portholes some of the interface difficulties. Displaying more than a few images takes considerable screen real-estate making it difficult to have Portholes available for peripheral viewing while focusing on other workstation tasks<sup>4</sup>. In addition, many of the actions are still not as flexible for user control as we would like nor as natural for prompting interactions as we would hope.

The "awareness" often seems inconsequential—late night sightings, a voice message that is part of a song, dinosaurs fighting in a commons area. However, the enthusiasm with which our users take up the system suggests to us that they sense the same potential in "awareness information" as we do, and are eager to access and exploit it. Certainly, we have observed that communications among colleagues across sites has increased, especially informal, unprompted communications of a type which would not have occurred before. Four months after our initial questionnaire, some simple statistics collection in the server tells us that participants continue to be regular users of Portholes. Making information available to colleagues in a way that does not distract from the task at hand but rather adds to the sense of work group community is the use of Portholes we hone to achieve.

# **CONCLUSIONS**

Based on our experiences with the notion of awareness, we have designed, implemented, and brought into a use a prototype system to support lightweight awareness-gathering in distributed work groups. We have extended several of the notions from earlier awareness interfaces (Polyscope and Imager) to support a distributed work group, to expand the underlying system architecture, and to begin studying the use of the system in daily work activities. In looking at the feedback from our users and their patterns of usage of this system, we're pleased by the number of people who frequently use pvc and/or edison and by the ways in which they are using it.

Our user observations suggest that awareness may be a useful basis for community access (an information tool, especially for locating colleagues) and for community building (a shared space for "sightings" and personal snippets). In particular, this second usage helps maintain working relationships in a group which would otherwise have few direct interactions.

Our experiences with Portholes suggest that awareness across distance has meaning, that it can lead positively toward communications and interactions, and perhaps most importantly, that it can contribute to a shared sense of community. Furthermore, systems like Portholes show the potential for media spaces and electronic networks as environments for collaboration in low bandwidth situations. We expect the continued use, development, and evaluation of the Portholes system to contribute to a greater understanding of the nature of awareness and the support of distributed work groups.

### **ACKNOWLEDGEMENTS**

We particularly thank Amin Vahdat for implementing edison and Tom Moran, Alan Borning, and Mike Travers for helping us get started. Scott Elrod, Enrique Godreau, Scott Minneman, and Pierre Wellner contributed to making it run,

<sup>4.</sup> A full display of all available images takes almost all of a 17-inch screen, although other windows can be placed on top of it.

particularly the frame-grabbing processes. We also very much appreciate the comments from Victoria Bellotti, Francoise Brun-Cottan, Bill Gaver, Steve Harrison, Susan Irwin, Lennart Lovstrand, Allan MacLean, and Wendy Mackay on this paper. Most importantly, we thank the Portholes-Users for their willingness to explore new ideas and new technologies with enthusiasm.

# REFERENCES

- 1. Allen, T. (1977), Managing the Flow of Technology, MIT Press, Cambridge, Massachusetts.
- 2. Borning, A. and Travers, M. (1991), Two Approaches to Casual Interaction over Computer and Video Networks, Proc. CHI '91 Human Factors in Computer Systems, New Orleans, Louisiana.
- 3. Bulick, S., Abel, M., Corey, D., Schmidt, J. & Coffin, S. (1989). The US WEST Advanced Technologies Prototype Multi-media Communications System, Proc. GLOBECOM '89 Global Telecommunications Conference, Dallas, Texas.
- 4. Gaver, W., Moran, T., MacLean, A., Dourish, P., Carter, K. and Buxton, W. (1991), Working Together in Media Space: Collaboration Research at EuroPARC, Proc. UNICOM Symposium on CSCW—The Multimedia and Networking Paradigm, London.

- 5. Heath, C. & Luff, P. (1991), Disembodied conduct: Communication through video in a multi-media environment, Proc. CHI '91 Human Factom in Computing Systems, New orleans, Louisiana.
- 6. Irwin, S. (1990), Technology, Talk and the Social World: A Study of Video-Mediated Interaction. Dissertation. Michigan State University.
- 7. Kraut, R., Egido, C., and Galegher, J. ( 1988) Patterns of Contact and Communication in Scientific Research Collaboration, Proc. CSCW '88 Computer-Supported Cooperative Work, Portland, Oregon.
- 8. Mantei, M,, Backer, R., Sellen, A., Buxton, W., Milligan, T. and Wellman, B. (1991 ), Experiences in the Use of a Media Space, Prcc. CHI '91 Human Factors in Computer Systems, New Orleans, Louisiana.
- 9. Olson, M., and Bly, S. (1991) The Portland Experience: A Report On A Distributed Research Group, Intl. Journal of Man-Machine Studies, 34.
- 10. Root, R. (1988). Design of a Multi-Media Vehicle for Social Browsing, Proc. CSCW '88 Computer Support for Cooperative Work, Portland, Oregon.
- 11. Stults, R. (1988) Experimental Use of Video to Support Design Activity, Technical Report SSL-89- 19, Xerox Palo Alto Research Centre, Palo Alto, California.