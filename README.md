# community-smells
A repository to collect articles on community smells

# Concept

After finding a beautiful heatmap on Rude [Compounds on Reddit](https://www.reddit.com/r/dataisbeautiful/comments/vmw0eu/oc_frequency_of_compound_insults_eg_poophead/), I wondered how this could be extended to a research topic. Github have some figures on [Sustainable communities](https://octoverse.github.com/#sustainable-communities), suggesting that *teams with high trust are more likely to have a healthy collaborative culture*:

> Developing is about community. Codes of conduct, contribution guidelines, Good First Issues, and respectful language in Discussions signal a community is safe, welcoming, and trusted. Communities with these signals attract more contributors, while also creating a stronger sense of belonging and fulfillment.

Wouldn't it be neat to quantize how programmers benefit from sustainable communites? There is some [related research](https://scholar.google.se/scholar?cites=17946175484241396803&as_sdt=2005&sciodt=0,5&hl=sv) on the topic, regarding a phenomena called *community smells*. The research has potential to be interdisciplinary; depending angle of incidence I could collaborate with anthropologists and linguists. 

In this repository I am going to put summaries of papers and ideas that might lead to a scientific paper on the subject. The end-goal is to promote civil communication.

# TODO
* Read on science regarding "online comments" (eg [this paper](https://onlinelibrary.wiley.com/doi/abs/10.1111/jcom.12104), or [this](https://arxiv.org/pdf/1809.00289.pdf) and [this](https://www.tandfonline.com/doi/abs/10.1080/10510974.2017.1397038))

* Investigate the keyword "social etiquette" of the techworld.

* [An attempt to map users from github issues](https://elib.uni-stuttgart.de/handle/11682/10641). Sounds interesting. 

* [Bug predicting](https://link.springer.com/article/10.1007/s11219-020-09538-7)

# Articles 

### [The "Shut the f** k up" Phenomenon: Characterizing Incivility in Open Source Code Review Discussions](https://dl.acm.org/doi/abs/10.1145/3479497)

Analyzes 1,545 emails from the **Linux Kernel Mailing List** (LKML) concerning rejected patches. 

> We found that more than half (66.66%) of the non-technical emails included uncivil features [in the Linux Kernel Mailing List].
> We also found that there are civil alternatives to address arguments. 

A majority of non-technical emails include seemingly unnecessary "uncivil features". Are programmers rude by nature? 🤔

* The workload on the Linux kernel is exceptional with hundreds of emails per day and maintainer. 
* Quality of contributions are very diverse, which might affect the maintainers mood. 
* Many authors [16, 39, 55] believe that “incivility is in the eye of the beholder”; 
* **Results:** Identify "Tone-bearing discussion features", and categorize them as "positive", "neutral", "negative", and "uncivil".
* Although the Linux Kernel has a Code of Conduct, incivility is still present. The article calls for other means to tackle the problem of uncivil communication in the context of software development. 

### [“Did You Miss My Comment or What?” Understanding Toxicity in Open Source Discussions](https://www.cs.cmu.edu/afs/cs.cmu.edu/Web/People/ckaestne/pdf/icse22_toxicity.pdf)
> **NOTE**: Not cited in [bib](docs/bib/bibliography.bib)

### [How heated is it? Understanding GitHub locked issues](https://arxiv.org/abs/2204.00155)
> **NOTE**: Not cited in [bib](docs/bib/bibliography.bib)

### [Litterature review](https://www.sciencedirect.com/science/article/pii/S0950584922001872?dgcid=rss_sd_all) setting up a taxonomy and calling for more reserach on the field. Good quote: "Community smells are sociotechnical anti-patterns and one source of social debt."

Use cancer framework to diagnose community smells:
> We used the National Cancer Institute’s framework for the stages of cancer (a chronic condition)1 to represent the origin and evolution of community smells. This stage-based representation can help teams diagnose the status of community smells as their effects worsen and spread. The first author developed the initial version of the framework. The second author reviewed and suggested adjustments to arrive at the final version.

**Social Debt**: [...] define social debt as “unforeseen project costs connected to a suboptimal development community”. An extension suggest that social debt leads to technical debt (perhaps obvious?)

Components of social debt:
> Socio-technical decisions, community smells, sub-optimal team organizational, and sub-optimal social structures.

They present the 30 most common community smells:

<details>
<summary> Community smells (opens a BIG table 😵‍💫)</summary>

|    | Community smell             | Description                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|----|-----------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1  | Architecture by osmosis     | This smell describes people making architecture decisions based on inappropriate information management. While some teammates manage and filter information through undefined communication channels or methods, others use different standards to document change requests. These actions cause problems with locating architecture decision sources, waste of time, and unstable architecture configuration [20].                           |
| 2  | Architecture hood           | The smell emerges when decision-making teams in charge of architecture decisions work remotely or distant from teammates. Thus, cooperation is challenging. Developers cannot exchange communications with the software architects responsible for those decisions causing implementation problems [5].                                                                                                                                       |
| 3  | Black cloud                 | This smell is present when organizations do not provide the conditions for social interactions and effective communication between teammates. Thus, the conditions do not support the exchange of knowledge during software development processes, e.g., professional experience or understanding of projects in progress [5], [10].                                                                                                          |
| 4  | Class cognition             | In this smell, refactoring makes the modular structures and refactored classes more difficult to understand. Thus, other teammates, including current developers and newcomers, spend time and effort understanding the new environment version and file locations [10].                                                                                                                                                                      |
| 5  | Code red                    | It is a smell denoting the existence of highly complex classes. Thus, a limited number of developers, i.e., 1–2 people at most, can manage such classes [10].                                                                                                                                                                                                                                                                                 |
| 6  | Cognitive distance          | In software engineering, it is the distance that developers perceive on the physical, technical, social, and cultural levels concerning peers with considerable background differences. The effects are associated with, for example, resource management issues, conflicts among teammates, and code smells [42].                                                                                                                            |
| 7  | Cookbook development        | Developers are stuck in how they usually work according to old-framework-based cookbooks, e.g., the waterfall model. They do not accept innovative ideas or new ways of working, e.g., agile methods, that change their comfort zones. Consequently, software product features do not fulfill customer’s expectations [42].                                                                                                                   |
| 8  | DevOps clash                | The smell describes clashes between development and operations teams from multiple geographical locations with contractual obligations to either development or operations activities. These clashes lead to a slower development process and ineffective operations [42].                                                                                                                                                                    |
| 9  | Disengagement               | It is a situation where developers think the software product is mature enough. Then they send it to operations technicians even though the software is unfinished. This circumstance reflects a lack of curiosity from the developers’ side, ending in missing software features or applying wild assumptions [42].                                                                                                                          |
| 10 | Dispersion                  | This community smell concerns a fix or refactoring that causes the fragmentation of an existing group, working in or being part of a collaboration network. Functionality rearrangements also lead to haphazard work. Finally, coordinating and carrying out maintenance activities is more challenging [10].                                                                                                                                 |
| 11 | Dissensus                   | It is the inability to achieve consensus on how to proceed despite repeated attempts at doing it. Therefore, code smells detected in software components remain without the required adjustments [10].                                                                                                                                                                                                                                        |
| 12 | Hyper community             | The smell refers to a highly connected community sensible to groupthink. It also influences smaller subcommunities in its network. Consequently, it leads to social turbulence and faulty software components [42].                                                                                                                                                                                                                           |
| 13 | Informality excess          | Excessive informality is the relative absence of information management and control protocols. These conditions lead to information spillover and low accountability of teammates [42].                                                                                                                                                                                                                                                       |
| 14 | Institutional isomorphism   | It is the similarity of processes or structures of one software development group or sub-community to those of another. This condition can be the result of imitation or independent development under the same constraints. The effects can include lack of innovation, stagnancy, and communication [42].                                                                                                                                   |
| 15 | Invisible architecting      | It is a situation in which teammates document software architecture decisions and register meeting agreements inconsistently. Consequently, the descriptions of such decisions, necessary for the software architecture process, become invisible. The lack of accurate information generates, for example, decision unawareness and conflicts among teammates [20].                                                                          |
| 16 | Leftover techie             | This smell consists of a broken collaborative network. Also, there is no effective communication between developers and technicians (e.g., help desk, operation, and maintenance). The technicians are not usually involved in multiple aspects of the software development process to have a shared knowledge of software features [5].                                                                                                      |
| 17 | Lone wolf                   | This smell occurs when defiant teammates carry out their work irrespective or regardless of their peers. This smell reflects poor communication addressing project needs. The effects are, for instance, unsanctioned architecture decisions across the development process, code smells, and project delays [11], [12].                                                                                                                      |
| 18 | Lonesome architecting       | Non-architect teammates see the need to make architecture decisions because the current architects are too few and far apart. These non-architects make decisions without consulting with experts involved in such decisions. From a social perspective, developers are unaware of what they are doing. Also, this scenario leads to incompatibility problems and faster decision-making [20].                                                |
| 19 | Newbie free-riding          | Newcomer teammates must understand by themselves what to do and for whom, which leads to the free-riding of older employees. This unfriendly work environment adds more pressure to the team and affects people’s psychological state [42].                                                                                                                                                                                                   |
| 20 | Obfuscated architecting     | It occurs when multiple subteams of a development network lack the organizational and the socio-technical vision required for harmonized operations. For instance, projects need new developers to implement changes to legacy and new products. However, newcomers included in projects lack the technical background to deal with legacy products. Among effects, teams faced waste of time, code smells, and developers’ frustration [20]. |
| 21 | Organizational silo         | This community smell is associated with task coordination problems. Software development tasks are sometimes not interconnected with each other. This smell sets challenges to check task dependencies and non-conducive conditions for effective communication among teammates performing tasks. This scenario puts the socio-technical congruence at risk [5], [11].                                                                        |
| 22 | Organizational skirmish     | An organizational skirmish is a scenario where teams have differences over their organizational cultures. It makes the work of project managers difficult. The impact is notorious on productivity, e.g., project delays [5].                                                                                                                                                                                                                 |
| 23 | Power distance              | The distance that less powerful software development teammates perceive with those power-holder teammates, e.g., experienced teammates or decision-makers. It finally disrupts the software process and impacts organizational finances [42].                                                                                                                                                                                                 |
| 24 | Priggish members            | They are pedant teammates demanding of others pointlessly precise conformity or exaggerated propriety, which is annoying. The attitude frustrates teammates and affects the software process [42].                                                                                                                                                                                                                                            |
| 25 | Prima donnas                | This smell indicates the presence of teammates working in isolation. They are unwilling to welcome the change of legacy products and support from other teammates. These teammates prevent the organization from innovative solutions or processes and effective communication and collaboration [5].                                                                                                                                         |
| 26 | Radio silence or Bottleneck | It is a scenario where leaders and teammates perform tasks in very formal and complex organizations. Under these conditions, team communication structures are not conducive to spread information across the teams efficiently. For instance, a person working as a unique information intermediary for different teams leads to communication overload and massive delays [5], [11].                                                        |
| 27 | Sharing villainy            | This community smell depicts work environments where the goal of sharing reliable knowledge or information is a challenge. Organizations do not provide the expected conditions for knowledge sharing, like opportunities for meetings and incentives. Hence, some teammates do not see knowledge sharing as a productive activity for projects’ completion [5].                                                                              |
| 28 | Solution defiance           | This smell describes conflicts between teams. Teammates with similar deep-level factors (e.g., technical background) and organizational cultural beliefs (e.g., values and norms) create subteams. Then they go into conflicts in decision-making meetings since every group supports their opinions on potential solutions [5].                                                                                                              |
| 29 | Time warp                   | After changes in organizational structures and processes, experienced teammates wrongly assume time frames for exchanging communications and no need for explicit coordination. Some effects of this community smell are unsatisfied customers and faulty software [42].                                                                                                                                                                      |
| 30 | Unlearning                  | Components of training courses, e.g., technological innovations and best practices, become unfeasible learning material when it is shared with older teammates. These teammates show a very high experience diversity. Consequently, the updated accumulated knowledge is at risk of being gradually lost [42].                                                                                                                               |

</details>

The researchers claim it is possible to quantify some community smells with statistical tools:

>  The study evaluated four community smells, Black cloud, Lone wolf, Organizational silo, and Radio silence and five code smells, long method, feature envy, blob class, spaghetti code, and misplace class. **Examples of technical and socio-technical factors used in this study are lines of code, total commits, truck-factor, and developers turnover**.

Ch 4.3.3 is interesting when it comes to measuring. They cite a [report in bug prediction](https://scholar.google.com/scholar_lookup?title=An%20empirical%20study%20on%20the%20effect%20of%20community%20smells%20on%20bug%20prediction&publication_year=2021&author=B.%20Eken&author=F.%20Palma&author=B.%20Ayşe&author=T.%20Ayşe) that tried to predict future costs by using community smells. Not super-successful, but some significance was found:

> The authors found that both code and community smells are good indicators in bug prediction models, but the performance of the models depends on project features and validation strategies.

They keep on citing more sources and concluding women have a great impact on socio-technical debt:

> The results showed community smell instances are lower in gender-diverse teams. Women play a significant role in reducing community smells that affect communication and coordination. 
