![](_page_0_Picture_0.jpeg)

![](_page_0_Picture_1.jpeg)

# Howopen sourcemaintainers keep contributors—and

# themselves—happy

IT'S NEVER TOO EARLY OR TOO LATE TO START THINKING ABOUT CONTRIBUTOR RELATIONS.

KLINT FINLEY // JULY 22, 2021

**The ReadME Project** amplifies the voices of the open source community: the maintainers, developers, and teams whose contributions move the world forward every day.

Contributor relation wa a hot topic at the Global [Maintainer](https://globalmaintainersummit.github.com/) [Summit](https://globalmaintainersummit.github.com/) event hoted by GitHub on June 8-9 2021. The event organizer, GitHub developer advocate Kara Sowle and Brian Dougla, dedicated ix eion to the ubject.

![](_page_1_Picture_5.jpeg)

aintainr do th havy liting in opn ourc, pnding countl hour ixing bug, mrging pull rqut, triaging iu, and providing upport. But community contribution ar hat rally mak opn ourc pcial. From inightul

uggtion to complx tchnical atur, popl rom around th orld contribut thir kill and prpctiv to mak opn ourc otar bttr. "All th ork do a maintainr i mad poibl ith th hlp o our community o contributor,["](https://github.com/tern-tools/tern) [Trn](https://github.com/tern-tools/tern) comaintainr Ro Judg aid during hr talk at th Global aintainr Summit. Indd, thi talnt pool i th raon o many individual and organization opn ourc otar in th irt plac.

aintainr truggling to [balanc](https://github.com/readme/octoverse-balance) thir opn ourc ork ith th rt o thir liv can bnit gratly rom th kill and prpctiv o contributor. Contributor can hlp rduc maintainr' orkload by ixing bug or implmnting atur, and it ould b impoibl or many projct to cal up to mt th nd o ur ithout robut contributor communiti.

But rviing contribution, modrating dicuion on iu and propoal, and managing communiti crat n rponibiliti or maintainr a contributor communiti gro. Popular projct can attract o many propctiv contributor that maintainr hav to pnd mor tim coordinating thir activiti than riting cod. In hr book on opn ourc, Working in Public, rarchr and author Nadia Eghbal point out that or many dvlopr, contributing to a popular projct i a mark o ditinction. "I tartd to th problm i not that thr' a darth o popl ho ant to contribut to an opn ourc projct, but rathr that thr ar too many contributor—or thy'r th rong kind o contributor," Eghbal rot.

Finding ay to attract nough contributor to utain projct hil caling-up contributor rlation i on o th grat challng acing today' maintainr.

![](_page_2_Picture_3.jpeg)

#### Community building

Having too many contributor may ound lik a lcom problm to n maintainr truggling to attract contribution.

During hi kynot[,](https://github.com/kubernetes/kubernetes) [Kubrnt](https://github.com/kubernetes/kubernetes) co-oundr Brndan Burn mphaizd th nd to mak ur projct look a activ a poibl o that potntial contributor don't aum thy'v bn abandond. That man puhing n cod rquntly.

But it' not nough to jut look activ. Burn alo mphaizd th nd to rpond quickly to qution and pull rqut, a concrn Judg highlightd a ll. I you tak too long, a potntial ur or contributor may mov on. Organization ith uicint rourc can aign ta to rpond to GitHub Iu, or vn crat an on-call chdul. Individual maintainr hould jut do thir bt. "Thi i not to ay you houldn't tak a brak," Judg aid. "Jut communicat to th community hat thy can xpct hil you'r aay."

ultipl pakr undrcord th nd to b lcoming. "Popl undrtimat ho important and ho hard thi i," Burn aid. H point out that although you might b tird o anring th am qution ovr and ovr, n ur and contributor on't kno that. Snapping at omon or aking an innocnt qution ill lav a bad imprion o you and your projct.

In hr talk on contributor incntiv, [FOSSASIA](https://fossasia.org/) oundr Hong Phuc Dang pointd out that tchnology choic can play a big rol in hat projct popl ill ant to contribut to. For xampl, h mntiond that uin[g](https://github.com/readme/react) [Ract.j,](https://github.com/readme/react) intad o lrknon ur intrac librari, might hlp attract mor talnt inc thr i a hug ba o dvlopr ho ar alrady amiliar ith it and many mor ho ant to larn it.

Cah paymnt ar on obviou bnit that jut about anyon ill apprciat. But Dang mphaiz that rcognition i alo an important incntiv or contributor. For xampl, FOSSASIA highlight contribution rom individual in ocial mdia pot, nlttr, and othr communication o that vryon gt om rcognition or th ork thy do. Giving contributor th opportunity to tak on mor rponibiliti, hthr that' mrg acc or having thm hlp onboard n contributor, i anothr porul motivator. "Whn popl gt mor rponibiliti thy bcom mor ngagd and mor xcitd about th projct," Dang ay.

#### Bttr contribution through automation

Triaging th ork o contributor and maintaining a community i an normou amount o ork. Kping opn ourc projct, and thir maintainr, halthy rquir a bigger investment in paying the people who do the work to keep the projects we all rely on running.

Rust Foundation Interim Executive Director Ashley Williams urged companies to hire more maintainers to work full-time on their projects. "There's no difference between investing in technology and investing in its people," she said. The Rust Foundation is experimenting with a new spin on open source foundation sponsorship. Instead of donating money to the Rust Foundation, companies can become sponsors by hiring maintainers to work on Rust.

But even full-time maintainers can end up overwhelmed. "There's generally more work than anyone can actually do," Paulus Schoutsen, maintainer of <u>Home Assistant</u>, cautioned. Because there's a potentially infinite number of things maintainers can spend time on, the key is being strategic about what you do and, more importantly, don't do. Multiple speakers emphasized the importance of avoiding scope creep in projects. "Every extra line of code means more of a support burden," said <u>Prometheus</u> maintainer Bartłomiej Płotka. New features need documentation and tests, and increase the number of questions users have.

Multiple speakers shared their approach to automation, a popular strategy to help maintainers manage contributions. Linters and code formatters are particular favorites. AutoFormating also lowers barriers to entry since contributors are less likely to have code rejected over stylistic preferences. Homebrew maintainer Mike McQuaid noted that shifting to an automated code review process meant fewer arguments over minor details. "We weren't being accused, as maintainers, of being pedantic anymore," he said.

Python core maintainer <u>Mariatta Wijaya</u> shared some of the custom bots her team uses to make reviewing contributions easier. For example, the "<u>Knights Who Say Ni</u>" verifies whether the contributor license agreement has been signed and, if not, blocks the submission until it has. Meanwhile, the "<u>Bedevere</u>" closes invalid pull requests and identifies problems such as missing issue numbers, while "<u>Miss-islington</u>" automatically backports approved pull requests.

Schoutsen recommended using <u>GitHub Actions</u> to automate tasks like locking old pull requests and automatically closing stale issues. Closing old pull requests and issues without resolving them might seem unfriendly, but Schoutsen points out that having lots of unresolved requests will make your project look like it isn't being maintained. And it could make it harder to respond to new requests in a timely fashion. "Keep your

plat clan," h aid. "I iu pil up, you'r l likly to look at thm. So jut clo th old on. I it' important, it ill com up again."

![](_page_5_Picture_1.jpeg)

#### Stting boundari

A cQuaid not, hovr, you can't automat vrything. Som thing, lik oring prai and dback, till nd th human touch.

On o tho thing i aying "no" to contribution. Judg outlind vral raon you might hav to rjct a pull rqut, atur rqut, or othr propoal. For xampl, a propod chang might introduc bug, gnrat tchnical dbt, or inlat th cop o your projct. Somtim you jut on't hav tim to implmnt a atur rqut.

Saying no can b hard, [NgRX](https://github.com/ngrx) maintainr Brandon Robrt notd in hi talk, pcially i you'r uring rom impotr yndrom and orry that you might not mak th right call. "Part o m didn't ant to turn don contribution," h aid. "It' a challng to put that ork in."

But, a Judg ay: "You'r th maintainr or a raon. Somtim th anr i no and you houldn't l guilty or it."

Robrt rcommndd dining a clar viion or your projct to mak it air to mak tough dciion—an ida chod by vral pakr. Th NgRX tam crat dign documnt to communicat th cop and viion o th projct to ur and

contributor. It' air to ay "no" hn omon propo a chang that i outid th dind cop o a projct.

Judg mphaizd that it' alay important to thank popl or thir ork, vn i you'r aying no to a contribution. It' important not to mak rjction pronal. "You ar rjcting th propoal, not th pron bhind it," h aid. Whn poibl, try to phra a rjction a an opportunity to ay y. For xampl, i you don't hav tim to implmnt a chang, uggt thy mak th chang thmlv. "99% o th tim thy'll ay no, but thy might urpri you and it giv thm a chanc to bcom part o th olution," h ay.

Onc again, rpon tim i ky. Th longr you tak to rpond, th mor likly it i you'll dicourag utur participation. Jut bcau omon i propoing omthing unorkabl no don't man thy on't com back ith a bttr ida in th utur.

Thr ar a pic o contributor rlation that ar applicabl to all projct. "B kind" and "tak car o yourl and your popl" ar om o th mot important and univral principl o opn ourc. Byond that, vry maintainr ill nd to ind th tratgi that ork bt or thir projct.

You can atch mor talk rom th [ummit](https://youtube.com/playlist?list=PL0lo9MOBetEEkOyAtPqiupGm91cu8QB0I) to larn mor. By haring thir xprinc through vnt lik th, maintainr ar crating a body o knoldg to hlp ach othr build bttr contributor communiti. It' yt anothr ay th opn ourc community i coming togthr to olv a common problm.

#### or tori

![](_page_7_Picture_0.jpeg)

Coding [acceibility:](https://github.com/readme/featured/accessibility-artificial-intelligence) Building autonomy with AI

FEATURED ARTICLE

![](_page_8_Picture_0.jpeg)

I Laravel the happiet developer [community](https://github.com/readme/featured/laravel-community) on the planet?

FEATURED ARTICLE

![](_page_9_Picture_0.jpeg)

[TypeScript](https://github.com/readme/featured/typescript-gradual-types) and the dawn of gradual type

FEATURED ARTICLE

## About The ReadME Project

Coding i uually n a a olitary activity, but it' actually th orld' largt community ort ld by opn ourc maintainr, contributor, and tam. Th unung hro put in long hour to build otar, ix iu, ild qution, and manag communiti.

Th RadE Projct i part o GitHub' ongoing ort to ampliy th voic o th dvlopr community. It' an volving pac to ngag ith th community and xplor th tori, challng, tchnology, and cultur that urround th orld o opn ourc.

FOLLOWUS:

![](_page_10_Picture_4.jpeg)

![](_page_10_Picture_5.jpeg)

![](_page_10_Picture_6.jpeg)

![](_page_10_Picture_7.jpeg)

### NOMINATE A [DEVELOPER](https://github.com/readme/nominate)

Nominat inpiring dvlopr and projct you think hould atur in Th RadE Projct.

### SUPPORT THE [COMMUNITY](https://github.com/sponsors)

Rcogniz dvlopr orking bhind th cn and hlp opn ourc projct gt th rourc thy nd.