# Challenge Design

As documented elsewhere, we'll be collecting blood, somatic tissue, and tumor-infiltrating lymphocytes (TILs) from patients with a few different types of solid tumors. Whole-exome sequencing (WES) will be performed on the blood and somatic tissue and RNA-Seq will be performed on the somatic tissue.

## Input data
* Germline WES DNA (FASTQ)
* Somatic WES DNA (FASTQ)
* Somatic RNA (FASTQ)

## Data to submit
* VCF with predicted somatic mutations
* CSV with predicted HLA class I types
* CSVs with the ranked list of predicted neoepitopes (1 CSV for each stage of the neoepitope prediction pipeline)

## Challenge scoring