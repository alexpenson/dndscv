dndscv
=====

Description
---
The **dNdScv** R package is a suite of maximum-likelihood dN/dS methods designed to 
	quantify selection in cancer and somatic evolution (Martincorena *et al.*, 2017). The 
	package contains functions to quantify dN/dS ratios for missense, nonsense and 
	essential splice mutations, at the level of individual genes, groups of genes or at 
	whole-genome level. The *dNdScv* method was designed to detect cancer driver genes 
	(*i.e.* genes under positive selection in cancer) on datasets ranging from a few 
	samples to thousands of samples, in whole-exome/genome or targeted sequencing studies. 
	
The background mutation rate of each gene is estimated by combining local information 
	(synonymous mutations in the gene) and global information (variation of the mutation 
	rate across genes, exploiting epigenomic covariates), and controlling for the sequence 
	composition of the gene and mutational signatures. Unlike traditional implementations 
	of dN/dS, *dNdScv* uses trinucleotide context-dependent substitution matrices to 
	avoid common mutation biases affecting dN/dS (Greenman *et al.*, 2006).

Note
----
New functionalities will soon be added to this R package, including support for other 
human genome assemblies and other species. 

Installation
--------

You can use devtools::install_github() to install *dndscv* from this repository:

	> library(devtools); install_github("im3sanger/dndscv")
	
Reference
----
Martincorena I, *et al*. (2017) Universal Patterns of Selection in Cancer and Somatic Tissues. *Cell*.


Acknowledgements
--------

Moritz Gerstung and Peter Campbell.