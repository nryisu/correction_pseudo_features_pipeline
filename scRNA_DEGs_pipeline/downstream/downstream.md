# Dependencies
Below R package needs to be installed (The R version is 3.6.1):
- SingleCellExperiment
- scater
- TxDb.Mmusculus.UCSC.mm10.ensGene
- scran
- Rtsne
- edgeR
- ggplot2
- RColorBrewer
- NMF
- data.table

# Filter low quality cells, low expression genes and classify the cell cycle phase
`#`This script will output the mesc_npc.txt_cycle.rds file, we rename it to mesc_npc_cycle.rds for DEGs anaylsis.
Rscripts 0_qc.R mesc_npc.txt

# Identify the DEGs and enrichment analysis
Rscripts 1_deg.R mesc_npc_cycle.rds
