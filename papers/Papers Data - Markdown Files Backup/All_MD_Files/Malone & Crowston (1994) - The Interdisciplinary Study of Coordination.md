![](_page_0_Picture_0.jpeg)

# The Interdisciplinary Study of Coordination

THOMAS W. MALONE

Center for Coordination Science, Massachusetts Institute of Technology, Cambridge, Massachusetts 02139

#### KEVIN CROWSTON

University of Michigan School of Business Admznistration

This survey characterizes an emerging research area, sometimes called coordination theory, that focuses on the interdisciplinary study of coordination. Research in this area uses and extends ideas about coordination from disciplines such as computer science, organization theory, operations research, economics, linguistics, and psychology.

A key insight of the framework presented here is that coordination can be seen as the process of managing dependencies among activities. Further progress, therefore, should be possible by characterizing different kinds of dependencies and identifying the coordination processes that can be used to manage them. A variety of processes are analyzed from this perspective, and commonalities across disciplines are identified. Processes analyzed include those for managing shared resources, *producer/consumer* relationships, simultaneity constraints, and *task/subtask* dependencies.

Section 3 summarizes ways of applying a coordination perspective in three different domains: (1) understanding the effects of information technology on human organizations and markets, (2) designing cooperative work tools, and (3) designing distributed and parallel computer systems. In the final section, elements of a research agenda in this new area are briefly outlined.

Categories and Subject Descriptors: C.0 [ComputerSystems Organization]:General —System Architectures: C.2.4 [Computer-Communication Networks]: Distributed Systems; D.4.1 [Operating Systems]:Process Management; D.4.2 [Operating Systems]:Storage Management; H.1.1 [Modelsand Principles]:System and Information Theory; H.4.1 [Information Systems Application]: Office Automation; H.4.3 [Information Systems Applications]: Communications Applications; H.5.3 [Information Interfaces and Presentation]: Group and Organization Interfaces; I.2.11 [Artificial Intelligence]: Distributed Artificial Intelligence—Coherence and Coordination; K.4.3 [Computers and Society]: Organizational Impacts

General Terms: Design, Economics, Human Factors, Management, Theory Additional Key Words and Phrases: Computer-supported cooperative work, coordination, coordination science, coordination theory, groupware

#### 1. INTRODUCTION

In recent years, there has been a growing interest in questions about how the activities of complex systems can be coordinated [Huberman 1988b; Johansen 1988; Rumelhart et al. 1986; Winograd and Flores 1986; National Science Founda-

tion 1989; 1991; Bond and Gasser 1988; Huhns and Gasser 19891. In some cases, this work has focused on coordination in parallel and distributed computer systems, in others, on coordination in human systems, and in many cases, on complex systems that include both people and computers.

Permission to copy without fee all or part of this material is granted provided that the copies are not made or distributed for direct commercial advantage, the ACM copyright notice and the title of the publication and its data appear, and notice is given that copying is by permission of the Association for Computing Machinery. To copy otherwise, or to republish, requires a fee and/or specific permission.

© 1994 ACM 0360-0300/94/0300-0087 \$03.50

#### **CONTENTS**

- 1. INTRODUCTION
  - 11 A Motivating Question
  - 1.2 How Can We Proceed?
- 2 A FRAMEWORK FOR STUDYING COORDINATION
  - 2 1 What is Coordination
  - 2 2 Basic Coordination Processes
  - 2 3 Example. Analyzing the Task Assignment Process
  - 2 4 Other Processes Needed for Coordination
- 3. APPLYING A COORDINATION PERSPECTIVE
  - 3.1 Approaches to Analyzing Coordination in Different Kinds of Systems
  - 3.2 Understanding the Effects of Information Technology on Organizations and Markets
  - 3.3 Designing Cooperative-Work Tools
  - 34 Designing Distributed and Parallel Computer Systems
  - 3.5 Summary of Applications
- 4. RESEARCH AGENDA
  - 4 1 Representing and Classifying Coordination Processes
  - 4 2 Analyzing Specific Processes
  - 4.3 Applications and Methodologies
- 5 CONCLUSIONS

APPENDIX A: PREVIOUS DEFINITIONS OF COORDINATION

APPENDIX B: RESULTS ABOUT COORDINATION

FROM SELECTED FIELDS

ACKNOWLEDGMENTS

REFERENCES

Our goal in this survey is to summarize and stimulate development of theories that can help with this work. This new research area—the interdisciplinary study of coordination—draws on a variety of different disciplines including computer science, organization theory, management science, economics, linguistics, and psychology. Many of the researchers whose efforts can contribute to and benefit from this new area are not vet aware of each other's work. Therefore, by summarizing this diverse body of work in a way that emphasizes its common themes, we hope to help define a community of interest and to suggest useful directions for future progress.

There is still no widely accepted name for this area, so we will use the term coordination theory to refer to theories about how coordination can occur in diverse kinds of systems. We use the term *theory* with some hesitation because it connotes to some people a degree of rigor and coherence that is not yet present in this field. Instead, the field today is a collection of intriguing analogies, scattered results, and partial frameworks. We use the term *theory*, however, in part to signify a provocative goal for this interdisciplinary enterprise, and we hope that the various studies reviewed will serve as steps along the path toward an emerging theory of coordination.

#### 1.1 A Motivating Question

We begin with one of the questions that coordination theory may help answer: How will the widespread use of information technology change the ways people work together? This is not the only possible focus of coordination theory, but it is a particularly timely question today for two reasons:

(1) In recent years, large numbers of people have acquired direct access to computers, primarily for individual tasks like spreadsheet analysis and word processing. These computers are now beginning to be connected to each other. Therefore, we now have, for the first time, an opportunity for vastly larger numbers of people to use computing and communications capabilities to help coordinate their work. For example, specialized new software has been developed to (a) support multiple authors working together on the same document, (b) help people display and manipulate information more effectively in face-to-face meetings, and (c) help people intelligently route and process electronic messages (see detailed references in Section 3.3).

It now appears likely that there will be a number of commercially successful products of this new type (often called "computer-supported cooperative work" or "groupware"), and to some observers these applications herald a paradigm shift in computer

usage as significant as the earlier shifts toward time sharing and personal computing. It is less clear whether the continuing development of new computer applications in this area will depend solely on trial and error and intuition or whether it will also be guided by a coherent underlying theory of how people coordinate their activities now and how they might do so differently with computer support.

(2) In the long run, the dramatic improvements in the costs and capabilities of information technologies are changing—by orders of magnitude the constraints on how certain kinds of communication and coordination can occur. At the same time, there is a pervasive feeling in businesses today that global interdependencies are becoming more critical, that the pace of change is accelerating, and that we need to create organizations that are more flexible and adaptive. Together, these changes may soon lead us across a threshold where entirely new ways of organizing human activities become desirable.

For example, new capabilities for sending information faster, less expensively, and more selectively may help create what some observers (e.g., Toffler [19701) have called "adhocracies"-rapidly changing organizations with highly decentralized networks of shifting project teams. As another example, lowering the costs of coordination between firms may encourage more market transactions (i.e., more "buying" rather than "making") and, at the same time, closer coordination across firm boundaries (such as "just-in-time" inventory management).

#### 1.2 How Can We Proceed?

If we believe that new forms of organizing are likely to become more common, how can we understand the possibilities better? What other new kinds of coordination structures will emerge in the electronically connected world of the near future? When are these new structures desirable? What is necessary for them to work well?

To some extent, we can answer these questions by observing innovative organizations as they experiment with new technologies. But to understand the experiences of these organizations, we may need to look more deeply into the fundamental constraints on how coordination can occur. And to imagine new kinds of organizational processes that no organizations have tried yet, we may need to look even further afield for ideas.

One way to do both these things—to understand fundamental constraints and to imagine new possibilities—is to look for analogies in how coordination occurs in very different kinds of systems. For example, could we learn something about tradeoffs between computing and communicating in distributed computer systems that would illuminate possibilities for coordination in human organizations? Might coordination structures analogous to those used in bee hives or ant colonies be useful for certain aspects of human organizations? And could lessons learned about coordination in human systems help understand computational or biological systems, as well?

For these possibilities to be realized, a great deal of cross-disciplinary interaction is needed. It is not enough just to believe that different systems are similar, we also need an intellectual framework for "transporting" concepts and results back and forth between the different kinds of systems.

In the remainder of this survey, we attempt to provide the beginnings of such a framework. We first define coordination in a way that emphasizes its interdisciplinary nature and then suggest an approach for studying it further. Next, we describe examples of how a coordination perspective can be applied in three domains: (1) understanding the effects of information technology on human organizations and markets, (2) designing cooperative-work tools, and (3) designing distributed and parallel computer sys-

tems. Finally, we briefly suggest elements of a research agenda for this new area.

# 2. A FRAMEWORK FOR STUDYING COORDINATION

#### 2.1 What is Coordination?

We all have an intuitive sense of what the word "coordination" means. When we attend a well-run conference, when we watch a winning basketball team, or when we see a smoothly functioning assembly line we may notice how well coordinated the actions of a group of people seem to be. Often, however, good coordination is nearly invisible, and we sometimes notice coordination most clearly when it is lacking. When we spend hours waiting on an airport runway because the airline cannot find a gate for our plane, when the hotel where we thought we had a reservation is fully booked, or when our favorite word processing program stops working in a new version of the operating system we may become very aware of the effects of poor coordination.

For many purposes, this intuitive meaning is sufficient. However, in trying to characterize a new interdisciplinary area, it is also helpful to have a more precise idea of what we mean by "coordination." Appendix A lists a number of definitions that have been suggested for this term. The diversity of these definitions illustrates the difficulty of defining coordination and also the variety of possible starting points for studying the concept. For our purposes here, however, it is useful to begin with the following simple definition:

Coordination is managing dependencies between activities.'

This definition is consistent with the simple intuition that, if there is no inter-

dependence, there is nothing to coordinate. It is also consistent with a long history in organization theory of emphasizing the importance of interdependence [Thompson 1967; Galbraith 1973; Lawrence and Lorsch 1967; Pfeffer 1978; Rockart and Short 1989; Hart and Estrin 1990; Roberts and Gargano 19891.

As the definition suggests, we believe it is helpful to use the word *coordination* in a fairly inclusive sense. For instance, it is clear that actors performing interdependent activities may have conflicting interests and that what might be called "political processes" are ways of managing them [Ciborra 1987; Williamson 1985; Schelling 1960; Kling, 1980]. Similarly, even though words like "cooperation," "collaboration," and "competition" each have their own connotations, an important part of each of them involves managing dependencies between activities.<sup>2</sup>

It should also be clear that coordination, as we have defined it, can occur in many kinds of systems: human, computational, biological, and others. For instance, questions about how people manage dependencies among their activities are central to parts of organization theory, economics, management science, sociology, social psychology, anthropology, linguistics, law, and political science. In computer systems, dependencies between different computational processes must certainly be managed, and, as numerous observers have pointed out, certain kinds of interactions among computational processes resemble interactions among people [Fox 1981; Hewitt 1986; Huberman 1988a; 1988b; Miller and Drexler 1988; Smith and Davis 19811. To give a sense of the approaches differ-

<sup>&#</sup>x27;This definition was particularly influenced by Rockart and Short [1989] and Curtis [1989]. The importance of coordination in this very general sense was perhaps first recognized by Holt [1980; 1983].

<sup>&#</sup>x27;These terms also, of course, have broader meanings. For instance, cooperation usually implies shared goals among different actors; competition usually implies that one actor's gains are another's losses; and collaboration often connotes peers working together on an intellectual endeavor. However, it is sometimes useful to consider all these terms as describing different approaches to managing dependencies among activities, that is, as different forms of coordination.

Table 1. Examples of Common Dependencies between Activities and Alternative Coordination Processes for Managing Them (Indentations in the left column indicate more specialized versions of general dependency types)

| Dependency                      | Examples of coordination processes for managing dependency                                  |
|---------------------------------|---------------------------------------------------------------------------------------------|
| Shared resources                | "First come/first serve", priority order, budgets, managerial decision, market-like bidding |
| Task assignments                | (same as for "Shared resources")                                                            |
| Producer/consumer relationships |                                                                                             |
| Prerequisite constraints        | Notification, sequencing, tracking                                                          |
| Transfer                        | Inventory management (e.g., "Just In Time", "Economic Order Quantity")                      |
| Usability                       | Standardization, ask users, participatory design                                            |
| Design for manufacturability    | Concurrent engineering                                                                      |
| Simultaneity constraints        | [Scheduling, synchronization                                                                |
| Task / subtask                  | Goal selection, task decomposition                                                          |

ent fields have taken to studying coordination, we summarize in Appendix B examples of results about coordination from computer science, organization theory, economics, and biology.

Even though we believe there are more similarities among these different kinds of systems than most people appreciate, there are obviously many differences as well. One of the most important differences is that issues of incentives, motivations, and emotions are usually of much more concern in human systems than in other kinds of systems. In computer programs, for example, the incentives of a program module are usually easy to describe and completely controlled by a programmer. In human systems, on the other hand, the motivations, incentives, and emotions of people are often extremely complex, and understanding them is usually an important part of coordination. Even in human systems, however, analogies with other kinds of systems may help us understand fundamental constraints on coordination and imagine new kinds of organizations that might be especially motivational for people.

# 2.2 Basic Coordination Processes

A primary vehicle for facilitating transfer among these different disciplines is to identify and study the basic *processes* involved in coordination. Are there fundamental coordination processes that occur in all coordinated systems? If so, how can we represent and analyze these processes? Is it possible to characterize situations in a way that helps generate and choose appropriate coordination mechanisms for them?

One of the advantages of the definition we have used for coordination is that it suggests a direction for addressing these questions. If coordination is defined as managing dependencies, then further progress should be possible by characterizing different kinds of dependencies and identifying the coordination processes that can be used to manage them.

Table 1 suggests the beginnings of such an analysis (see Malone et al. [1993] for

more details). For example, one possible kind of dependency among different activities is that they require the same (limited) resources. The table shows that shared-resource constraints can be managed by a variety of coordination processes such as "first come/first serve," priority order, budgets, managerial decision, and market-like bidding. If three job shop workers need to use the same machine, for instance, they could use a simple "first come/first serve" mechanism. Alternatively, they could use a form of budgeting with each worker having preassigned time slots, or a manager could explicitly decide what to do whenever two workers wanted to use the machine at the same time. In some cases, they might even want to "bid" for use of the machine and the person willing to pay the most would get it.

The lists of dependencies and coordination processes in Table 1 are by no means intended to be exhaustive. It is important to note, however, that many specific processes that arise in particular kinds of systems (such as "design for manufacturability") can be seen as instances of more generic processes (such as managing "usability" constraints between adjacent steps in a process).

In fact, we believe that one of the most intriguing possibilities for coordination theory is to identify and systematically analyze a wide variety of dependencies and their associated coordination processes. Such a "handbook" of coordination processes could not only facilitate interdisciplinary transfer of knowledge about coordination, it could also provide a guide for analyzing the coordination needs in particular situations and generating alternative ways of fulfilling them (see Malone et al. [1993]).

One question that arises immediately is how to categorize these dependencies and coordination processes. Table 1 provides a start in this direction. Crowston [1991] suggests a more structured taxonomy based on all the possible relationships between "tasks" and "resources."

To illustrate the possibilities for analyzing coordination processes, we will

discuss in the remainder of this section the coordination processes listed in Table 1 and how they have been analyzed in different disciplines.

### 2.2.1 Managing Shared Resources

Whenever multiple activities share some limited resource (e.g., money, storage space, or an actor's time), a resource allocation process is needed to manage the interdependencies among these activities. Resource allocation is perhaps the most widely studied of all coordination processes. For example, it has received significant attention in economics, organization theory, and computer science

**Economics.** Much of economics is devoted to studying resource allocation processes, especially those involving market-like pricing and bidding mechanisms. As economists have observed, for instance, markets have a number of interesting properties as resource allocation mechanisms [Simon 1981]. For one thing, they can be very decentralized: many independent decision makers interacting with each other locally can produce a globally coherent allocation of resources without any centralized controller (e.g., Smith [1776]). For another thing, markets have a built-in set of incentiues: when all participants in a perfect market try to maximize their own individual benefits, the overall allocation of resources is (in a certain sense) globally "optimal" (e.g., Debreu [1959]).

Organization Theory. Organization theory has also paid great attention to resource allocation issues. For instance, control of resources is intimately connected with personal and organizational power: those who control resources have power and vice versa [Pfeffer and Salancik 19781. In general, organization theorists emphasize hierarchical resource allocation methods where managers at each level decide how the resources they control will be allocated among the people who report to them [Burton and Obel 1980a; 1980b]. In prac-

tice, however, resource allocation in organizations is much more complex than a simple hierarchical model suggests. For instance, managers may try to increase their own power by attracting resources (e.g., employees and money) away from other possible activities [Barnard 19641 or by using their resources in a way that is very suboptimal from the point of view of the whole organization.

How can we choose among different resource allocation methods? Recent work in transaction cost theory addresses part of this question by analyzing the conditions under which a hierarchy is a better way of coordinating multiple actors than a market [Williamson 1975; 19851. For example, if there are extra costs associated with a market transaction (such as extensive legal and accounting work), then the costs of internal transactions within a hierarchical firm may be lower and therefore preferable. A related question involves the conditions under which it is desirable to use market-like resource allocation mechanisms (such as transfer pricing) within a hierarchical organization [Eccles 19851.

Computer Science. Resource allocation issues also arise in computer systems, and much work has been done on these topics [Cytron 1987; Halstead 19851. For instance, operating systems require algorithms for allocating resources—such as processors and memory —to different processes and for scheduling accesses to input/output devices, such as disks [Deitel 19831. As we will see below, there have also already been examples of cross-fertilization of ideas about resource allocation between computer science and other fields. For example, in Section 2.3.3, we will see how ideas about distributed computer systems helped understand the evolution of human organizations, and in Section 3.4, we will see how analogies with human markets have generated novel resource allocation schemes for computer systems.

**Task Assignment.** One very important special case of resource allocation is task assignment, that is, allocating the

scarce time of actors to the tasks they will perform. An insight of the approach we are taking here, therefore, is that all the resource allocation methods listed in Table 1 are potentially applicable for task assignment, too.

For instance, in trying to imagine new coordination processes in a human organization, one might consider whether any given situation requiring task assignment could be better managed by managerial decision, by prior assignment according to task type, or by a pricing mechanism. To illustrate the surprising ideas this might lead to, consider Turoff's [1983] suggestion that employees within a large organization should be able to "bid" for the internal projects on which they wish to work and that teams could be selected using these bids. There are obviously many factors to consider in determining whether such an arrangement would be desirable in a particular situation, but it is interesting to note that one potential disadvantage — the significantly greater communication required would be much less important in a world with extensive computer networks.

# 2.2.2 Managing Producer / Consumer Relationships

Another extremely common kind of relationship between activities is a "producer/consumer" relationship, that is, a situation where one activity produces something that is used by another activity. This relationship clearly occurs in all physical manufacturing processes, for instance, where the output of one step on an assembly line is the input to the next. It also occurs with information whenever one person in an organization uses information from another or when one part of a computer program uses information produced by another.

Producer/consumer relationships often lead to several kinds of dependencies:

(1) Prerequisite constraints: A very common dependency between a "producer" activity and a "consumer" activity is that the producer activity

must be completed before the consumer activity can begin. When this dependency exists, there must at least be some *notification* process to indicate to the consumer activity that it can begin. For instance, when an automobile designer delivers a completed drawing of a part to the engineer who will design the manufacturing process for that part, the arrival of the drawing in the engineer's in-box "notifies" the engineer that her activity can begin.

Managing prerequisite dependencies also often involves explicit sequencing and tracking processes to be sure that producer activities have been completed before their results are needed. For instance, techniques from operations research, such as PERT charts and critical-path methods, are often used in human organizations to help schedule large projects with multiple activities and complex prerequisite structures. These and other project-tracking systems are also often used by managers to identify activities that are late and then use their authority to "motivate" the people responsible for the late tasks.

What alternatives can we imagine for managing this dependency? One possibility would be computer-based tracking systems that made it easy for everyone in the project to see status information about all the other activities and their dependencies. In this case, late tasks could be visible to everyone throughout the project, and "authoritarian" motivation by managers might become less important.

Sequencing problems arise frequently in computer systems, as well. For instance, one of the key issues in taking advantage of parallel processing computers is determining which activities can be done in parallel and which ones must wait for the completion of others [Arvind and Culler 1986; Holt 1988; Peterson 1977; 19811. Some of these ideas from com-

- puter science have also been used to help streamline processes in human organizations by taking advantage of their latent parallelism [Ellis et al. 1979].
- (2) Transfer: When one activity produces something that is used by another activity, the thing produced must be transferred from the "producer" activity to the "consumer" activity. Managing this dependency usually involves physical transportation. In this sense, physical transportation can be considered a coordination activity, since it involves managing a dependency between a "producer" activity and a "consumer" activity. When the thing transferred is information, we usually call the transfer "communication", rather than transportation.

In addition to simply transporting things, managing the transfer dependency also often involves storing things being transferred from one activity to another. For instance, one way of managing this aspect of the transfer dependency is to carefully control the timing of both activities so that items are delivered "just in time" to be used, and no storage is needed. This technique, for example, is becoming increasingly common in manufacturing environments [Schonberger 1982; 19861. A more common approach is to maintain an *inventory* of finished items, ready for the second activity to use, as a buffer between the two activities. Operations researchers, for instance, have developed techniques for determining at what stock levels and by how much to replenish an inventory in order to minimize costs (e.g., the "economic order quantity" [McClain et al. 19921).

Managing this dependency is also important in certain parts of computer science. For example, in parallel processing systems the rate of execution of processes must sometimes be regulated to ensure that the producer does not overwhelm the consumer or vice versa [Arvind et al.

19861. As our framework would suggest, a common approach to this problem is to place a buffer between the two processes and allocate space in the buffer to one process or the other. Network protocols manage similar problems between communicating processes that do not share any memory [Tannenbaum 19811.

(3) Usability: Another, somewhat less obvious, dependency that must often be managed in a producer/consumer relationship is that whatever is produced should be usable by the activity that receives it. One common way of managing this dependency is by standardization, creating uniformly interchangeable outputs in a form that users already expect. This is the approach on assembly lines, for example. Another approach is to ask users what characteristics they want. For instance, in human organizations this might be done by market research techniques such as surveys and focus groups [Kinnear and Taylor 19911.

A third, related, alternative is participatory design, that is, having the users of a product actively participate in its design [Schuler and Namioka 19931. This is a widely advocated approach to designing computer systems, for example, and it is interesting to note that the increasingly common practice of "concurrent engineering" [Carter and Baker 19911 can also be viewed as a kind of "participatory design." In concurrent engineering, people who design a product do not simply hand the design "over the transom" to those who design its manufacturing process. Instead, they work together concurrently to create designs that can be manufactured more easily.

In computer systems, the usability dependency occurs whenever one part of a system must use information produced by another. In general, this dependency is managed by designing various kinds of interchange languages and other standards.

#### 2.2.3 Managing Simultaneity Constraints

Another common kind of dependency among activities is that they need to occur at the same time (or cannot occur at the same time). Whenever people schedule meetings, for instance, they must satisfy this constraint.

Another example of this constraint occurs in the design of computer systems in which multiple processes (i.e., instruction streams) can be executed simultaneously. (These systems may have multiple processors or a single processor which is shared among the processes.) In general, the instructions of the different processes can be executed in any order. Permitting this indeterminacy improves the performance of the system (e.g., one process can be executed while another waits for data to be input) but can cause problems when the processes must share data or resources. System designers must therefore provide mechanisms that restrict the possible orderings of the instructions by synchronizing the processes (that is, ensuring that particular instructions from different streams are executed at the same time) [Dubois et al. 1988].

Synchronization primitives can be used to control sharing of data between a producer and consumer process to ensure that all data are used exactly once (the *producer/consumer* problem) or to prevent simultaneous writes to a shared data item (the *mutual exclusion* problem). For example, if two processes simultaneously read and then update the same data (adding a deposit to an account balance, say), one process might overwrite the value stored by the other.

One example of interdisciplinary transfer involving this concept is the work of Singh and Rein [1992] in using computer science concepts about synchronized interactions to model processes in human organizations.

### 2.2.4 Managing Task / Subtask Dependencies

**Top-Down Goal Decomposition.** A common kind of dependency among activities is that a group of activities are all "subtasks" for achieving some overall

goal. As we discuss in more detail below, there is a sense in which some overall evaluation criteria or "goals" are necessarily implied by the definition of coordination. The most commonly analyzed case of managing this dependency occurs when an individual or group decides to pursue a goal and then decomposes this goal into activities (or subgoals) which together will achieve the original goal. In this case, we call the process of choosing the goal *goal selection* and the process of choosing the activities *goal decomposition*.

For example, the strategic-planning process in human organizations is often viewed as involving this kind of goal selection and goal decomposition process. Furthermore, an important role for all managers in a traditionally conceived hierarchy is to decompose the goals they are given into tasks that they can, in turn, delegate to people who work for them. There are, in general, many ways a given goal can be broken into pieces, and a long-standing topic in organization theory involves analyzing different possible decompositions such as by function, by product, by customer, and by geographical region [Mintzberg 19791. Some of these different goal decompositions for human organizations are analogous to ways computer systems can be structured [Malone and Smith 1988].

In computer systems, we usually think of the goals as being predetermined, but an important problem involves how to break these goals into activities that can be performed separately. In a sense, for example, the essence of all computer programming is to decompose goals into elementary activities. For instance, programming techniques such as subroutine calls, modular programming, object-oriented programming, and so forth can all be thought of as techniques for structuring the process of goal decomposition [Liskov and Guttag 19861. In these cases the goal decomposition is performed by a human programmer. Another example of goal decomposition in computer systems is provided by work on planning in artificial intelligence [Chapman 1987; Fikes and Nilsson 1971; Allen et al. 19901. In

this case, goals are decomposed by a planning program into a sequence of elementary activities, based on knowledge of the elementary activities available, their prerequisites, and their effects.

In some cases, techniques for goal decomposition used in computer systems may suggest new ways of structuring human organizations. For example, Moses [1990] suggests that human organizations might sometimes be better off not as strict hierarchies but as multilayered structures in which any actor at one level could direct the activities of any actor at the next level down. This multilayered structure is analogous to successive layers of languages or "virtual machines" in a computer system (see Malone [1990]).

# Bottom-Up Goal Identification.

Even though the most commonly analyzed cases of coordination involve a sequential process of goal selection and then goal decomposition, the steps do not necessarily happen in this order. Another possibility, for instance, is that several actors realize that the things they are already doing (with small additions) could work together to achieve a new goal. For example, the creation of a new interdisciplinary research group may have this character. In human systems, this "bottom-up" process of goal selection can often engender more commitment from the actors involved than a top-down assignment of responsibility.

#### 2.2.5 Managing Other Dependencies

As noted above, the dependencies discussed so far are only a suggestive list of common dependencies. We believe there are many more dependencies to be identified and analyzed. For instance, when two divisions of a company both deal with the same customer, there is a *shared-reputation* dependency between their activities: what one division does affects the customer's perception of the company as a whole, including the other division. As another example, when several people in the same office want to buy a new rug, a key problem is not how to *allocate* the

*Coordination process* Computer Science Economics and Operations Organization Theory Research Managing shared resources techniques for processor analyses of markets and analyses of different (including task assignments) scheduling and memory other resource allocation organizational structures: mechanisms: scheduling allocation budgeting processes, algorithms and other organizational power, and optimization techniques resource dependence Managing producer / consumer data flow and Petri net PERT charts, critical path Participatory design: relationships (including analyses methods: scheduling market research prerequisites and usability techniques constraints) synchronization scheduling techniques meeting scheduling; Managing simultaneity constraints techniques, mutual certain kinds of process modeling exclusion Managing task / subtask modularization economies of scale and strategic planning; relationship techniques in management by programming; planning objectives; methods of in artificial intelligence grouping people into units

Table 2. Examples of How Different Disciplines Have Analyzed Coordination Processes

rug, but what color or other *characteristics* it should have. We might call this, therefore, a *shared-characteristics* dependency.

More generally, there are many types of dependencies between objects in the world that are managed by coordination processes. For instance, an important part of managing the design of complex manufactured products involves managing the dependencies among different subcomponents. At first glance, our definition of coordination (as managing dependencies among activities) might appear to omit dependencies among objects that are not activities. We believe, however, that this focus has the advantage of greatly simplifying the analysis of a coordinated situation. In fact, it appears that all dependencies that require coordination can be treated this way. For example, dependencies among components matter because they, explicitly or implicitly, affect the performance of some activities (e.g., designing or redesigning the components), and they can, therefore, be viewed as a source of dependencies among those activities.

In general, as these examples illustrate, there may be many ways of describing different dependencies, coordination processes, and their relationships to each other [Crowston 1991]. We believe that there are many opportunities for further work along these lines.

# 2.2.6 Summary of Basic Coordination Processes

Table 2 loosely summarizes our discussion so far by listing examples of how common coordination processes have been analyzed in different disciplines. The key point of this table, and indeed of much of our discussion, is that the concepts of coordination theory can help identify similarities among concepts and results in different disciplines. These similarities, in turn, suggest how ideas can be transported back and forth across disciplinary boundaries and where opportunities exist to develop even deeper analyses.

# 2.3 Example: Analyzing the Task Assignment Process

So far, the examples we have described have mostly involved a single field or analogies that have been transported from one discipline to another. To illustrate the possibilities for developing abstract theories of coordination that can apply simultaneously to many different kinds of systems, let us consider the task assignment process as analyzed by Malone and Smith [Malone 1987; Malone and Smith 19881; also see related work by Baligh and Richartz [1967] and Burton and Obel [1980a]. As we have described in more detail elsewhere [Malone 1992], these analyses illustrate the kind of interdisciplinary interaction that our search for coordination theory encourages: the models grew originally out of designing distributed computer systems; they drew on results from operations research; and they led eventually to new insights about the evolution of human organizations.

# 2.3.1 A Generic Task Assignment Problem

Consider the following task assignment problem. A system is producing a set of "products," each of which requires a set of "tasks" to be performed. The tasks are of various types, and each type of task can only be performed by "server" actors specialized for that kind of task. Furthermore, the specific tasks to be performed cannot be predicted in advance; they only become known during the course of the process and then only to actors we will call "clients." This description of the task assignment problem is certainly not universally applicable, but it is an abstract description that can be applied to many common task assignment situations. For instance, the tasks might be (1) designing, manufacturing, and marketing different kinds of automobiles or (2) processing steps in different jobs on a computer network.

# 2.3.2 Possible Coordination Mechanisms

One (highly centralized) possibility for solving this task assignment problem is

for all the clients and servers to send all their information to a central decision maker who decides which servers will perform which tasks and then notifies them accordingly. Another (highly decentralized) possibility is suggested by the competitive-bidding scheme for computer networks formalized by Smith and Davis [1981]. In this scheme, a client first broadcasts an announcement message to all potential servers. This message includes a description of the activity to be performed and the qualifications required. The potential servers then use this information to decide whether to submit a bid on the action. If they decide to bid, their bid message includes a description of their qualifications and their availability for performing the action. The client uses these bid messages to decide which server should perform the activity and then sends an award message to notify the server that is selected.

Malone [1987] and Malone and Smith [1988] analyzed several alternative coordination mechanisms like these, each of which is analogous to a mechanism used in human organizations. In particular, they developed formal models to represent various forms of markets (centralized and decentralized) and various forms of hierarchies (based on products or functions). Then they used techniques from queuing theory and probability theory to analyze tradeoffs among these structures in terms of production costs, coordination costs, and vulnerability costs. For instance, they showed that the centralized schemes had lower coordination costs, but were more vulnerable to processor failures. Decentralized markets, on the other hand, were much less vulnerable to processor failures but had high coordination costs. And decentralized hierarchies ("product hierarchies") had low coordination costs, but they had unused processor capacity which led to high production costs.

# 2.3.3 Applying these Models to Various Kinds of Systems

Even though these models omit many important aspects of human organiza-

tions and computer systems, they help illuminate a surprisingly wide range of phenomena. For instance, as Malone and Smith [1988] show, the models are consistent with a number of previous theories about human organizational design [March and Simon 1958; Galbraith 1973; Williamson 19851 and with major historical changes in the organizational forms of both human organizations [Chandler 1962; 19771 and computer systems. These models also help analyze design alternatives for distributed scheduling mechanisms in computer systems, and they suggest ways of analyzing the structural changes associated with introducing new information technology into organizations (Section 3.2 of this survey) [Crowston et al. 1987; Malone and Smith 19881.

# 2.4 Other Processes Needed for Coordination

In addition to the processes described above for managing specific dependencies, two other processes deserve specific attention: group decision making and communication. It is sometimes possible to analyze these processes as ways of managing specific dependencies. For instance, communication can be viewed as a way of managing producer/consumer relationships for information. However, because of the importance of these two processes in almost all instances of coordination, we describe them separately here.

## 2.4.1 Group Decision Making

Many coordination processes require making decisions that affect the activities of a group. For instance, in sharing resources a group must somehow "decide" how to allocate the resources; in managing task/subtask dependencies, a group must "decide" how to segment tasks. In all these cases, the alternative ways of making group decisions give rise to alternative coordination processes. For example, any group decision can, in principle, be made by authority (e.g., a "manager" decides), by voting, or by consensus (resulting from negotiation).

Because of the importance of group decision making in coordination, answers to questions about group decision making [Simon 1976; Arrow 1951] will be important for developing coordination theory. For instance, what are the decision-making biases in groups [Janis and Mann 19771 as opposed to individuals [Kahneman and Tversky 1973]? How do computer-based group decision-making tools affect these processes [Kraemer and King 1988; Dennis et al. 1988; Kiesler et al. 1984]? Can we determine optimal ways of allocating tasks and sharing information for making group decisions [Miao et al. 1992]? How do (or should) decisionmaking processes change in situations where both rapid response and high reliability are required [Roberts et al. 1994].

#### 2.4.2 Communication

As with decision making, there is already a great deal of theory about communication, both from a technical point of view [Shannon and Weaver 1949] and from an organizational point of view [Allen 1977; Rogers and Agarwala-Rogers 1976; Weick 19691. One obvious way of generating new coordination processes, for example, is by considering alternative forms of communication (synchronous versus asynchronous, paper versus electronic) for all the places in a process where information needs to be transferred.

A coordination framework also highlights new aspects of these problems. For example, when we view communication as a way of managing producer/consumer relationships for information, we may be concerned about how to make the information "usable." How, for instance, can actors establish common languages that allow them to communicate in the first place? This question of developing standards for communication is of crucial concern in designing computer networks in general [Dertouzos 19911 and cooperative-work tools in particular [Lee and Malone 19901. The process by which standards are developed is also of concern to economists, philosophers, and

others [Farrell and Saloner 1985; Hirsch 1987].

A related set of questions arises when we are concerned about how a group of actors can come to have "common knowledge"; that is, they all know something, and they also all know *that* they all know it. There is a growing literature about this and related questions in fields as diverse as computer science, economics, and linguistics [Halpern 1987; Aumann 1976; Milgrom 1981; Gray 1978; Cohen and Levesque 1991; Shoham 19941.

# 3. APPLYING A COORDINATION PERSPECTIVE

## 3.1 Approaches to Analyzing Coordination in Different Kinds of Systems

Any scientific theory (indeed, any statement about the world) must neglect some things, in order to focus on others. For example, Kling [1980] describes how different perspectives (such as rational, structural, and political) on the use of information systems in organizations each illuminate aspects of reality neglected by the others. In some situations, one or another of these perspectives may be most important, and all of them are involved to some degree in any real situation. In applying coordination theory to any particular system, therefore, it may be necessary to consider many other factors as well.

For instance, in designing a new computer system to help people coordinate their work, "details" about screen layout and response time may sometimes be as important as the basic functionality of the system, and the reputation of the manager who introduces the system in a particular organization may have more effect on the motivation of people to use it in that organization than any incentive structures designed into the system. Similarly, in designing a distributed computer system, the failure rates for different kinds of communications media and processors may be the primary design consideration, overwhelming any other considerations about how tasks are allocated among processors.

# 3.1.1 Parametric Analysis **Versus**Baseline Analysis

There are at least two ways an interdisciplinary theory can help deal with differences like these among systems: (1) parametric analysis and (2) baseline analysis.

Parametric Analysis. In parametric analysis, the abstract theories include parameters which may be different for different kinds of systems. For instance, the principles of aerodynamics apply to both birds and airplanes, even though parameters such as size, weight, and energy expenditure are very different in the two kinds of systems. Similarly, abstract models of coordination may include parameters for things like incentives, cognitive capacities, and communication costs, which are very different in human, computational, and biological systems. Examples of models that have been applied to more than one kind of system in this way are summarized in Sections 2.3 and 3.4.2.

Baseline Analysis. In baseline analysis, one theory is used as a baseline for comparison to the actual behavior of a system, and deviations from the baseline are then explained with other theories. For example, in behavioral decision theory (e.g., Kahneman and Tversky [1973]), mathematical decision theory is used to analyze the ways people actually make decisions. In the cases where people depart from the prescriptions of the normative mathematical theory, new theories are developed to explain the differences. Even though the original mathematical theory does not completely explain people's actual behavior, the anomalies explained by the new theories could not even have been recognized without a baseline theory for comparison. This suggests that an important part of coordination theory will be behauorial coordination theory in which careful observations of actual coordination in human systems

are used to develop, test, and augment abstract models of coordination

# 3.1.2 Identifying the Components of Coordination in a Situation

In order to analyze a situation in terms of coordination, it is sometimes important to explicitly identify the components of coordination in that situation. According to our definition of coordination above, coordination means "managing dependencies between activities." Therefore, since activities must, in some sense, be performed by "actors," the definition implies that all instances of coordination include actors performing activities that are interdependent.3 It is also often useful to identify evaluation criteria for judging how well the dependencies are being "managed." For example, we can often identify some overall "goals" of the activity (such as producing automobiles or printing a report) and other dimensions for evaluating how well those goals are being met (such as minimizing time or costs). Some coordination processes may be faster or more accurate than others, for instance, and the costs of more coordination are by no means always worthwhile.

It is important to realize that there is no single "right" way to identify these components of coordination in a situation. For instance, we may sometimes analyze everything that happens in a manufacturing division as one "activity," while at other times, we may want to analyze each station on an assembly line as a separate "activity." As another example, when we talk about muscular coordination, we implicitly regard different parts of the same person's body as separate "actors" performing separate "activities."

**Conflicting Goals.** One important case of identifying evaluation criteria occurs when there are conflicting goals in a

situation. In analyzing coordination in human organizations, it is often useful to simply ask people what their goals are and evaluate their behavior in terms of these criteria. However, some amount of goal conflict is nearly always present [Ciborra 1987; Williamson 1985; Schelling 19601, and people may be unable or unwilling to accurately report their goals, anyway. To understand these situations, it is often useful to both try to identify the conflicting goals and to analyze the behavior of the system in terms of some overall evaluation criteria. For instance, different groups in a company may compete for resources and people, but this very competition may contribute to the company's overall ability to produce useful products [Kidder 19811.

Another important example of conflicting goals occurs in market transactions. As we saw above, all participants in a market might have the goal of maximizing their own individual benefits, but we, as observers, can evaluate the market as a coordination mechanism in terms of how well it satisfies overall criteria such as maximizing consumer utilities [Debreu 19591 or "fairly" distributing economic resources.

### 3.1.3 Preview of Examples

In the remainder of this section, we describe examples of how concepts about coordination have been applied in three different areas: (1) understanding the new possibilities for human organizations and markets provided by information technology, (2) designing cooperative-work tools, and (3) designing distributed and parallel computer systems. The early examples use very general notions of coordination; the later ones are more explicit in their identification of specific components of coordination

This list is not intended to be a comprehensive list of all ways that theories of coordination could be applied. In fact, most of the work we describe here did not explicitly use the term "coordination theory." We have chosen examples, how-

<sup>&</sup>lt;sup>3</sup>See Baligh and Burton [1981], Baligh [1986], Barnard [1964], Malone [1987], Malone and Smith [19881, McGrath [1984], and Mintzberg [19791 for related decompositions of coordination.

ever, to illustrate the wide range of applications for interdisciplinary theories about coordination.

## 3.2 Understandingthe Effects of Information Technology on Organizations and Markets

Managers, organization theorists, and others have long been interested in how the widespread use of information technology (IT) may change the ways human organizations and markets will be structured [Leavitt and Whisler 1958; Simon 19761. One of the most important contributions of coordination theory may be to help understand these possibilities better.

To illustrate how the explicit study of coordination might help with this endeavor, we begin with a very general argument that does not depend on any of the detailed analyses of coordination we have seen so far in this survey.<sup>4</sup> Instead, this argument starts with the simple observation that coordination is itself an activity that has costs. Even though there are many other forces that may affect the way coordination is performed in organizations and markets (e.g., global competition, national culture, government regulation, and interest rates), one important factor is clearly its cost, and that is the focus of this argument. In particular, it seems quite plausible to assume that information technology is likely to significantly reduce the costs of certain kinds of coordination [Crawford

Now, using some elementary ideas from microeconomics about substitution and elasticity of demand, we can make some simple predictions about the possible effects of reducing coordination costs. It is useful to illustrate these effects by analogy with similar changes in the costs of transportation induced by the introduction of trains and automobiles:

- (1) A "first-order" effect of reducing transportation costs with trains and automobiles was simply some substitution of the new transportation technologies for the old: people began to ride on trains more and in horse-drawn carriages less.
- (2) A "second-order" effect of reducing transportation costs was to increase the amount of transportation used: people began to travel more when this could be done more cheaply and conveniently in trains than on foot.
- (3) Finally, a "third-order" effect was to allow the creation of more "transportation-intensive" structures: people eventually began to live in distant suburbs and use shopping malls—both examples of new structures that depended on the widespread availability of cheap and convenient transportation.

Similarly, we can expect several effects from using new information technologies to reduce the costs of coordination:

- (1) A "first-order" effect of reducing coordination costs with information technology may be to substitute information technology for some human coordination. For instance, many banks and insurance companies have substituted automated systems for large numbers of human clerks in their back offices. It has also long been commonplace to predict that computers will lead to the demise of middle management because the communication tasks performed by middle managers could be performed less expensively by computers [Leavitt and Whisler 1958]. This prediction was not fulfilled for several decades after it was made, but many people believe that it finally began to happen with large numbers of middle management layoffs in the 1980s and 1990s.
- (2) A "second-order" effect of reducing coordination costs may be to increase the overall amount of coordination used. In some cases, this may over-

<sup>&</sup>lt;sup>4</sup>See Malone [1992] and Malone and Rockart [1991] for more detailed versions of the argument in this section

whelm the first-order effect. For instance, in one case we studied, a computerized conferencing system was used to help remove a layer of middle managers (see Crowston et al. [1987]). Several years later, however, almost the same number of new positions (for different people at the same grade level) had been created for staff specialists in the corporate staff group, many of whom were helping to develop new computer systems. One interpretation of this outcome is that the managerial resources no longer needed for simple communication tasks could now be applied to more complex analysis tasks that would not previously have been undertaken.

(3) A "third-order" effect of reducing coordination costs may be to encourage a shift toward the use of more "coordination-intensive" structures. In other words, coordination structures that were previously too "expensive" will now become more feasible and desirable. For example, as noted above, information technology can facilitate what some observers [Mintzberg 1979; Toffler 19701 have called adhocracies. Adhocracies are very flexible organizations, including many shifting project teams and highly decentralized networks of communication among relatively autonomous entrepreneurial groups. One of the disadvantages of adhocracies is that they require large amounts of unplanned communication and coordination throughout an organization. However, technologies such as electronic mail and computerized conferencing can help reduce the costs of this communication, and advanced information-sharing tools [Malone et al. 1987a; Lotus 1989] may help make this communication more effective at much larger scales.

What might these new coordination-intensive structure be like? Let us consider recent work on two specific questions about the effects of information technology on organizations and markets: (1) How will IT affect the size of organizations? and (2) How will IT affect the degree of centralization of decision making in organizations? This work does not focus explicitly on any specific dependencies. Instead, it compares two pairs of general coordination mechanisms that can manage many such dependencies: (1) market transactions versus internal decision making with firms and (2) centralized versus decentralized managerial decisions.

#### 3.2.1 Firm Size

Malone et al. [1987b] have used ideas from transaction cost theory to systematically analyze how information technology will affect firm size and, more generally, the use of markets as a coordination structure. They conclude that by reducing the costs of coordination, information technology may lead to an overall shift toward smaller firms and proportionately more use of markets—rather than internal decisions within firms—to coordinate economic activity.

This argument has two parts. First, since market transactions often have higher coordination costs than internal coordination [Williamson 1985; Malone et al. 1987b] an overall reduction in the "unit costs" of coordination should lead to markets becoming more desirable in situations where internal transactions were previously favored. This, in turn, should lead to less vertical integration and smaller firms.

For example, after the introduction of computerized airline reservation systems, the proportion of reservations made through travel agents (rather than by calling the airline directly) went from 35% to 70%. Thus, the function of selling reservations was "disintegrated" from the airlines and moved to a separate firm—the travel agents. Econometric analyses of the overall U.S. economy in the period 1975–1985 are also consistent with these predictions: the use of information technology appears to be correlated with decreases in both firm size and vertical integration [Brynjolfsson et al. 19941.

If we extrapolate this trend to a possible long-run extreme, it leads us to speculate that we might see increasing use of "firms" containing only one person. For instance, Malone and Rockart [1991] suggest that there may someday be electronic marketplaces of "intellectual mercenaries" in which it is possible to electronically assemble "overnight armies" of thousands of people who work for a few hours or days to solve a particular problem and then disband. Flexible arrangements like this might appeal especially to people who had a strong desire for autonomy—the freedom to choose their own hours and working situations.

#### 3.2.2 Centralization of Decision Making

Gurbaxani and Whang [1991] have used ideas from agency theory to systematically analyze the effects on centralization of the reductions in coordination costs enabled by IT. They conclude that IT can lead to either centralization or decentralization, depending on how it is used. While this conclusion may not be surprising, the structure of their analysis helps us understand the factors involved more clearly: (1) when IT primarily reduces decision information costs, it leads to more centralization. For instance, the Otis Elevator Company used IT to centralize the reporting and dispatching functions of their customer service system, instead of having these functions distributed to numerous remote field offices [Stoddard 19861; (2) on the other hand, when IT primarily reduces agency costs, it leads to more decentralization. As used here, agency costs are the costs of employees not acting in the interests of the firm. For instance, when one insurance company developed a system that more effectively monitored their salespeople's overall performance, they were able to decentralize to the salespeople many of the decisions that had previously been made centrally [Bruns and McFarlan 19871. Overall, this bidirectional trend for IT and centralization is consistent with empirical studies of this question [Attewell and Rule 19841.

An alternative approach to this question is provided by Danziger et al. [1982]. In a sense, this work can be considered a kind of "behavioral coordination theory." In studies of computerization decisions in 42 local governments in the U.S., they found that changes in centralization of power were not best explained by any of the formal factors one might have expected. Instead, they found that since people who already have power influence computerization decisions, the new uses of computers tend to reinforce the existing power structure, increasing the power of those who already have it.

### 3.3 Designing Cooperative-Work Tools

There has recently been a great deal of interest in designing computer tools to help people work together more effectively [Greif 1988; Johansen 1988; Ellis et al. 1991; Peterson 1986; Tatar 1988; 19901. (Additional references are listed in Table 3.) Using terms such as "computer-supported cooperative work" and 'groupware," these systems perform functions such as helping people collaborate on writing the same document, managing projects, keeping track of tasks, and finding, sorting, and prioritizing electronic messages. Other systems in this category help people display and manipulate information more effectively in face-to-face meetings and represent and share the rationales for group decisions.

In this section, we will describe how ideas about coordination have been helpful in suggesting new systems, classifying systems, and analyzing how these systems are used.

# 3.3.1 Using Coordination Concepts from Other Disciplines to Suggest Design Ideas

One way of generating new design ideas for cooperative-work tools is to look to other disciplines that deal with coordination. For instance, even though the following authors did not explicitly use the term "coordination theory," they used ideas about coordination from other dis-

 Table 3. A Taxonomy of Cooperative-WorkTools Based on the Processes They Support

| Process                                                             | Example systems                                                                                          |
|---------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
| Managing shared resources (task assignment and prioritization)      | Coordinator (Winograd and Flores, 1986)<br>Information Lens (Malone, et al., 1987)                       |
| Managing producer/consumer relationships (sequencing prerequisites) | Polymer (Croft & Lefkowitz, 1988)                                                                        |
| Managing simultaneity constraints (synchronizing)                   | Meeting scheduling tools (e.g., Beard, et al., 1990)                                                     |
| Managing task / subtask relationship (goal decomposition)           | Polymer (Croft and Lefkowitz, 1988)                                                                      |
| Group decision-making                                               | gIBIS (Conklin and Begeman, 1988)<br>Sibyl (Lee, 1990)                                                   |
|                                                                     | electronic meeting rooms (e.g., Stefik, et al., 1987; Dennis, et al., 1988; DeSanctis & Gallupe, 1987)   |
| Communication                                                       | Electronic mail, Computer conferencing (e.g., Lotus, 1989)                                               |
|                                                                     | electronic meeting rooms (e.g., Stefik, et al., 1987; Dennis, et al., 1988; DeSanctis and Gallupe, 1987) |
|                                                                     | Information Lens (Malone, et al., 1987)                                                                  |
|                                                                     | collaborative authoring tools (e.g., Fish, et al., 1988; Ellis, et al., 1990; Neuwirth, et al., 1990)    |

ciplines to help develop cooperative-work tools.

# 3.3.2 Using Ideas from Linguistics and Philosophy About Speech Acts

Winograd and Flores [Flores et al. 1988; Winograd 1987; Winograd and Flores 19861 have developed a theoretical perspective for analyzing group action based heavily on ideas from linguistics (e.g., Searle [19751). This perspective emphasizes different kinds of speech acts, such as requests and commitments. For example, Winograd and Flores analyzed a generic "conversation for action" in terms of the possible states and transitions involved when one actor performs a task at the request of another. An actor may respond to a request, for instance, by (1) promising to fulfill the request, (2) de-

clining the request, (3) reporting that the request has already been completed, or (4) simply acknowledging that the request has been received. The analysis of this conversation type (and several others) provided a primary basis for designing the Coordinator, a computer-based cooperative-work tool. For example, the Coordinator helps people make and keep track of requests and commitments to each other. It thus supports what we might call the "mutual agreeing" part of the task assignment process.

### 3.3.3 Using Ideas from Artificial Intelligence and Organization Theory About Blackboards and Adhocracies

Malone [1990] describes how ideas from artificial intelligence and organization theory combined to suggest a new tool for

routing information within organizations. In the "blackboard architecture," program modules interact by searching a global blackboard for their inputs and posting their outputs on the same blackboard [Nii 1986; Erman et al. 19801. This provides very flexible patterns of communication among different program modules: any module can communicate with any other module, even when this interaction is not explicitly anticipated by the program designer. In adhocracies, as we saw above, just this kind of unplanned, highly decentralized communication is essential for rapidly responding to new situations [Mintzberg 1979; Toffler 19701. Stimulated, in part, by this need for an "organizational blackboard," Malone et al. [1987a] designed the Information Lens system. A central component of this system is an "anyone server" that lets people specify rules about what kinds of electronic messages they are interested in seeing. The system then uses these rules to route all nonprivate electronic messages to everyone in the organization who might want to see them. (To help people deal with large numbers of messages, another part of the system uses a different set of rules to sort and prioritize the messages people receive.)

# 3.3.4 Using Ideas from Philosophy and Rhetoric About Decision Making

Two cooperative-work tools, gIBIS [Conklin and Begeman 19881 and Sibyl [Lee 19901 are designed to help groups of people make decisions more effectively. To do this, they explicitly represent the arguments (and counterarguments) for different alternatives a group might choose. Both these systems are based on ideas from philosophy and rhetoric about the logical structure of decision making. For example, the basic elements in the gIBIS system (issues, positions, and arguments) are taken from a philosophical analysis of argumentation by Rittel and Kunz [1970]. The constructs for representing arguments in Sibyl are based on the work of philosophers like Toulmin [1958] and Rescher [19771.

## 3.3.5 Using Ideas from Computer Science About Parallel Processes

Holt [1988] describes a theoretical language used for designing coordination tools that is based, in part, on ideas about Petri nets, a formalism used in computer science to represent process flows in distributed or parallel systems [Peterson 1981; 19771. This language is part of a larger theoretical framework called "coordination mechanics" and has been used to design a "coordination environment" to help people work together on computer networks.

# 3.3.6 Summary of Examples

Clearly, using ideas about coordination from other disciplines does not provide any guarantee of developing useful cooperative-work tools. However, we feel that considering these examples within the common framework of coordination theory provides two benefits: (1)it suggests that no one of these perspectives is the complete story and (2) it suggests that we should look to previous work in various disciplines for more insights about coordination that could lead to new cooperative-work tools.

### 3.3.7 A Taxonomy of Cooperative-Work Tools

As shown in Table 3, the framework we have suggested for coordination provides a natural way of classifying existing cooperative-work systems according to the coordination processes they support. Some of these systems primarily emphasize a single coordination-related process. For instance, electronic mail systems primarily support the message transport part of communication, and meeting scheduling tools primarily support the synchronization process (i.e., arranging for several people to attend a meeting at the same time). There is a sense, of course, in which each of these systems also support other processes (e.g., a simple electronic mail system can be used to assign tasks), but we have categorized the systems here according to the processes they explicitly emphasize.

Some of the systems also explicitly support several processes. For example, the Information Lens system supports both the communication-routing process (by rules that distribute messages to interested people) and a form of resource allocation process (by helping people prioritize their own activities using rules that sort messages they receive). And the Polymer system helps people decompose goals into tasks and sequence the tasks (e.g., to prepare a monthly report, first gather the project reports and then write a summary paragraph).

One possibility raised by this framework is that it might help identify new opportunities for cooperative-work tools. For instance, the Coordinator focuses on supporting one part of the task assignment process (mutual agreement on commitments). However, it does not provide much help for the earlier part of the process involving selecting an actor to perform the task in the first place (see Section 2.3). New tools, such as an "electronic yellow pages" or bidding schemes like those suggested by Turoff [19831 and Malone [1987] might be useful for this purpose.

Another intriguing possibility suggested by this framework is that it might be possible to implement "primitives" for a number of different coordination-related processes in the same environment and then let people combine these primitives in various ways to help solve particular coordination problems. This is one of the goals of the Oval system [Malone et al. 1992; Lai et al. 19881.

# 3.3.8 Analyzing Incentives for Using Cooperative-Work Tools

Another use for coordination theory in designing cooperative-work tools can be to help systematically evaluate proposed or actual systems. For example, Markus and Connolly [19901 systematically analyze how the payoffs to individual users of a cooperative-work system depend on how many other people are using the system. They do this by using an economic model from Schelling [1978] to ex-

tend Grudin's [1988] insights about the incentives to use cooperative-work systems. For instance, on-line calendars and many other cooperative-work applications involve "discretionary databases" which users can view or update as they see fit. For each individual user, however, the benefits of viewing the database can be obtained without contributing anything. Thus, it is often in the interests of each individual user to use the database without making the effort required to contribute to it. Unfortunately, the equilibrium state of a system like this is for no one to ever contribute anything!

An interesting empirical illustration of this phenomenon occurred in a study of how one large consulting firm used the Lotus Notes group-conferencing system. In this study, Orlikowski [1992] found that there were surprising inconsistencies between the intended uses of the system and the actual incentives in the organization. For instance, Orlikowski observed that this organization (like many others) was one'in which people were rewarded for being the "expert" on something—for knowing things that others did not. Should we be surprised, therefore, that many people were reluctant to spend much effort putting the things they knew into a database where everyone else could easily see them?

These observations do not, of course, mean that conferencing systems like this one cannot be useful in organizations. What they do mean, however, is that we must sometimes be sensitive to very subtle issues about things like incentives and organizational culture in order to obtain the full benefits of such systems. For instance, it might be desirable in this organization to include, as part of an employee's performance appraisal, a record of how often their contributions to the Notes database were used by other people in the organization.

# 3.4 Designing Distributed and Parallel Computer Systems

Much recent activity in computer science has involved exploring a variety of dis-

tributed and parallel computer architectures. In many ways, physically connecting the processors to each other is easy compared to the difficulty of coordinating the activities of many different processors working on different aspects of the same problem.

In this section, we describe examples of work that has addressed these issues in an explicitly interdisciplinary way, drawing on insights from other disciplines or kinds of systems to design or analyze distributed or parallel computer systems. In particular, we consider examples of (1) analogies with social and biological systems as a source of design ideas and (2) quantitative tools for analyzing alternative designs.

## 3.4.1 Analogies with Social and Biological Systems as a Source of Design Ideas

One of the basic problems in designing distributed or parallel computer systems is how to assign tasks to processors, and several distributed computer systems have addressed this problem with competitive-bidding mechanisms based on analogies with human markets. For example, the Contract Nets protocol [Smith and Davis 1981; Davis and Smith 1983] formalizes a sequence of messages to be exchanged by computer processors sharing tasks in a network. The "contracts" are arbitrary computational tasks that can potentially be performed by any of a number of processors on the network; the "clients" are machines at which these tasks originate; and the "contractors" are machines that might process the tasks (i.e., the servers). The sequence of announcement, bid, and award messages used by this protocol was described above in our analysis of the task assignment process (Section 2.3). One of the desirable features of this system is its great degree of decentralization and the flexibility it provides for how both clients and contractors can make their decisions. For instance, clients may select contractors on the basis of estimated completion time or the presence of specialized data; contractors may select tasks to bid on based

on the size of the task or how long the task has been waiting.

Using these or similar ideas, a number of other bidding systems have been developed (e.g., Stankovic [19851 and Kurose and Simha [1989]). For instance, several bidding systems have been developed to allow personal workstations connected by a local-area network to share tasks [Malone et al. 1988; Waldspurger et al. 19881. In this way, users can take advantage of the unused processing capacity at idle workstations elsewhere on the network. Furthermore, the local bidding "negotiations" can result in globally coherent processor scheduling according to various priorities (see Malone et al. [1988]). (For a review of several related systems and an analysis of a variety of bidding algorithms, see Drexler and Miller [1988] and Miller and Drexler [19881.)

The notion of competitive-bidding markets has also been suggested as a technique for storage management by Miller and Drexler [1988] and Drexler and Miller [19881. In their proposal, when object A wishes to maintain a pointer to object B, object A pays "rent" to the "landlord" of the space in which object B is stored. These rents are determined by competitive bidding, and when an object fails to pay rent, it is "evicted (that is, garbage collected). Their proposal includes various schemes for how to determine rents, how to pass rents along a chain of references, and how to keep track of the various costs and payments without excessive overhead. They conclude that this proposal is not likely to be practical for small-scale storage management (such as garbage collection of individual Lisp cells), but that it may well be useful for sharing large objects in complex networks that cross "trust boundaries" (e.g., interorganizational networks). The scheme also appears useful for managing local caching and the migration of objects between different forms of short-term and long-term storage.

Another central problem that arises in distributed and parallel systems is how and when to route information between processors. For instance, one interesting example of this problem arises in artificial intelligence programs that search a large space of possibilities, the nature of which is not well known in advance. It is particularly useful, in this case, for processors to exchange information about intermediate results in such a way that each processor can avoid performing work that is rendered unnecessary by work already done elsewhere.

One solution to this problem is suggested by the Scientific Community Metaphor embodied in the Ether system [Kornfeld and Hewitt 1981; Kornfeld 19821. In this system, there are a number of "sprites," each analogous to an individual scientist, that operate in parallel and interact through a global database. Each sprite requires certain conditions to be true in the global database before it is "triggered." When a sprite is triggered, it may (1) compute new results that are added to the global database, (2) create new sprites that await conditions that will trigger them, or (3) stifle a collection of sprites whose work is now known to be unnecessary. In one example use of this system, Kornfeld [19821 shows how sharing intermediate results in this way can dramatically improve the time performance of an algorithm (even if it is executed by time-sharing a single processor). He calls this effect "combinatorial implosion."

This system also uses the Scientific Community Metaphor to suggest a solution to the resource allocation problem for processors. Each sprite is "supported)) by a "sponsor," and without a sponsor, a sprite will not receive any processing time to do its work. For instance, a sponsor may sometimes support both work directed toward proving some proposition and work directed toward proving the negation of the proposition. Whenever one of these lines of work is successful, support is withdrawn from the other.

### 3.4.2 Analyzing Stability Properties of Resource Allocation Algorithms

Another way of applying coordination concepts is to help evaluate alternative

designs of distributed and parallel computer systems. For instance, Huberman and Hogg [1988] and Lumer and Huberman [19901 have applied mathematical techniques like those used in chaos theory to analyze the dynamic behavior of distributed computer networks. In one case they analyze, for example, heavily loaded processors in a network transfer task to more lightly loaded processors according to a probabilistic process. When any processor in such a system can exchange tasks with any other processor, the behavior of the system is unstable for large numbers of processors (e.g., more than 21 processors in a typical example). However, when the processors are grouped hierarchically into clusters that exchange tasks frequently among themselves and only occasionally with other clusters, the system remains stable for arbitrarily large numbers of processors. This hierarchical arrangement has the disadvantage that it takes a long time to reach stability. In an intriguing analogy with human organizations, however, Huberman and his colleagues find that this disadvantage can be eliminated by having a few "lateral links" between different clusters in the hierarchy [Lumer and Huberman 19901.

### 3.5 Summary of Applications

As summarized in Table 4, the examples we have described show how a coordination perspective can help (1) analyze alternative designs and (2) suggest new design ideas. In each case, these applications depended on interdisciplinary use of theories or concepts about coordination

#### 4. RESEARCH AGENDA

We have seen how a number of different disciplines can contribute to answering the questions about coordination and how **theories** of coordination can, in turn, **be** applied to the concerns of several different disciplines. What is needed to further develop this interdisciplinary study of coordination?

on firm size, centralization,

Analyzing how the payoffs to

depend on the number of other making

individual users of a system

Analyzing stability properties

of load sharing algorithms in

computer networks

and internal structure

Application area

Organizational

structures and

Cooperative work

Distributed and

parallel computer

information

technology

tools

systems

Examples of analyzing alternative designs

Examples of generating new design ideas alternative designs

Creating temporary "intellectual marketplaces" to solve specific problems.

**Table 4.** Sample Applications of a Coordination Perspective

As we suggested above, a central concern of coordination theory should be to exidentify and analyze specific coordination on

processes and structures. Therefore, a

critical item on the agenda for coordina-

tion research should be to develop these

analyses. For example, the following kinds of questions arise.

4.1 Representing and Classifying

**Coordination Processes** 

How can we represent coordination processes? When should we use flowcharts, Petri nets, or state transition diagrams? Are there other notations that are even more perspicuous for analyzing coordination? How can we classify different coordination processes? For instance, can we usefully regard some coordination processes as "special cases" of others? How are different coordination processes combined when activities are actually performed?

#### 4.1.1 Characterizing Dependencies

What kinds of dependencies are there? Are there ways to organize them that highlight common possibilities for managing them? Are some special cases of others? What causes dependencies? As we modify or alter a process, what tech-

niques will be useful for keeping track of existing dependencies or identifying new ones? What techniques are useful for identifying dependencies in a field study of a particular process?

Designing new tools for task assignment,

information routing, and group decision-

Using competitive bidding mechanisms to

Using a scientific community metaphor to organize parallel problem-solving.

allocate processors and memory in

computer systems.

# 4.1.2 How General are Coordination Processes?

Another set of questions has to do with how generic coordination processes really are: How far can we get by analyzing very general coordination processes, and when will we find that most of the important factors are specific to coordinating a particular kind of task? For example, are there general heuristics for coordination that are analogous to the general problem-solving heuristics studied in cognitive science and artificial intelligence?

#### 4.2 Analyzing Specific Processes

At least as important as these general questions are analyses of specific processes. For example, how far can we go in analyzing alternative coordination processes for problems such as resource allocation? Can we characterize an entire "design space" for solutions to this problem and analyze the major factors that would favor one solution over another in specific situations? Could we do the same

thing for other processes such as goal selection or managing timing dependencies? Are there other processes (such as managing other kinds of dependencies) that could be analyzed systematically in ways that have not yet been done?

In analyzing alternative processes for specific problems, we might consider various kinds of properties: Which processes are least "expensive" in terms of production costs and coordination costs? Which processes are fastest? Which processes are most stable in the face of failures of actors or delays of information? Which processes are most susceptible to incentive problems? For instance, how does the presence of significant conflicts of interest among actors affect the desirability of different resource allocation methods? How do information-processing limitations of actors affect the desirability of different methods? For example, are some methods appropriate for coordinating people that would not be appropriate for coordinating computer processors, and vice versa? What new methods for coordinating people become desirable when human informationprocessing capacities are augmented by computers?

#### 4.3 Applications and Methodologies

A critical part of the research agenda for this area is to develop coordination theory in the context of various different kinds of systems. For instance, in Section 3, we suggested numerous examples of these possibilities for human organizations and computer systems.

In some cases, this work may involve applying previously developed theories to these application areas. In many cases, however, we expect that new systems or new observations of these systems will stimulate the development of new theories. For example, all of the following methodologies appear likely to be useful in developing coordination theory: (1) empirically studying coordination in human or other biological systems (e.g., field studies, laboratory studies, or econometric studies), (2) designing new technolo-

gies for supporting human coordination, (3) designing and experimenting with new methods for coordinating distributed and parallel computer systems, and (4) formal modeling of coordination processes (e.g., mathematical modeling or computer simulation).

# 5. CONCLUSIONS

Clearly, the questions we have just listed are only the beginning of a set of research issues in the interdisciplinary study of coordination. However, we believe they illustrate how the notion of "coordination" provides a set of abstractions that help unify questions previously considered separately in a variety of different disciplines and suggests avenues for further exploration.

While much work remains to be done, it appears that this approach can build on much previous work in these different disciplines to help solve a variety of immediate practical needs, including: (1) designing computer and communication tools that enable people to work together more effectively,(2) harnessing the power of multiple computer processors working simultaneously on related problems, and (3) creating more flexible and more satisfying ways of organizing collective human activity.

# APPENDIX A: PREVIOUS DEFINITIONS OF COORDINATION

"The operation of complex systems made up of components" [National Science Foundation 19891.

"The emergent behavior of collections of individuals whose actions are based on complex decision processes" [National Science Foundation 19891.

"Information processing within a system of communicating entities with distinct information states" [National Science Foundation 1989].

"The joint efforts of independent communicating actors towards mutually defined goals" [National Science Foundation 1989].

"Networks of human action and commitments that are enabled by computer and communications technologies" [National Science Foundation 19891.

"Composing purposeful actions into larger purposeful wholes" (A. Holt, personal communication, 1989).

"Activities required to maintain consistency within a work product or to manage dependencies within the workflow" [Curtis 19891.

"The integration and harmonious adjustment of individual work efforts towards the accomplishment of a larger goal" [Singh 1992].

"The additional information processing performed when multiple, connected actors pursue goals that a single actor pursuing the same goals would not perform" [Malone 19881.

"The act of working together" [Malone and Crowston 19911.

# APPENDIX B: RESULTS ABOUT COORDINATION FROM SELECTED FIELDS

Even though use of the term "coordination theory" is quite recent, a great deal of previous work in various fields can contribute to the interdisciplinary understanding of coordination. In this appendix, we briefly describe examples of such work from several different disciplines. These examples focus on cases where coordination has been analyzed in ways that appear to be generalizable beyond a single discipline or type of actor. We have not, of course, attempted to list all such cases; we have merely tried to pick illustrative examples from several disciplines.

#### **Computer Science**

#### Sharing Resources

Much research in computer science focuses on how to manage activities that share resources, such as processors, memory, and access to input/output devices (e.g., Deitel [1983]). Other mechanisms have been developed to enforce resource allocations. For example, semaphores, monitors, and critical regions for mutual exclusion are programming con-

structs that can be used to grant a process exclusive access to a resource (see Hoare [1975] and Dijkstra [1968]). Researchers in database systems have developed numerous other mechanisms, such as locking or timestamping, to allow multiple processes to concurrently access shared data without interference (see Bernstein and Goodman [1981]).

#### Managing Unreliable Actors

Additionally, protocols have been developed to ensure the reliability of transactions comprising multiple reads or writes on different processors (see Kohler [1981]). In particular, these protocols ensure that either all a transaction's operations are performed or none are, even if some of the processors fail.

#### Segmenting and Assigning Tasks

One of the important problems in allocating work to processors is how to divide up the tasks. For example, Carrerio and Gelernter [19891 discuss three alternative ways of dividing parallel programs into units: according to the type of work to be done, according to the subparts of the final output, or simply according to which processor is available.

#### Managing Information Flows

Another important set of issues involves managing the flow of information. For instance, researchers in artificial intelligence and particularly in distributed artificial intelligence (DAI) [Bond and Gasser 1988; Huhns and Gasser 19891 have used "blackboard architectures" to allow processes to share information without having to know precisely which other processes need it [Nii 1986; Erman et al. 19801 and "partial global plans" to allow actors to recognize when they need to exchange more information [Durfee and Lesser 19871.

#### **Economics and Operations Research**

In a sense, almost all of economics involves the study of coordination, with a

special focus on how incentives and information flows affect the allocation of resources among actors. For example, classical microeconomics analyzes how different sources of supply and demand can interact locally in a market in ways that result in a globally coherent allocation of resources. Among the major results of this theory are formal proofs that (under appropriate mathematical conditions) if consumers each maximize their individual "utilities" and if firms each maximize their individual profits, then the resulting allocation of resources will be globally "optimal" in the sense that no one's utilities can be increased without decreasing someone else's (see Debreu [1959]).

Some more recent work in economics has focused on the limitations of markets and contracts for allocating resources. For instance, transaction cost theory analyzes the conditions under which a hierarchy is a better way of coordinating multiple actors than a market (see Williamson [1975]). Agency theory focuses on how to create incentives for some actors ("agents") to act in a way that advances the interests of other actors ("principals") even when the principals cannot observe everything their agents are doing [Ross 19731. One result of this theory is that there are some situations where no incentives can motivate an agent to perform optimally from the principal's point of view [Jensen and Meckling 19761.

Finally, some parts of economics focus explicitly on information flows. For example, team theory and its descendants analyze how information should be exchanged when multiple actors need to make interdependent decisions but when all agents have the same ultimate goals (see Marschak and Radner [1972], Hurwicz [1973], and Reiter [1986]). Mechanism design theory also analyzes how to provide incentives for actors to reveal information they possess, even when they have conflicting goals. For example, this theory has been applied to designing and analyzing various forms of auctions. In a "second-price auction," for instance, each participant submits a sealed bid, and the highest bidder is only required to pay the amount of the second highest bid. It can be shown that this mechanism motivates the bidders to each reveal the true value they place on the item being sold, rather than trying to "game the system" by bidding only enough to surpass what they expect to be the next highest bid [Myerson 1981].

Operations research analyzes the properties of various coordination mechanisms, but operations research also includes a special focus on developing optimal techniques for coordination decisions. For instance, operations research includes analyses of various scheduling and queuing policies and techniques such as linear programming and dynamic programming for making resource allocation decisions optimally (see Dantzig [1963]).

## **Organization Theory**

Research in organization theory, drawing on disciplines such as sociology and psychology, focuses on how people coordinate their activities in formal organizations. A central theme in this work has involved analyzing general issues about coordination (see Simon [1976], March and Simon [1958], Thompson [1967], Galbraith [1977], Lawrence and Lorsch [1967] and summarized by Mintzberg [19791 and Malone [19901). We can loosely paraphrase the key ideas of this work as follows.

All activities that involve more than one actor require (1) some way of dividing activities among the different actors and (2) some way of managing the interdependencies among the different activities [March and Simon 1958; Lawrence and Lorsch 19671. Interdependencies between activities can be of (at least) three kinds: (a) pooled, where the activities share or produce common resources but are otherwise independent, (b) sequential, where some activities depend on the completion of others before beginning, and (c) reciprocal, where each activity requires inputs from the other [Thompson 19671. These different kinds of interdependencies can be managed by a variety of coordination mechanisms, such as: *standardization*, where predetermined rules govern the performance of each activity; *direct supervision*, where one actor manages interdependencies on a case-by-case basis: and *mutual adjustment*, where each actor makes on-going adjustments to manage the interdependencies [March and Simon 1958; Galbraith 1973; Mintzberg 1979].

These coordination mechanisms can be used to manage interdependencies, not only among individual activities, but also among groups of activities. One criterion for grouping activities into units is to minimize the difficulties of managing these intergroup interdependencies. For example, activities with the strongest interdependencies are often grouped into the smallest units; then these units are grouped into larger units with other units with which they have weaker interdependencies. Various combinations of the coordination mechanisms, together with different kinds of grouping, give rise to the different organizational structures common in human organizations, including functional hierarchies, product hierarchies, and matrix organizations. For instance, sometimes all activities of the same type (e.g., manufacturing) might be grouped together in order to take advantage of economies of scale; at other times, all activities for the same product (e.g., marketing, manufacturing, and engineering) might be grouped together to simplify managing the interdependencies among the activities.

#### **Biology**

Many parts of biology involve studying how different parts of living entities interact. For instance, human physiology can be viewed as a study of how the activities of different parts of a human body are coordinated to keep a person alive and healthy. Other parts of biology involve studying how different living things interact with each other. For instance, ecology can be viewed as the study of how the activities of different plants

and animals are coordinated to maintain a "healthy" environment.

Some of the most intriguing studies of biological coordination involve coordination among different animals in a group. For example, Mangel and Clark [1988] discuss the optimal hunting pack size for lions, who trade the benefit of an increased chance of catching something against the cost of having to share what they catch. Deneubourg and Gross [19891 point out that the interaction among simple rules—such as "do what my neighbor is doing"—and the environment may lead to a variety of collective behaviors.

The most striking examples of such group behaviors are in social insects, such as honey bees or army ants, where the group displays often quite complex behavior, despite the simplicity of the individuals (see Franks [1989] and Seeley [1989]). Using a variety of simple rules, these insects "allocate" individual workers at economically efficient levels to a variety of tasks—including searching for new food sources, gathering nectar or pollen from particular sources (bees), carrying individual food items back to the bivouac (ants), guarding the hive (bees), and regulating the group temperature. For example, in honey bees, the interaction of two simple local rules controls the global allocation of food collectors to particular food sources. First, nectar-storing bees unload nectar from foraging bees returning to the hive at a rate that depends on the richness of the nectar. Second, if bees are unloaded rapidly, they recruit other bees to their food source. The result of these two rules is that more bees collect food from better sources. Seeley [1989] speculates that this decentralized control may occur because it provides faster responses to local stresses [Miller 19781, or it may be simply because bees have not evolved any more global means of communication.

### **ACKNOWLEDGMENTS**

This work was supported, in part, by Digital Equipment Corporation, the National Science Foundation (grant nos. IRI-8805798 and IRI-8903034), and other sponsors of the MIT Center for Coordination

Science. Parts of this paper were included in three previous papers [Malone 1988; Malone and Crowston 1990; 1991]. We are especially grateful to Deborah Ancona, John Carroll, Michael Cohen, Randall Davis, Rob Kling, John Little, and Wanda Orlikowski for comments on earlier versions of the survey, and to participants in numerous seminars and workshops at which these ideas have been presented.

#### **REFERENCES**

- ALLEN, T. J. 1977. Managing the Flow of Technology. MIT Press, Cambridge, Mass.
- ALLEN, J., HENDLER, J. AND TATE, A. EDS. 1990.

  Readings in Planning. Morgan Kaufmann, San
  Mateo Calif
- Arrow, K. J. 1951. Social Choice and Individual Value. Vol. 12. John Wiley and Sons, New York.
- ARVIND, AND CULLER, D. E. 1986. Dataflow architectures. In *Annual Reviews in Computer Science*. Vol. 1. Annual Reviews, Inc., Palo Alto, Calif.
- ARVIND, NIKHIL, R. S., AND PINGALI, K. K. 1986. I-Structures: Data structures for parallel computing. In *Proceedings of the Graph Reduction Workshop*.
- ATTEWELL, P. AND RULE, J. 1984. Computing and organizations: What we know and what we don't know. Commun. ACM 27, 1184–1192.
- Aumann, R. J. 1976. Agreeing to disagree. *Ann. Stat.* 4, 1236–1239.
- Baligh, H. H. 1986. Decision rules and transactions, organizations and markets. *Manage. Sci.* 32, 1480–1491.
- Baligh, H. H. and Burton, R. M. 1981. Describing and designing organizational structures and processes. *Int. J. Policy Anal. Inf. Syst.* 5, 251–266.
- BALIGH, H. H. AND RICHARTZ, L. 1967. Vertical Market Structures. Allyn and Bacon, Boston.
- BARNARD, C. I. 1964. The Functions of the Executive. Harvard University, Cambridge, Mass.
- BEARD, D., MURUGAPPAN, P., HUMM, A., BANKS, D., NAIR, A., AND SHAN, Y.-P. 1990. A visual calendar for scheduling group meetings. In Proceedings of the 3rd Conference on Computer-Supported Cooperative Work. ACM Press, New York, 279–290.
- Bernstein, P. and Goodman, N. 1981. Concurrency control in distributed database systems. *ACM Comput. Surv. 13*, 2, 185–221.
- Bond, A. H. and Gasser, L. Eds. 1988. *Readings in Distributed Artificial Intelligence*. Morgan Kaufman, San Mateo, Calif.
- Bruns, W. J. and McFarlan, F. W. 1987. Information technology puts power in control systems. *Harvard Bus. Rev.* (Sept.-Oct.), 89-94.
- BRYNJOLFSSON, E., MALONE, T., GURBAXANI, J., AND KAMBIL, A. 1994. Does information technology lead to smaller firms? *Manage. Sci.*

- BURTON, R. M. AND OBEL, B. 1980a. A computer simulation test of the M-form hypothesis. *Admin. Sci.* **Q.** 25, 457–466.
- Burton, R. M. AND OBEL, B. 1980b. The efficiency of the price, budget, and mixed approaches under varying a priori information levels for decentralized planning. *Manage. Sci.* 26, 401–417.
- CARRIERO, N. AND GELERNTER, D. 1989. Coordination languages and their significance. Working Paper YALEU/DCS/RR-716. New Haven, CT: Dept. of Computer Science, Yale Univ. New Haven, Conn.
- CARTER, D. E. AND BAKER, B. S. 1991. Concurrent Engineering: The Product Development Environment for the 1990's. Addison-Wesley, Reading, Mass.
- CHANDLER, A. D. 1977. Administrative coordination, allocation and monitoring: Concepts and comparisons. Working paper 77-21. European Institute for Advanced Studies in Management. Brussels.
- CHANDLER, A. D., Jr. 1962. Strategy and Structure: Chapters in the History of the American Industrial Enterprise. MIT Press, Cambridge, Mass
- CHAPMAN, D. 1987. Planning for conjunctive goals. Artif. Zntell. 32, 333–377.
- CIBORRA, C. U. 1987. Reframing the role of computers in organizations: The transaction costs approach. *Office: Tech. People* 3, 17–38.
- COHEN, P. AND LEVESQUE, H. J. 1991. Teamwork. Technote No. 504. SRI International, Menlo Park, Calif.
- CONKLIN, J. AND BEGEMAN, M. L. 1988. gIBIS: A hypertext tool for exploratory policy discussion. In *Proceedings of CSCW '88 Conference on Computer-Supported Cooperative Work*. ACM Press, New York, 140–152.
- Crawford, A. B., Jr. 1982. Corporate electronic mail—A communication-intensive application of information technology. *MIS Q. 6*, (Sept.), 1–13.
- CROFT, W. B. AND LEFKOWITZ, L. S. 1988. Using a planner to support office work. In *Proceedings* of the ACM Conference on Office Znformation Systems. ACM, New York, 55–62.
- CROWSTON, K. 1991. Towards a coordination cookbook. Recipes for multi-agent action. Ph.D. dissertation, MIT Sloan School of Management, Cambridge, Mass.
- Crowston, K., Malone, T. W, and Lin, F. 1987. Cognitive science and organizational design: A case study of computer conferencing. *Hum. Comput. Interaction* 3, 59–85.
- Curtis, B. 1989. Modeling coordination from field experiments. In *Proceedings of the Conference on Organizational Computing, Coordination and Collaboration: Theories and Technologies for Computer-Supported Work.*
- CYTRON, R. 1987. Limited processor scheduling of doacross loops. In *Proceedings of the 1987*

- International Conference on Parallel Processing. Pennsylvania State University, University Park, Penn.
- DANTZIG, G. B. 1963. *Linear Programming and Extensions*. Princeton University Press, Princeton, N.J.
- DANZIGER, J. N., DUTTON, W. H., KLING, R. AND KRAEMER, K. L. 1982. Computers and Politics: High Technology in American Local Governments. Columbia University Press, New York.
- DAVIS, R. AND SMITH, R. G. 1983. Negotiation as a metaphor for distributed problem solving. *Artif. Intell.* 20, 63–109.
- Debreu, G. 1959. Theory of Value: An Axiomatic Analysis of Economic Equilibrium. Wiley, New York
- DEITEL, H. M. 1983. An Introduction to Operating Systems. Addison-Wesley, Reading, Mass.
- DENEUBOURG, J. L. AND GROSS, S. 1989. Collective patterns and decision-making. *Ethol. Evol.* 1, 295–311.
- DENNIS, A. R., JOEY, F. G., JESSUP, L. M.. NUNA-MAKER, J. F., AND VOGEL, D. R. 1988. Information technology to support electronic meetings. MIS &. 12, 4(Dec.), 591–619.
- DERTOUZOS, M. L. 1991. Building the information marketplace. *Tech. Reu.* (Jan.), 29-40.
- DeSanctis, G. and Gallupe, B. 1987 **A** foundation for the study of group decision support systems. *Manage*. Sci. 33, 5, 589–609.
- DIJKSTRA, E. W. 1968. The structure of the T. H. E. operating system *Commun. ACM 11*, 5, 341-346.
- DREXLER, K. E. AND MILLER, M. S. 1988. Incentive engineering for computational resource management. In *The Ecology of Computation* Elsevier, Amsterdam, 231–266.
- Dubois, M., Scheurich, C., and Briggs, F. A. 1988. Synchronization, coherence, and event ordering in multiprocessors. *IEEE Comput. 21*, 2, 9–21.
- Durfee, E. D. and Lesser, V. R. 1987. Using partial global plans to coordinate distributed problem solvers. In *Proceedings of the 10th International Joint Conference on Artificial Intelligence (IJCAI-87)*. 875–883.
- Eccles, R. G. 1985. The Transfer Pricing Problem: A Theory for Practice. Lexington Books, Lexington, Mass.
- ELLIS, C. A., GIBBONS, R., AND MORRIS, P. 1979. Office streamlining. In *Proceedings of the International Workshop on Integrated Offices*. Institut de Recherche d'Informatique de d'Automatique, Versailles, France.
- ELLIS, C. A., GIBBS, S. J., AND REIN, G. L. 1991. Groupware, some issues and experiences. Commun. ACM 34, 1, 38–57.
- ELLIS, C. A., GIBBS, S. J., AND REIN, G. L. 1990. Design and use of a group editor In Engineering for Human-Computer Interaction. North-Holland/Elsevier, Amsterdam, 13-25.

- ERMAN, L. D., HAYES-ROTH, F., LESSER, V. R., AND REDDY, D. R. 1980. The HEARSAY-I1 speech understanding system: Integrating knowledge to resolve uncertainty. ACM Comput. Surv. 12, 2, 213-253.
- FARRELL, J. AND SALONER, G. 1985. Standardization, compatibility, and innovation. *Rand J. Econ. 16*, (Spring), 70–83.
- FIKES, R. E. AND NILSSON, N. J. 1971. STRIPS: A new approach to the application of theorem proving to problem solving. *Artif. Intell.* 2, 198–208.
- FISH, R., KRAUT, R., LELAND, M., AND COHEN, M 1988. Quilt: A collaborative tool for cooperative writing. In *Proceedings of the Conference* on Office Information Systems. ACM, New York, 30–37.
- FLORES, F., GRAVES, M., HARTFIELD, B., AND WINO-GRAD, T. 1988. Computer systems and the design of organizational interaction. ACM Trans. Office Inf. Syst. 6, 2, 153-172.
- Fox, M. S. 1981. An organizational view of distributed systems. *IEEE Trans. Syst. Man. Cybernet.* 11, 1, 70-79.
- Franks, N. R. 1989. Army ants: A collective intelligence. Am. Sci. 77, (Mar.-Apr.), 139-145.
- GALBRAITH, J. R. 1977. Organizatzon Design. Addison-Wesley, Reading, Mass.
- GALBRAITH, J. R. 1973. Designing Complex Organizations. Addison-Wesley, Reading, Mass.
- GRAY, J 1978. Notes on data base operating systems. Res. Rep. RJ2188. IBM. Yorktown Heights, N.Y.
- GREIF, I., EDS. 1988. Computer Supported Cooperative Work. Morgan Kaufmann Publishers, Los Angeles, Calif.
- GRUDIN, J. 1988. Why CSCW applications fail: Problems in the design and evaluation of organizational interfaces. In Proceedings of the 2nd Conference on Computer-Supported Cooperative Work. ACM Press, New York, 85–93.
- GURBAXANI, V. AND WHANG, S. 1991. The impact of information systems on organizations and markets. *Commun. ACM* 34, 1, 59–73.
- HALPERN, J. Y. 1987. Using reasoning about knowledge to analyze distributed systems. In Annual Review of Computer Science. Vol. 2. Annual Reviews Inc., Palo Alto, Calif., 37–68.
- HALSTEAD, R. H. 1985. Multilisp: A language for concurrent symbolic computation. ACM Trans. Program. Lang. Syst. 7, 4, 501–538.
- HART, P. AND ESTRIN, D. 1990. Inter-organization computer networks: Indications of shifts in interdependence. In Proceedings of the ACM Conference on Office Information Systems. ACM, New York.
- HEWITT, C. 1986. Offices are open systems. ACM Trans. Office Syst. 4, 3, 271-287.
- HIRSCH, E. D. 1987. Cultural Literacy: What Every American Needs to Know. Houghton Mifflin, Boston,

- HOARE, C. A. R. 1975. Monitors: An operating systems structuring concept. Commun. ACM 17, 10, 549–557. Corrigendum, *Commun. ACM* 18, 2, 95.
- HOLT, A. W. 1988. Diplans: A new language for the study and implementation of coordination. ACM Trans. Office Znf. Syst. 6, 2, 109-125.
- HOLT, A. W. 1980. Coordinator programs. Unpublished Tech. Rep. Massachusetts Computer Associates, Inc., Wakefield, Mass.
- HOLT, A W., RAMSEY, H. R., AND GRIMES, J. D. 1983. Coordination system technology as the basis for a programming environment. *Elec. Commun.* 57, 4, 307–314.
- HUBERMAN, B. A. Ed. 1988a. The Ecology of Computation. North Holland, Amsterdam.
- Huberman, B. A. 1988b. Open systems: The ecology of computation. PARC Working Paper P88-00074. Xerox PARC, Palo Alto, Calif.
- HUBERMAN. B. A. AND HOGG, T. 1988. The behaviour of computational ecologies. In *The Ecology of Computation*. Elsevier, Amsterdam, 77-116.
- HUHNS, M. N. AND GASSER, L., EDS. 1989. Distributed Artificial Zntelligenre. Vol. 3. Morgan Kaufmann, San Mateo, Calif.
- Hurwicz, L. 1973. The design of resource allocation mechanisms. *Am. Econ. Rev. Papers Proc.* 58, (May), 1–30.
- Janis, I. L. and MA', L. 1977. Decision-Making. Free Press, New York.
- JENSEN, M. C. AND MECKLING, W. H. 1976. Theory of the firm: Managerial behavior, agency costs and ownership structure. J. An. Econ. 3, 305–360.
- Johansen, R. 1988. Groupware: Computer Support for Business Teams. The Free Press, New York.
- KAHNEMAN, D. AND TVERSKY, A. 1973. On the psychology of prediction. *Psychol. Rev.* 80, 237–251.
- KIDDER, T. 1981. The Soul of a New Machine. Little Brown, Boston.
- KIESLER, S., SIEGEL, J., AND McGuire, T. W. 1984. Social psychological aspects of computer-mediated communication. Am. Psychol. 39, 1123–1134.
- KINNEAR, T. C. AND TAYLOR, J. R. 1991. Marketing Research: An Applied Approach. McGraw Hill, New York.
- KLING, R. 1980. Social analyses of computing: Theoretical perspectives in recent empirical research. *ACM Comput. Surv. 12*, 1, 61–110.
- KOHLER, W. 1981. A survey of techniques for synchronization and recovery in decentralized computer systems. ACM Comput. Suru. 13, 2, 149–183.
- KORNFELD, W. A. 1982. Combinatorially Implosive Algorithms. Commun. ACM 25, 10, 734–738.

- KORNFELD, W. A. AND HEWITT, C. 1981. The scientific community metaphor. *IEEE Trans. Syst. Man. Cybernet. SMC-11*, 24–33.
- KRAEMER, K. AND KING, J. L. 1988. Computer-based systems for cooperative work and group decision-making. ACM Comput. Suru. 20, 2, 115-146.
- Kurose, J. F. and Simha, R. 1989. A microeconomic approach to optimal resource allocation in distributed computer systems. *IEEE Trans. Comput.* 38, 5, 705–717.
- Lai, K. Y., Malone, T., and Yu, K.-C. 1988. Object Lens: A spreadsheet for cooperative work. *ACM Trans. OfficeInf. Syst.* 6, 4, 332–353.
- LAWRENCE, P. AND LORSCH, J. 1967. Organization and Environment. Division of Research, Harvard Business School, Boston.
- LEAVITT, H. J. AND WHISLER, T. L. 1958. Management in the 1980's. *Harvard Bus. Rev.* 36, (Nov./Dec.), 41-48.
- LEE, J. 1990. Sibyl: A qualitative decision management system. In *Artificial Intelligence at MIT: Expanding Frontiers*. Vol. 1. MIT Press, Cambridge, Mass.
- LEE, J. AND MALONE, T. W. 1990. Partially shared views: A scheme for communicating among groups that use different type hierarchies. ACM Trans. Inf. Sys. 8, 1, 1-26.
- LISKOV, B. AND GUTTAG, J. 1986. Abstraction and Specification in Program Development. MIT Press, Cambridge, Mass.
- LOTUS. 1989. Lotus Notes Users Guide. Lotus Development Corp., Cambridge, Mass.
- LUMER, E. AND HUBERMAN, B. A. 1990. Dynamics of resource allocation in distributed systems. Tech. Rep. SSL-90-05. Xerox PARC, Palo Alto, Calif.
- MALONE, T. W. 1992. Analogies between human organization and artificial intelligence systems: Two examples and some reflections. In Distributed Intelligence: Perspectives of Artificial Intelligence on Organization and Management Theory. Elsevier, Amsterdam.
- MALONE, T. W. 1990. Organizing information processing systems: Parallels between organizations and computer systems. In *Cognition, Computation, and Cooperation*. Ablex, Norwood, N.J., 56–83.
- MALONE, T. W. 1988. What is coordination theory. Working Paper no. 2051-88. MIT Sloan School of Management, Cambridge, Mass.
- MALONE, T. W. 1987. Modeling coordination in organizations and markets. *Manage. Sci. 33*, 1317–1332.
- MALONE, T. W. AND CROWSTON, K. G. 1991. Toward an interdisciplinary theory of coordination. Tech. Rep. no. 120. Massachusetts Institute of Technology, Center for Coordination Science, Cambridge, Mass.
- MALONE, T. W. AND CROWSTON, K. 1990. What is coordination theory and how can it help design

- cooperative work systems. In *Proceeding of the Third Conference on Computer-Supported Cooperative Work*. ACM Press, New York, 357–370
- MALONE, T. W. AND ROCKART, J. F. 1991. Computers, networks, and the corporation. Sci. Am. 265, 3 (Sept.), 128–136.
- MALONE, T. W. AND SMITH, S. A. 1988. Modeling the performance of organizational structures. *Oper. Res.* 36, 3, 421–436.
- Malone, T. W., Crowston, K., Lee, J., and Pentland, B. 1993. Tools for inventing organizations: Toward a handbook of organizational processes. In *Proceedings of the 2nd IEEE Workshop on Enabling Technologies Infrastructure for Collaborative Enterprises*. IEEE, New York.
- MALONE, T. W., FIKES, R. E., GRANT, K. R., AND HOWARD, M. T. 1988. Enterprise: A marketlike task scheduler for distributed computing. In *The Ecology of Computation*. North-Holland, New York.
- MALONE, T. W., GRANT, K. R., TURBAK, F. A., BROBST, S. A., AND COHEN, M. D. 1987a. Intelligent information-sharing systems *Commun. ACM* 30, 390-402
- MALONE, T. W., LAI, K.-Y., AND FRY, C. 1992. Experiments with Oval: A radically tailorable tool for cooperative work. In *Proceedings of the ACM Conference on Computer-Supported Cooperative Work* (CSCW '92). ACM, New York.
- MALONE, T. W, YATES, J., AND BENJAMIN, R. I. 1987b. Electronic markets and electronic hierarchies *Commun. ACM 30*, 484-497
- MANGEL, M. AND CLARK, C. W. 1988. Dynamic Modeling in Behavioral Ecology. Princeton University Press, Princeton, N.J.
- MARCH, J. G. AND SIMON, H. A. 1958. Organizations. John Wiley and Sons, New York.
- Markus, M. L. and Connolly, T. 1990 Why CSCW applications fail: Problems in the adoption of interdependent work tools. In *Proceedings of the 3rd Conference on Computer-Supported Cooperative Work*. ACM Press, New York, 371–380.
- MARSCHAK, J. AND RADNER. R. 1972. Economic Theory of Teams. Yale University, New Haven,
- McClain, J., Thomas, L. J., and Mazola, J. 1992. Operations Management. 3rd ed. Prentice-Hall, Englewood Cliffs, N.J.
- McGrath, J. E. 1984. *Groups: Interaction and Performance*. Prentice-Hall, Englewood Cliffs, N.J.
- MIAO, X., LUH, P. B., AND KLEINMAN, D. L. 1992. A normative-descriptive approach to hierarchical team resource allocation. *ZEEE Trans. Syst. Man. Cybernet.* 22, 3, 482–497.
- MILGROM, P. 1981. An axiomatic characterization of common knowledge. *Econornetrica* 49, 1, 17–26.

- MILLER, J. G. 1978. Living Systems. McGraw-Hill, New York.
- MILLER, M. S. AND DREXLER, K. E. 1988. Markets and computation: Agoric open systems. In *The Ecology of Computation*. North-Holland, Amsterdam, 133–176.
- MINTZBERG, H. 1979. The Structuring of Organizations. Prentice-Hall, Englewood Cliffs, N.J.
- Moses, J. 1990. Organization and ideology. Unpublished Manuscript. Dept. of Electrical Engineering and Computer Science, Massachusetts Institute of Technology, Cambridge, Mass.
- MYERSON, R. B. 1981. Optimal auction design. Math. Oper. Res. 6, 58-73.
- Neuwirth, C. M., Kaufer, D. S., Chandhok, R., and Morris, J. H. 1990. Issues in the design of computer-support for co-authoring and commenting. In *Proceedings of the 3rd Conference on Computer Supported Cooperative Work* (CSCW 90). ACM Press, New York, 183–195.
- NII, P. 1986. The blackboard model of problem solving. AI Mug. (Spring), 38–53.
- NATIONAL SCIENCE FOUNDATION 1991. Coordination Theory and Collaboration Technology Workshop Summary (June 3–5). National Science Foundation, Washington, D.C.
- NATIONAL SCIENCE FOUNDATION 1989. A report by the NSF-IRIS Review Panel for Research on Coordination Theory and Technology. NSFF Forms and Publication Unit, National Science Foundation, Washington, D.C.
- ORLIKOWSKI, W 1992. Learning from notes: Organizational issues in groupware implementation. In Proceedings of the Conference on Computer Supported Cooperative Work (CSCW 92). ACM, New York
- Peterson, D., Eds. 1986. Proceedings of the Conference on Computer-Supported Cooperative Work. ACM. New York.
- Peterson, J. L. 1981. Petri Net Theory and the Modeling of Systems. Prentice-Hall, Englewood Cliff, N.J.
- Peterson, J. L. 1977. Petri nets. *ACM Comput. Surv.* 9, 3, 223–252.
- Pfeffer, J. 1978. Organizational Design. Harlan Davidson, Arlington Heights, Ill.
- PFEFFER, J. AND SALANCIK, G. R. 1978. The External Control of Organizations: A Resource Dependency Perspective. Harper and Row, New York
- REITER, S. 1986. Informational incentive and performance in the (new)<sup>2</sup> welfare economics. In *Studies in Mathematical Economics*. Studies in Mathematics, volume 25. Mathematical Association of America.
- RESCHER, N. 1977. Dialectics. A Controversy-Oriented Approach to the Theory of Knowledge. State University of New York Press, Buffalo, N.Y.
- RITTEL, H. AND KUNZ, W. 1970. Issues as elements of information systems. Working paper

- 131. University of Stuttgart, Institut fur Grundlagen der Planung I.A., Stuttgart, Germany.
- ROBERTS, K. H. AND GARGANO, G. 1989. Managing a high reliability organization: A case for interdependence. In *Managing Complexity in High Technology industries: Systems and People*. Oxford University Press, New York, 147–159.
- ROBERTS, K. H., STOUT, S. K., AND HALPERN, J. J. 1994. Decision dynamics in two high reliability military organizations. *Manage. Sci.*
- ROCKART, J. F. AND SHORT, J. E. 1989. IT and the networked organization: Toward more effective management of interdependence. In *Management in the 1990s Research Program Final Report*. Massachusetts Institute of Technology, Cambridge, Mass.
- ROGERS, E. AND AGARWALA-ROGERS, R. 1976.

  Communication in Organizations. Free Press,
  New York
- Ross, S. 1973. The economic theory of agency. *Am, Econ. Rev.* **63,** 134–139.
- RUMELHART, D. E., McCLELLAND, J. L. AND PDP RESEARCH GROUP. 1986. Parallel Distributed Processing: Explorations in the Microstructures of Cognition. MIT Press, Cambridge, Mass.
- SCHELLING, T. C. 1978. Micromotives and Macrobehavior. Norton, New York.
- Schelling, T. C. 1960. Strategy of Conflict. Harvard University Press, Cambridge, Mass.
- SCHONBERGER, R. 1986. World Class Manufacturing. Free Press, New York.
- Schonberger, R. 1982. *Japanese Manufacturing Techniques*. Free Press, New York.
- Schuler, D. and Namioka, A., Eds. 1993. Participatory Design: Principles and Practices. Lawrence Erlbaum, Hillsdale, N.J.
- SEARLE, J. R. 1975. A taxonomy of illocutionary acts. In *Language, Mind and Knowledge*. University of Minnesota, Minneapolis, Minn., 344–369.
- SEELEY, T. D. 1989. The honey bee colony as a superorganism. *Am. Sci.* 77, (Nov.-Dec.), 546-553.
- SHANNON, C. E. AND WEAVER, W. 1949. The Mathematical Theory of Communication. University of Illinois Press, Urbana, Ill.
- SHOHAM, Y. 1994. Agent oriented programming. J. Artif. Intell.
- SIMON, H. A. 1981. Sciences of the Artificial. 2nd ed. MIT Press, Cambridge, Mass.
- SIMON, H. A. 1976. Administrative Behavior. 3rd ed. Free Press, New York.
- SINGH, **B.** 1992. Interconnected Roles (IR): A coordinated model. Tech, Rep. CT-84-92. Micro-

- electronics and Computer Technology Corp., Austin, Tex.
- SINGH, B. AND REIN, G. L. 1992. Role Interaction Nets (RIN): A process description formalism. Tech. Rep. CT-083-92. Microelectronics and Computer Technology Corp., Austin, Tex.
- SMITH, A. 1776. *The Wealth of Nations*. 1986 ed. Penguin Books, London.
- SMITH, R. G. AND DAVIS, R. 1981. Frameworks for cooperation in distributed problem solving. *IEEE Trans. Syst. Man. Cybernet.* 11, 1, 61–70.
- STANKOVIC, J. 1985. An application of Bayesian decision theory to decentralized control of job scheduling. *IEEE Trans. Comput. C-34*, 2, 117–130.
- STEFIK, M., FOSTER, G., BOBROW, D. G., KAHN, K., LANNING, S., AND SUCHMAN, L. 1987. Beyond the chalkboard: Computer support for collaboration and problem solving in meetings. *Commun. ACM* 30, 1, 32–47.
- STODDARD, D. 1986. OTISLINE. Case 9-186-304. Harvard Business School, New Haven. Conn.
- TANNENBAUM, A. S. 1981. Computer Networks. Prentice-Hall, Englewood Cliffs, N.J.
- Tatar, D. Eds. 1990. Proceedings of the 3rd Conference on Computer-Supported Cooperative Work. ACM Press. New York.
- TATAR, D., EDS. 1988. Proceedings of the 2nd Conference on Computer-Supported Cooperative Work. ACM Press, New York.
- THOMPSON, J. D. 1967. Organizations on Action: Social Science Bases of Administrative Theory. McGraw-Hill, New York.
- Toffler, A. 1970. Future Shock. Bantam Books, New York.
- Toulmin, S. 1958. The Uses of Argument. Cambridge University Press, Cambridge, England.
- TUROFF, M. 1983. Information. value, and the internal marketplace. Unpublished manuscript. New Jersey Institute of Technology, Newark, N.J.
- WALDSPURGER, C. A., HOGG, T., HUBERMAN, B. A., KEPHART, J. O., AND STORNETTA, S. 1988. Spawn: A distributed computational ecology. Unpublished Working Paper. Xerox PARC, Palo Alto, Calif.
- WEICK, K. E. 1969. The Social Psychology of Organizing. Addison-Wesley, Reading, Mass.
- WILLIAMSON, O. 1985. The Economic Institutions of Capitalism. Free Press, New York.
- WILLIAMSON, O. E. 1975. Markets and Hierarchies. Free Press, New York.
- Winograd, T. 1987. A language/action perspective on the design of cooperative work. *Hum Comput. interaction.* 3, 3-30.
- WINOGRAD, T. AND FLORES, F. 1986. Understanding Computers and Cognztion: A New Foundation for Design. Ablex, Norwood, N.J.

Received May 1991; final revision accepted July 1993.