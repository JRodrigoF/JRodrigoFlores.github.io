---
title: "Truth set reference for the human Y chromosome"
excerpt: "Building a high-confidence call set for Y chromosome SNVs and structural variants based o short and ĺong reads using reference samples"
collection: projects
---

A ’truth set’ can be defined as a sample for which we know all the correct SNVs and structural variants. These high-confidence call sets have been built based on a combination of sequencing approaches such as the integration of short-read Illumina and long-read Pacbio/Nanopore data. Such useful data sets have only been assembled for a few reference samples (NA12878, CEPH family, AshkenazimTrio, etc) and, importantly here, always for the autosomal sections of the genome. Knowing the ’truth’ enables anyone to test any possible combination of QC steps, mappers, callers, variants filters, parameters, etc, and thus assess which combination of them (i.e. in practice, two versions of a snp calling pipeline) gets closer to the 'truth' and therefore happens to be the best for a particular purpose.

In short, the project is to build several ’truth' sets based on data available for samples which have been sequenced using a wide array of technologies (but relevant here: Illumina, PacBio, 10xGenomics and Nanopore). As has been already done for the autosomes, we can integrate the data and build a ’truth’ set for the Y chromosome of these samples. Such resource is not available for the community doing Y chromosome research. 


References:

[https://gatkforums.broadinstitute.org/gatk/discussion/10912/what-is-truth-or-how-an-accident-of-nature-can-illuminate-our-path](https://gatkforums.broadinstitute.org/gatk/discussion/10912/what-is-truth-or-how-an-accident-of-nature-can-illuminate-our-path)

[https://www.nature.com/articles/s41592-018-0054-7](https://www.nature.com/articles/s41592-018-0054-7)

[https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1006834](https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1006834)

[https://jimb.stanford.edu/giab/](https://jimb.stanford.edu/giab/)

[https://www.illumina.com/platinumgenomes.html](https://www.illumina.com/platinumgenomes.html)

[https://ftp-trace.ncbi.nlm.nih.gov/giab/ftp/data/](https://ftp-trace.ncbi.nlm.nih.gov/giab/ftp/data/)

[https://www.ebi.ac.uk/ena/data/view/PRJEB3246](https://www.ebi.ac.uk/ena/data/view/PRJEB3246)

