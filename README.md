# community-smells
A repository to collect articles on community smells

# Concept

After finding a beautiful heatmap on Rude [Compounds on Reddit](https://www.reddit.com/r/dataisbeautiful/comments/vmw0eu/oc_frequency_of_compound_insults_eg_poophead/), I wondered how this could be extended to a research topic. Github have some figures on [Sustainable communities](https://octoverse.github.com/#sustainable-communities), suggesting that *teams with high trust are more likely to have a healthy collaborative culture*:

> Developing is about community. Codes of conduct, contribution guidelines, Good First Issues, and respectful language in Discussions signal a community is safe, welcoming, and trusted. Communities with these signals attract more contributors, while also creating a stronger sense of belonging and fulfillment.

Wouldn't it be neat to quantize how programmers benefit from sustainable communites? There is some [related research](https://scholar.google.se/scholar?cites=17946175484241396803&as_sdt=2005&sciodt=0,5&hl=sv) on the topic, regarding a phenomena called *community smells*. The research has potential to be interdisciplinary; depending angle of incidence I could collaborate with anthropologists and linguists. 

In this repository I am going to put summaries of papers and ideas that might lead to a scientific paper on the subject. The end-goal is to promote civil communication.

# TODO
* Read on science regarding "online comments" (eg [this paper](https://onlinelibrary.wiley.com/doi/abs/10.1111/jcom.12104), or [this](https://arxiv.org/pdf/1809.00289.pdf) and [this](https://www.tandfonline.com/doi/abs/10.1080/10510974.2017.1397038))

* [Litterature review](https://www.sciencedirect.com/science/article/pii/S0950584922001872?dgcid=rss_sd_all) setting up a taxonomy and calling for more reserach on the field. Good quote: "Community smells are sociotechnical anti-patterns and one source of social debt."

* Investigate the keyword "social etiquette" of the techworld.

* [An attempt to map users from github issues](https://elib.uni-stuttgart.de/handle/11682/10641). Sounds interesting. 

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
