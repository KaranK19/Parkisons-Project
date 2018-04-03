# Parkisons-Project

# Introduction
This problem set will be an exercise in integrative genomics. First we will learn how Genome-Wide Association Studies (GWAS) work. Then we will learn how to find differential genes between colorectal cancer tumor/normal samples in a functional genomics example.

# PART 1: GWAS
To study the problem of Parkinson’s Disease, you have the raw data from two experiments. You will need to analyze these experimental raw data and integrate the results.
This publication describes a genome-wide association study on Parkinson's Disease. More than 408,000 single nucleotide polymorphisms (SNPs) were measured (or genotyped) across 276 patients with Parkinson’s Disease, and 276 normal control individuals. Each SNP is a potentially differing nucleotide between individuals. Recall that there are estimated to be as many as 10 million SNPs in the human genome, so this collection does not encompass all of them.
The raw data for this study are here:
* https://queue.coriell.org/Q/ninds_upload/6/Original/pd_pre.zip
* https://queue.coriell.org/Q/ninds_upload/6/Original/pd_map.zip
* https://queue.coriell.org/Q/ninds_upload/4/Original/cc_pre.zip
* https://queue.coriell.org/Q/ninds_upload/4/Original/cc_map.zip
The cc subdirectory indicates data for the Caucasian control individuals, while the pd subdirectory indicates data for the individuals with Parkinson's Disease.

# Method & Outcome
We can first use the chi-squared test to determine whether the genotype distribution seen in Parkinson’s Disease patients is different than control individuals (i.e. a case-control study). A chi-squared test for these data with 2 degrees of freedom yields a p-value of 6.301 x 10-6, indicating that it is highly unlikely that the Parkinson’s Disease distribution matches the control distribution. A Fisher-exact test could also be used, yielding similar results. Either way, this would indicate that the genotype distributions are significantly associated with the presence of Parkinson’s Disease.

# Envoirnment

R-Studio(R-Programming)
