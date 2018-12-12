---
title: 'Impact of SNP selection on admixture signals'
date: 2018-11-11
permalink: /posts/2018/11/Impact-of-SNP-selection-on-admixture-signals/
tags:
  - ascertainment bias
  - snp selection
  - admixture
  - human origins array
  - Illumina array
  - Polaris data
---

While SNP ascertainment bias is a well known issue in SNP array-based studies [[Clark et al (2005)](http://doi.org/10.1101/gr.4107905), [Albrechtsen et al (2010)](http://doi.org/10.1093/molbev/msq148), [Lachance et al (2013)](http://doi.org/10.1002/bies.201300014)], I have not been able to find a published study or discussion in the Internet about the impact that SNP selection bias can have on amixture analysis using the software admixture [Alexander et al (2009)](http://doi.org/10.1101/gr.094052.109).

Here I explore this topic by 1) genotyping 150 high-coverage samples from Africa, Europe and East Asia (see [Polaris Diversity Panel](https://jrodrigoflores.com/posts/2018/11/Polaris-project-diversity-panel)), 2) sub-setting the snps to a) all snps found, b) snps in highly reliable and accessible regions of the human genome, c) snps present in the [Illumina Infinium OmniExpress array](https://www.illumina.com/products/by-type/microarray-kits/infinium-omni-express.html), and d) snps present in the Human Origins array.
