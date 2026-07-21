# methylobacterium_metapangenomics

R scripts for "Metapangenomics reveals host-driven adaptation of Methylobacterium to the phyllosphere"
Scripts author: Jocelyn Lauzon, Département des sciences biologiques, Université du Québec à Montréal

These Bash and R markdown scripts cover all metapangenomic and statistical analyses, as well as figures related to the article.

Scripts should be run in the order listed below.

## Bash script description

anvio.txt
This script contains all commands related to the analyses performed with anvio v.8

## R markdown scripts descriptions

mapped_reads.Rmd
Relation between host species and paired-end reads and mapped reads.

genomes_horizontal_cov_hist.Rmd
Distribution histograms of horizontal coverage values.

bacteria_genus_analyses.Rmd
Analyses on total bacterial communities at the genus level.

methylo_species_analyses.Rmd
Analyses of Methylobacterium species' community diversity, composition and phylogenetic relatedness.

gene_data_preparation.Rmd
Preparation of data for gene composition and diversity analyses based on anvio analyses outputs.
Merging metapangenome table with horizontal coverage ('detection') and coverage depth statistics.
Creation of 3 dataframes to work from.
'data.pangenome.rds' -> for pangenome analyses
'data.fct.det.rds' -> for gene horizontal coverage ('detection') analyses
'data.fct.cov.rds' -> for gene coverage depth (diversity and differential abundances analyses)
Also contains descriptive statistics on the number of individual genes and functional annotations from the three databases

pangenome_char.Rmd
Descriptive statistics on the number of core, accessory and single genes, as well as hypothetical proteins.
Analyses of genome openness.

genes_diversity.Rmd
Alpha and beta diversity analyses on gene clusters.

DAGCs_analyses.Rmd
Differentially abundant gene clusters analyses with DESeq2.
Creation of DAGCs tables and figures.

combine_var_prof.Rmd
Preparation for the pN/pS analyses.
For each of the 4 Methylobacterium species, combine variability profiles generated in anvio, 
and export files for subsequent analyses in anvio.

pN_pS.Rmd
Analyses of pN/pS ratio and positively selected genes by host species.