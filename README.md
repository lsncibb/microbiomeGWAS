# MicrobiomeGWAS
## Introduction
Microbiome is a software package for identifying host genetic variants associated with micorbiome distance matrix or beta-diversity. For each SNP, Microbiome GWAS can test the main effect or the SNP-environment interaction. We found that the score statistics have positive skewness and kurtosis, which lead to severely inflated type_I error rates. We addressed the problem by correcting the skewness and kurtosis to derive an approximation. Simulations suggested that the P-value approxcimations are accurate even for P=10E-7.   


## Reference
Xing Hua, Lei Song, Guoqin Yu, James J. Goedert, Christian C. Abnet, Maria Teresa Landi, Jianxin Shi. MicrobiomeGWAS: a tool for identifying host genetic variants associated with microbiome composition. 

The current version requires three sets of files: PLINK binary genotype files, a distance matrix and a set of covariates, e.g., PCAs for adjusting population stratefication. The current version does not support genotypic dosages. 

Microbiome is very fast, 


## Example
## Figure
[![Display Figure](https://github.com/lsncibb/microbiomeGWAS/figure.png)](https://github.com/lsncibb/microbiomeGWAS/id123456)
## Contact
* Xing Hua, xing.hua@nih.gov
* Lei Song, lei.song@nih.gov
* Jianxin Shi, Jianxin.Shi@nih.gov

