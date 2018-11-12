---
title: 'Differences between GATK best practices with and without using free-of-reference bias priors'
date: 2018-11-11
permalink: /posts/2018/11/GATK-best-practices-with-and-without-using-free-of-reference-bias-priors/
tags:
  - GATK
  - reference bias
  - priors
  - genotyping
  - bwa
  - concordance
  - Simons project
---

In the [supplementary section 1](https://media.nature.com/original/nature-assets/nature/journal/v538/n7624/extref/nature18964-s1.pdf) of the Simons Genome Diversity Project, Mallik et al. introduce the use of non-standard (not part of the best practises and default setting of GATK) snp calling priors. The default snp calling priors in GATK they write, "have built-in priors for Bayesian SNP calling that assume that the site is more likely to be homozygous  for  the  reference  allele  than  homozygous  for  the  variant  allele. When there is ambiguity in a heterozygous, GATK prefers the reference homozygous. This is a reference bias, and while this bias is not typically problematic for medical studies*, it can complicate interpretation of population genetics signals ... " 

While this is true, is also worth to keep in mind that this reference bias will be certainly more pronounced in low-coverage data. In this context it seems to make sense that for cases with weak evidence for the heterozygous state, reference homozygous would be favoured. I still need to check how this behaviour was set for the GATK and bcftools pipelines in the 1000G project. For high-coverage data on the other hand, as its the case with the Simons project (~30x Illumina data), one would expect that most of the true heterozygous SNPs will be decently covered and that the evidence for them will be good enough as to make the reference bias less of an issue. But to what extent the impact will be less? Doesn't it make sense that even under a high-coverage context, once again those position not covered so well and with weak evidence for a heterozygous state, better to favour the reference homozygous state?

Certainly the authors of this paper thought it was better to account for the possible bias. In an effort to understand better myself the impact of these modifications and prior differences, here I present a comparison of final genotypes obtained using the standard best practises GATK pipeline, both using default priors and the [values used by Mallik et al]((https://gatkforums.broadinstitute.org/gatk/discussion/11877/free-of-reference-bias-priors-in-haplotypecaller#latest)).

Comparison includes a table with differences in total number of hom-ref, heterozygous, and hom-alt variants.
If the differences are important, a PCA plot would also be included.

* BTW. I am not clear why this would be less problematic for medical studies as compared to population genetics studies. In both cases there would be a negative impact in detriment of the final results. The only possible reason I see on why this would affect to a lesser extend medical studies, is because in these type of studies usually the variants and SNPs in question are concentrated in genic regions, which tend to be complex in sequence (non-repetitive) and also more unique in the genome (with many exceptions of course). These two factors make genic regions easier mapped using short reads and genotype by variant callers. 

References:

[The Simons Genome Diversity Project: 300 genomes from 142 diverse populations](https://www.nature.com/articles/nature18964)

[The Simons Genome Diversity Project: 300 genomes from 142 diverse populations - Supplementary Information](https://media.nature.com/original/nature-assets/nature/journal/v538/n7624/extref/nature18964-s1.pdf)

[GATK forums](https://gatkforums.broadinstitute.org/gatk/discussion/11877/free-of-reference-bias-priors-in-haplotypecaller#latest)
