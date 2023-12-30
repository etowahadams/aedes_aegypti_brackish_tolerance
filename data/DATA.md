# Data descriptions
This contains the descriptions of the files and folders that are contained in this directory. 

## Original dataset
- `sri-lanka-all-plink/` contains all of the PLINK files associated with the Original Sri Lanka dataset.
- `sri-lanka-all-vcf` - The VCF file (and associated log files) that were created from `sri-lanka-all-plink/SriLanka_only`
- `sri_lanka_metadata.txt` contains the metadata associated with all mosquito samples

## Relatedness 
These files were generated to detect the relatedness between individuals. 
- `SriLanka_only_relate_Res.relatedness2` The relatedness calculated from every pair of individuals in the original dataset
This file was created using the command `vcftools --vcf data/sri-lanka-all-vcf/SriLanka_only_relate.vcf --relatedness2 --out SriLanka_only_relate_Res` 

## Filtered, no sibling dataset
- `no_siblings.txt` These are the IDs of the individuals used to filter `sri-lanka-all-plink/SriLanka_only` to make `sri-lanka-no-sib-plink/SriLanka_no_sib`
- `sri-lanka-no-sib-plink` - These are all of the PLINK files associated the dataset after siblings were removed from `sri-lanka-all-plink/SriLanka_only`. 
- `pca/` - These are the files associated with conducting the PCA analysis on the genotypes of the filtered, no sibling dataset 

