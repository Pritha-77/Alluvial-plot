
Gene–miRNA 
This repository contains an R workflow to visualize gene–miRNA interactions and gene–trait associations using alluvial (Sankey-style) plots.
________________________________________
⚙️ Requirements
•	R version ≥ 4.0
•	R packages:
o	readxl
o	stringr
o	writexl
o	ggplot2
o	ggalluvial
o	dplyr
Install missing packages with:
install.packages(c("readxl", "stringr", "writexl", "ggplot2", "ggalluvial", "dplyr"))
________________________________________
📥 Input Format
The input Excel file (list4.xlsx) should have at least these columns:
•	gene → Gene name (e.g., TP53, BRCA1)
•	miRNA → Associated miRNA(s)
Example:
gene	miRNA
TP53	miR-21
BRCA1	miR-34a
BRCA2	miR-200c
________________________________________
▶️ Usage
1.	Set working directory to your project folder:
2.	setwd("d:/NGS_Data_Analysis")
3.	Run the script:
4.	source("alluvial_plot.R")
5.	Outputs:
o	alluvial_gene_miRNA.pdf → Alluvial plot of genes vs top 50 miRNAs
o	alluvial_gene_trait.png → Alluvial plot of genes vs traits
________________________________________
📊 Output Examples
Gene–miRNA Alluvial Plot
•	Shows how the top 50 most frequent miRNAs map to their target genes.
________________________________________
🔍 Features
•	Filters miRNAs to the top 50 most frequent for readability.
•	Generates high-resolution PDF/PNG plots with adjustable size.
•	Color-coded by gene for better visualization.
•	Easily extensible to larger datasets or other categorical mappings.

