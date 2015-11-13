# MicrobiomeGWAS

MicrobiomeGWAS is a software package for identifying host genetic variants associated with micorbiome distance matrix or beta-diversity. For each SNP, microbiome GWAS tests the main effect or the SNP-environment interaction. 

The score statistics have positive skewness and kurtosis, which lead to severely inflated type-I error rates. We solved the problem by correcting the skewness and kurtosis, verified by simulations.    




## Input files
PLINK binary genotype files, a distance matrix and a set of covariates, e.g., PCAs for adjusting population stratefication. 
The current version does not support dosage data from imputation programs.

Usage:
Rscript microbiomeGWAS_Root_Path/R/microbiomeGWAS_v1.0.R -r microbiomeGWAS_Root_Path -p Your_Plink_Path/Plink_Pre -d Your_Dist_Matrix_Path/Dist_Matrix.txt -o Out_Path -c Your_Covariate_Path/Covariate.txt -i Your_Covariate_Name

## Memory requirement and computation speed
MicrobiomeGWAS processes one SNP at a time and does not load all genotype data into memory; thus, it requires only memory for storing the distance matrix. The computation time is summarized in the figure for analyzing a GWAS with 500,000 SNPs. "Main": main effect test only. "All": main effect test, interaction test and joint effect test. 


[![Display Figure](https://cloud.githubusercontent.com/assets/15255156/11046333/d8560a36-86fa-11e5-8105-6f644ee5c6d7.png)](https://github.com/lsncibb/microbiomeGWAS/)

## Future extensions
We are extending microbiomeGWAS for testing additive and dominant effects. We are also extending the algorithm to test multiple microbiome beta diversity matrices, e.g., generalized UniFrac, to achieve the optimal statistical power. 

## Reference
Xing Hua, Lei Song, Guoqin Yu, James J. Goedert, Christian C. Abnet, Maria Teresa Landi and Jianxin Shi. MicrobiomeGWAS: a tool for identifying host genetic variants associated with microbiome composition. 

## Contact
* Xing Hua, xing.hua@nih.gov
* Lei Song, lei.song@nih.gov
* Jianxin Shi, Jianxin.Shi@nih.gov

