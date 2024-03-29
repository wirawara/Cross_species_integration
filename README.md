


Data integration method based on RNA-seq: Cross-species gene expression aging integration
--------------------------------------------------------------------------

This framework represents a data integration method that integrates sequencing datasets based on ranking statistics, and detects functional gene modules within groups of interest, based on RNA-sequencing files.


* Preprint out [here](https://www.biorxiv.org/content/10.1101/287128v2)
* Published version [here](https://journals.plos.org/ploscompbiol/article/comments?id=10.1371/journal.pcbi.1007162)
* The code is available in the Supplementary Materials (https://www.biorxiv.org/content/biorxiv/suppl/2018/03/23/287128.DC1/287128-2.pdf)


![Screen Shot 2022-01-30 at 19 45 45](https://user-images.githubusercontent.com/14986121/151725187-c1113926-db58-4de8-8fea-c1bec78c0c4f.png)

To run the code
----------------------------
In the beginning of each .Rmd there is a set of R packages to be installed. 
* Check also the sessionInfo() for R packages.
* `kallisto 0.42.4`

Please refer to the Supplementary Materials for more details on running the pipeline.
The Supplementary Materials were prepared in an R markdown file for reproducibility.


Download required files
----------------------------


***Summary of gene expression datasets***


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

To process HOG groups from OMA database.

HOGs are inferred on public genomes and can be downloaded from the OMA orthology database <http://omabrowser.org/oma/home/> .


For running the code: 
	
1.  ```01_retrieval_OMA_groups.py``` - outputs: bilat_families.dic
2.  ```02_oma_unpickle.py```
3.  ```03_OMA_to_R.R```


The HOGs groups are saved in `oma_eogs.rds` and ready to be used in R.	



Pipeline
=========

Download data:




### Expression data correction and normalization



### Differential expression


* Figure 1C	



### Single gene level vs Gene set level


* Figure 2




### GSEA per species


* Figure 3



### Shared processes and DR

* Figure 3



### Functional modules

* Figure 4



### Modular architecture and candidate genes in GWAS

* Figure 5




Supplement Figures
______________________


