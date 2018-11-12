---
title: 'NNNN[A>T]NNNN: Sequence context-dependant human mutation rates free of recombination effects'
excerpt: "Using a huge number of high-coverage human Y chromosome sequences from different populations, we can assess how frequent certain mutations occur given a particulr sequence context in a free-of-recombination background"
collection: projects
---

"Although mutation is an inherently stochastic process, the distribution of mutations in the human genome is not uniform, and is correlated with genomic and epigenomic features, including local sequence context, recombination rate, and replication timing. Hence, there is considerable interest in studying the regional variation and context dependency of mutation rates to understand the basic biology of mutational processes.

The gold standard for studying the germline mutation rate in humans is direct observation of de novo mutations from family-based whole-genome sequencing (WGS) data. However, the inherently low-germline mutation rate means family-based WGS studies detect only 40–80 de novo mutations per trio sequenced, making it difficult to accumulate a dataset large enough to precisely estimate mutation rates and spectrum at a fine scale and identify factors that explain genome-wide variability in mutation rates.

Other data sources for studying mutation patterns include between-species substitutions or within-species polymorphisms. However, because these variants arose hundreds or thousands of generations ago, their distribution patterns along the genome have been influenced by many evolutionary forces, such as natural selection and GC-biased gene conversion (gBGC), and the fact that mutational processes evolve over time. 

We, therefore, adopt an approach that relies exclusively on extremely rare variants (ERVs) to study innate mutation patterns across the genome. Here, we exploit a collection of ~35.6 million singleton variants discovered in 3560 (European) sequenced individuals ..." 

..... extracts from [Carlson, J. et al 2018](https://www.nature.com/articles/s41467-018-05936-5).

<br/>

Following the previous, we can derive that it is possible to assess relative mutation rates in the human genome and their dependency to particular sequence contexts (3-mer: N[A>T]N , 5-mer: NN[A>T]NN, 7-mer: NNNN[A>T]NNNN ), but in addition to previous approaches, now using a human chromosome which is free of recombination and thus free of the changes in sequence context that this process introduces over a period of 50 generations (around 1244 years), which is the age estimated for the relatively young singletons studied by [Carlson, J. et al 2018](https://www.nature.com/articles/s41467-018-05936-5).

The Y chromose is composed of several ampliconic regions that undergo GC-biased gene conversion (gBGC), so one would need to take those out or better, analyze those in separate and then do the comparison of patterns observed in gBGC-exposed regions vs gBGC-non-exposed regions. The main disadvantage in this study is that even with a huge amount of Y chromosomes, the final number of high-quality singletons is not going to be in the range of ~30 millions and therefore will be a bit underpower to make numbers very robust. On the other hand, one can also analyze SNPs and increase by a magnitude or so the number of mutations. These mutations will have the advantage once again of , even very old, be free of the effects of recombination.





References:

[Carlson, J. et al. Extremely rare variants reveal patterns of germline mutation rate heterogeneity in humans. Nature Communications. 2018](https://www.nature.com/articles/s41467-018-05936-5)

[Evidence for recent, population-specific evolution of the human mutation rate](https://elifesciences.org/articles/24284)
