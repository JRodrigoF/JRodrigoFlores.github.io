---
title: 'Automated identification of human Y chromosome haplogroups based on ancient dna data'
excerpt: "A flexible tool that specifically addresses the shortcomings of ancient dna to identify Y haplogroups in an automated and reliable"
collection: projects
---

A better tool for Y haplogroup identification compared to the existing ones would address the following points:

.- Unlike yHaplo, and similar to YLeaf, the tool would be able to take bam files as input and perform variant calling using either bcftools or GATK. This allows to take into account information on read depth and genotype quality for each SNV and thus provide these metrics in the final assignments. Similar to YFitter, this could allow also to assign haplogroups in a probabilistic way and thus represent the uncertainty in assignment in cases with very low coverage and uncertain (low quality) read mappings.

.- Given a default option based on ISOGG being provided, the tool would also be able to take as input a custom table with variant positions and their names, as well as a custom representation of the Y tree in order to produce results based on this input. YFitter for example works with GRC36 coordinates and an already outdated tree topology. yHaplo on the other hand is heavily dependant on a tree and SNP nomenclature based on ISOGG and GRC37 coordinates, making it not trivial to modify in order to make it work with GRC38 coordinates or with an alternative nomenclature to ISOGG.

.- Similar to yHaplo and YFitter, a hierarchical search based on a pre-defined tree topology should be implemented. This is the main disadvantage of YLeaf, which finds and reports the variants found in a sample and which are linked to a specific haplogroup or sub-branch, but leaves to the user a systematic tree-based analysis of the results. 



References:

[Identifying Y-chromosome haplogroups in arbitrarily large samples of sequenced or genotyped men](https://www.biorxiv.org/content/early/2016/11/19/088716)

[YFitter: Maximum likelihood assignment of Y chromosome haplogroups from low-coverage sequence data](https://arxiv.org/abs/1407.7988?context=q-bio.GN)

[Yleaf: Software for Human Y-Chromosomal Haplogroup Inference from Next-Generation Sequencing Data](https://academic.oup.com/mbe/article-abstract/35/5/1291/4922696?redirectedFrom=fulltext)
