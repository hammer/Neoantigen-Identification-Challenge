# Challenge Design

We'll be collecting blood, somatic tissue, and tumor-infiltrating lymphocytes (TILs) from patients with a few different types of solid tumors. Whole-exome sequencing (WES) will be performed on the blood and somatic tissue and RNA-Seq will be performed on the somatic tissue.

## Input data
* Germline WES DNA (FASTQ)
* Somatic WES DNA (FASTQ)
* Somatic RNA (FASTQ)

## Data to submit
* VCF with predicted somatic mutations
* CSV with predicted HLA class I types
* CSVs with the ranked list of predicted neoepitopes
 * 1 CSV for each stage of the neoepitope prediction pipeline, with a descriptive label for the action performed by each stage (e.g. "expression filter", "trunk mutation")

## Scoring
A consolidated list of predicted neoepitopes will be built from all challenge submissions and a subset of those peptides will be synthesized and screened against the TILs from the patients using a proprietary assay. The final scoring algorithm has not been determined but will likely be related to the Normalized Discounted Cumulative Gain (NDCG) or F1 score. The results of the assay will be provided to all challenge participants.

Note that the primary goal of this challenge is to learn what pipeline stages are most informative for neoepitope identification, however, so in addition to scoring the final neoepitope lists we'll also be looking to see at which stage correct neoepitopes were filtered out.