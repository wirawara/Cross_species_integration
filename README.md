


Cross species aging paper
---------------------------------------
Repository to reproduce analyses from the Cross species aging Manuscript

*Komljenovic A & Robinson-Rechavi M. Cross-species functional modules identify conserved splicing and immune genes of aging.* 



To run the code
----------------------------
In the beginning of each .Rmd there is a set of R packages to be installed. 
* Check also the sessionInfo() for R packages.
* `kallisto 0.42.4`

Download required files
----------------------------


***Summary of gene expression datasets***


To download all these datasets, please go to `s0.preprocessing.steps.Rmd` and `s0.GTEx.preprocess.Rmd`.



Download from <http://www.gtexportal.org/home/datasets>:

* `GTEx_Analysis_v6p_RNA-seq_RNA-SeQCv1.1.8_gene_reads.gct.gz`
* `GTEx_Data_V6_Annotations_SampleAttributesDS.txt`
* `GTEx_Analysis_2015-01-12_Annotations_SubjectPhenotypesDS.txt`


Download from <https://www.ncbi.nlm.nih.gov/geo/>:

1. Human:
	
	B. Dietary restriction 
	* GSE38012 (skeletal muscle) - microarray

2. Mouse:
 
	A. Aging	
	* GSE6323 (skeletal muscle) - microarray
  	* GSE61915 (hippocampus) - RNAseq 
 	

	B. Dietary restriction
	* GSE6323 (skeletal muscle) - microarray

3. Fly:
 	
	A. Aging  
	* GSE42255 (wholebody) - microarray
 	
	B. Dietary restriction
	* GSE26726 (wholebody) - microarray


4. Worm:
 	
	A. Aging
  	* GSE46051 (wholebody) - RNASeq
 	
	B. Dietary restriction
	* GSE27677 (wholebody) - microarray




***Summary of download the OMA groups***

To process HOG groups from OMA database, refer to `s0.OMA.steps.Rmd`.

HOGs are inferred on public genomes and can be downloaded from the OMA orthology database <http://omabrowser.org/oma/home/> .


For running the code: 
	
1.  ```01_retrieval_OMA_groups.py``` - outputs: bilat_families.dic
2.  ```02_oma_unpickle.py```
3.  ```03_OMA_to_R.R```


The HOGs groups are saved in `oma_eogs.rds` and ready to be used in R.	










Pipeline
=========

Download data:

1. `s0.preprocessing.steps.Rmd`

2. `s0.GTEx.preprocess.Rmd`
	
3. `s0.OMA.steps.Rmd`



### Expression data correction and normalization



### Differential expression


* Figure 1C	

1. `s1.DiffExp.Rmd` 



### Single gene level vs Gene set level


* Figure 2

1. `s2.SingleGeneLevel_GeneSetLevel.Rmd` 



### GSEA per species


* Figure 3

1. `s3.GSEAperspecies.Rmd`




### Shared processes and DR


* Figure 4

1. `s4.SharedProcesses_DietaryRestriction.Rmd`


### Functional modules

* Figure 5

1. `s5.Modularity.Rmd`

### Modular architecture and candidate genes in GWAS

* Figure 6






Supplement Figures
______________________




Final .Rmd for main figures 
------------------------
This goes to reviewers.

