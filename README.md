# SNVs_DNMs_IRASFS
# General Info
[![DOI](https://zenodo.org/badge/749389873.svg)](https://doi.org/10.5281/zenodo.13864621)
This pipeline was genrated to calculated the Denovo SNVs germline mutation from WGS NGS data in IRASFS multi-siblings pedigree samples (mother, father and offspring). 
The raw sequences is private due to the human clinical sample restiriction.

## Overview

The workflow is structured around the development of bash, R, and Python scripts. Utilizing alternative datasets would necessitate modifications to the existing scripts.

The code presented herein is designed to explore the validation of de novo Single Nucleotide Variants (SNVs) data obtained from the IRASF cohort, exclusive to multi-child families. Subsequent analyses include the examination of mutation spectrum and signature analysis.

The initial step involved identifying the list of candidate De Novo Mutations (DNMs) from the IRASFS Whole-Genome Sequencing (WGS) dataset, carried out in bash using tools such as DeNovoGear (DNG) and GATK. The subsequent sections encompass post-processing steps aimed at validating the identified candidates, followed by further analyses.


The steps are:
1. Conduct pre-processing of validation data to ensure its compatibility before importing into the R environment.
2. Retrieve and import the list of sites to be validated from each callset.
3. Execute the processing of validation sites..
4. Apply filtering procedures to refine the results.
   

## Requirements 

Default software used to run the pipeline are:
- BWA 0.7.17
- Samtools 1.8.0
- Bcftools 1.8
- GATK 4.0.11.0
- DeNovoGear 1.1.1-308-g3ae70ba
- R 4.0.2 
- Python 3.9.2  
- Sigprofilerextractor  1.1.14  
- SigProfilerExtractor  1.0.18 


For some script the following version were used (specified in the step/README.txt):
- Samtools 1.12.0
- SigProfilerExtractor 1.1.14
  
