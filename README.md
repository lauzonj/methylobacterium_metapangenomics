# methylobacterium_metapangenomics

R scripts for "Metapangenomics reveals host-driven adaptation of Methylobacterium to the phyllosphere"
Script author: Jocelyn Lauzon, Département des sciences biologiques, Université du Québec à Montréal

These R markdown scripts cover all statistical analyses and figures related to the article.

Scripts should be run in the order listed below.

## Bash script

anvio_script.txt
This script contains all commands related to the analyses performed with anvio v.8




How did I do the nb_reads.txt table?

In general, What are the output files of anvio I used in R scripts?
--> must include in 'data' folder anvio's output files that are inputed directly in R scripts.




## R markdown scripts descriptions

mapped_reads.Rmd
Tests for:
paired-end reads ~ host species (Figure S4)
% mapped reads ~ host species (Figure S5)

genomes_horizontal_cov_hist.Rmd
Distribution histograms of horizontal coverage values (Figure S1A-B).

bracken_analyses.Rmd
Analyses on total bacterial communities (genus level).

methylo_species_analyses.Rmd
Analyses of Methylobacterium species' community diversity, composition and phylogenetic relatedness.




gene_data_preparation.Rmd
Preparation of data for gene composition and diversity analyses.
Merging metapangenome table with detection and coverage stats.
Creation of 3 dataframes to work from.
'data.pangenome.rds' -> for pangenome analyses
'data.fct.det.rds' -> for gene coverage and detection statistics analyses
'data.fct.cov.rds' -> for gene coverage analyses (diversity and differential abundances analyses)





pangenome_char.Rmd
Calculate number of core and accessory genes, and number of hypothetical proteins.






genes_cov_and_detect.Rmd
Analyses of genes mean coverage and detection distributions.

plant_traits_v2.Rmd
Prepare traits data to import to 'genes_diversity_v5-2' script.

genes_diversity_v5-3.Rmd
Diversity analyses of gene clusters.
DAGCs analyses (use 'TAKE 2' section of DAG). !! DO NOT use code for the creation of the DAGCs table nor for the COG categories figures. This code
was used for my M.Sc. thesis, but for the article, use 'DAGCs_analyses_folloup.Rmd'

DAGCs_analyses_followup.Rmd
Followup of the DAGCs analyses, of the 757 annotated DAGCs. Table : To include all COG categories and pathways, as well as all KEGG brite, 
classes, modules, etc. No missing info on DAGCs functions. Figures : creation of the article figure for COG categories and KEGG categories 
(manually curated based on the BRITE functional hierarchy).

DAGCs_figure.Rmd
Creation of figures showing enriched genes for specific functional categories.

selection_v2_251214.Rmd
Analyses of pN/pS ratio and positively selected genes by host species.