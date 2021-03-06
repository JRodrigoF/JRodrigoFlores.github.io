---
title: 'Concordance between HLA alleles genotyped using sanger sequencing and Illumina short-reads via Heng Li bwa-alt pipeline'
date: 2018-11-11
permalink: /posts/2018/11/HLA-genotyping-concordance-sanger-illumina/
tags:
  - HLA
  - Illumina
  - Sanger sequening
  - genotyping
  - bwa
  - concordance
---

Genotyping HLA alleles in samples that have been sequenced using Illumina short-reads is a challenging ([Brandt et al (2015)](http://www.g3journal.org/content/5/5/931)) and [non-trivial task](http://genestogenomes.org/the-trouble-with-hla-diversity/). Different approaches have been developed in recent years ([Warren et al (2012)](https://genomemedicine.biomedcentral.com/articles/10.1186/gm396), [Liu et al (2013)](https://academic.oup.com/nar/article/41/14/e142/1750166), [Bai et al (2014)](https://bmcgenomics.biomedcentral.com/articles/10.1186/1471-2164-15-325), [Dilthey et al (2015)](https://www.nature.com/articles/ng.3257#methods), [Xie et al (2017)](http://www.pnas.org/content/114/30/8059.full)). 

Here I tested the accuracy of [Heng Li's approach](https://github.com/lh3/bwa/blob/master/README-alt.md#hla-typing) of using the human genome reference GRC38 with the addition of ALT contigs, decoy sequences, and importantly, an array of ~500 [known HLA haplotypes](https://www.ebi.ac.uk/ipd/imgt/hla/docs/version_r3180.html) taken from the [IPD-IMGT/HLA](https://www.ebi.ac.uk/ipd/imgt/hla/) database (v3.18). I also offer a comparison of whether the genotyping accuracy increases by using the most recent version [v3.34](https://www.ebi.ac.uk/ipd/imgt/hla/docs/version_r3340.html) of the HLA database containing now about ~5000 haplotypes. 

Most probably the new additions correspond to rare haplotypes seen in not so well studied populations, however by increasing the number of HLA haplotypes we increase the power to discriminate between alleles, specially when we try to genotype populations for which the known HLA haplotypes are not so well studied. 

For the comparisons presented here I have used 150 samples from three populations (EUR, EAS, AFR) that have been sequenced by the Polaris project at high-coverage using Illumina sequencing. [See here](https://jrodrigoflores.com/posts/2018/11/Polaris-project-diversity-panel/) for details on the data.


References:

Gourraud, P. 2014. [HLA Diversity in the 1000 Genomes Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0097282)

[bwa/README-alt.md](https://github.com/lh3/bwa/blob/master/README-alt.md#hla-typing)

[The trouble with HLA diversity](http://genestogenomes.org/the-trouble-with-hla-diversity/)
