---
layout: page
title: Main
group: navigation
permalink: "index.html"
---
{% include JB/setup %}

A human-specific AS3MT isoform and BORCS7 are molecular risk factors in the 10q24.32 schizophrenia locus.
==============

### Authors: 

**Ming Li, Andrew E. Jaffe, Richard E. Straub, Ran Tao, Joo Heon Shin, Yanhong Wang, Qiang Chen, Chao Li, Yankai Jia, Kazutaka Ohi, Brady J. Maher, Nicholas J. Brandon, Alan Cross, Joshua G. Chenoweth, Daniel J. Hoeppner, Huijun Wei, Thomas M. Hyde, Ronald McKay, Joel E. Kleinman, Daniel R. Weinberger**

### Abstract

Genome-wide association studies (GWAS) have reported many SNPs associated with psychiatric disorders, but knowledge is lacking regarding molecular mechanisms. Here, we show that risk alleles spanning multiple genes across the 10q24.32 schizophrenia locus are associated in human brain selectively with increased expression of both *BORCS7* and a previously uncharacterized human-specific *AS3MT* isoform (*AS3MT<sup>d2d3</sup>*) that lacks arsenic methyltransferase activity and is more abundant in individuals with schizophrenia than in controls. Conditional expression analysis suggests that the *BORCS7* and *AS3MT<sup>d2d3</sup>* signals are largely independent. GWAS risk SNPs across this region are linked with a variable number tandem repeat (VNTR) polymorphism in the first exon of *AS3MT* which is associated with expression of *AS3MT<sup>d2d3</sup>* in both Caucasian and African American samples. The VNTR genotype predicts activity in luciferase assays and DNA methylation within the *AS3MT* gene. Both AS3MT<sup>d2d3</sup> and *BORCS7* are expressed in adult human neurons and astrocytes and are upregulated during human stem cell differentiation toward neuronal fates. Our results provide a molecular explanation for the prominent 10q24.32 locus association, including a novel and evolutionarily recent protein involved in early brain development and risk for psychiatric illness.

### Links

**Nature Medicine**

**PubMed**


Data Availability
------------

### Processed Data

The easiest way to access the underlying data from this paper is to use [this R object](http://LieberInstitute.github.io/as3mt-paper/rdas/rawAndRpkmCounts_plusGenotype_10q24_DLPFC_n738.rda) which contains:

1. Phenotype data: `pd`,  rows are subjects and columns are covariates and identifiers. Identifiers for the expression data are RNA Numbers (`Rxxxx`) and identifiers for the genotype data are Brain Numbers (`Brxxx`). Corresponding text file: [pd](http://LieberInstitute.github.io/as3mt-paper/data/phenotype_n738_LIBD.csv)
2. Gene-level data: `geneRpkm` and `geneCounts` correspond to gene RPKM and count values respectively and have genes/features down the rows and subjects/samples across the columns (in the same order as the rows of the phenotype data). `geneMap` is the corresponding annotation information. Corresponding text files: [geneRpkm](http://LieberInstitute.github.io/as3mt-paper/data/geneRpkm_n738_LIBD.csv), [geneMap](http://LieberInstitute.github.io/as3mt-paper/data/geneAnnotation_Ensembl75.csv)
3. Exon-level data: `exonRpkm` and `exonCounts` correspond to exon RPKM and count values respectively and have exons/features down the rows and subjects/samples across the columns (in the same order as the rows of the phenotype data). `exonMap` is the corresponding annotation information. Corresponding text files: [exonRpkm](http://LieberInstitute.github.io/as3mt-paper/data/exonRpkm_n738_LIBD.csv), [exonMap](http://LieberInstitute.github.io/as3mt-paper/data/exonAnnotation_Ensembl75.csv)
4. Junction-level data: `jRpkm` and `jCounts` correspond to junction RPMs and count values respectively and have exons/features down the rows and subjects/samples across the columns (in the same order as the rows of the phenotype data). `jMap` is the corresponding annotation information, which is a `GRanges` object. Corresponding text files: [jRpm](http://LieberInstitute.github.io/as3mt-paper/data/junctionRpm_n738_LIBD.csv), [jMap](http://LieberInstitute.github.io/as3mt-paper/data/junctionAnnotation_LIBD.csv)
5. Genotype data: `snpMat` contains the number of copies of the minor allele, and have variants down the rows and subjects/samples across the columns (in the same order as the rows of the phenotype data). `snpInfo` contains the corresponding annotation and GWAS statistics information. Corresponding text files: [snpMap](http://LieberInstitute.github.io/as3mt-paper/data/snpMinorCounts_LIBD.csv), [snpInfo](http://LieberInstitute.github.io/as3mt-paper/data/snp_annotation.csv)

### Alignment and Raw Data

The phenotype object has public file paths for the 2 megabase region BAM files in the 10q24.32 genomic locus, and raw gene and exon counts files, which are all hosted on AWS S3 storage.


#### Support or Contact

Having trouble accessing the data? Contact [Andrew E Jaffe](mailto:andrew.jaffe@libd.org) or [Ming Li](mailto:ming.li@libd.org) and we’ll help you sort it out. For questions about the paper, please email the corresponding author, [Daniel Weinberger](mailto:drweinberger@libd.org) 

------------------
<a href="http://libd.org">
<img src="images/LIBD_logo.jpg" alt="Drawing" style="width: 250px;"/>
