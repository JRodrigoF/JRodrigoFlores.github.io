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

Genotyping HLA alleles in samples that have been sequenced using Illumina short-reads is a challenging and [non-trivial task](http://genestogenomes.org/the-trouble-with-hla-diversity/). Different approaches have been developed in recent years. 

Here I tested the accuracy of [Heng Li's approach](https://github.com/lh3/bwa/blob/master/README-alt.md#hla-typing) of using the human genome reference GRC38 with the addition of ALT contigs, decoy sequences, and importantly, an array of ~2500 [known HLA haplotypes](https://www.ebi.ac.uk/ipd/imgt/hla/). I also offer a comparison of whether the accuracy increases if the same pipeline is used but with an extended and more recent version of the HLA database which now includes ~5000 haplotypes. 

Most probably the new additions correspond to rare haplotypes seen in not so well studied populations, however is good to keep in mind that by increasing the number of haplotypes in the assembly used, we also increase the power to discriminate between alleles, specially when we try to genotype populations for which the known HLA haplotypes are not so well studied. Here I used [150 samples](https://github.com/Illumina/Polaris) from three populations (EUR, EAS, AFR) that have been sequenced by the Polaris project at high-coverage using Illumina 150bp PE reads.


References:

[HLA Diversity in the 1000 Genomes Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0097282)

[bwa/README-alt.md](https://github.com/lh3/bwa/blob/master/README-alt.md#hla-typing)

[The trouble with HLA diversity](http://genestogenomes.org/the-trouble-with-hla-diversity/)
