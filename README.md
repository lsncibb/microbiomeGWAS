# MicrobiomeGWAS
## Introduction
Microbiome is a software package for identifying host genetic variants associated with micorbiome distance matrix or beta-diversity. For each SNP, Microbiome GWAS can test the main effect or the SNP-environment interaction. 

The score statistics have positive skewness and kurtosis, which lead to severely inflated type-I error rates. We solved the problem by correcting the skewness and kurtosis, verified by simulations.    


## Reference
Xing Hua, Lei Song, Guoqin Yu, James J. Goedert, Christian C. Abnet, Maria Teresa Landi and Jianxin Shi. MicrobiomeGWAS: a tool for identifying host genetic variants associated with microbiome composition. 

## Input files
PLINK binary genotype files, a distance matrix and a set of covariates, e.g., PCAs for adjusting population stratefication. 
The current version does not support genotypic dosages. 

## Memory require and computation speed
MicrobiomeGWAS processes one SNP at a time and does not load all genotype data into memory; thus, it requires only memory for storing the distance matrix. The computation time is summarized in the figure. 

## Figure
[![Display Figure](https://github.com/lsncibb/microbiomeGWAS/figure.png)](https://github.com/lsncibb/microbiomeGWAS/id123456)


## Example

## Contact
* Xing Hua, xing.hua@nih.gov
* Lei Song, lei.song@nih.gov
* Jianxin Shi, Jianxin.Shi@nih.gov

