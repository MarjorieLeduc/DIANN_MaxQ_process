# DIANN_MaxQ_process
Make descriptive and statistical analysis using DIA-NN or Maxquant output and generate word and excel reports with PCA, heatmaps, volcanoplots...

# Content
DIANN_MaxQ_process.rmd analyses data from Maxquant or DIA-NN softwares and generates 4 files :
- a Word file containing report with many plots including PCA, heatmaps, volcanoplot ...
- a Excel file containing protein quantifications, student tests results and number of peptides per proteins.
- a txt file containing the same data as the Excel file
- a .rds file that can be use with shiny_PROTEOMIC.R script to custom plots.

## Requirements
R4.4.0 or higher
RStudio 2024.04.1 Build 748 or higher

## Required data
To use DIANN_MaxQ_process.rmd,

For DIA-NN analysis, folder must contain :
    - report.pg_matrix.tsv.txt,
    - report.log.txt,
    - report.pr_matrix.tsv,
    - report.tsv
	(the Script is done for .d DIA files from Bruker)
	(.d names files must not contain spaces, or "-" or ".")
	(In the spectral library, the contaminant proteins' accessions should be preceded by "Conta_" to be detected as Contaminant)
	(export from DIANN must be called "report.tsv")
	
For Maxquant analysis, folder must contain :
    - proteinGroups.txt,
    - mqpar.xml,
    - evidence.txt,
    - #runningTimes.txt (found in "combined/proc/" folder)



## Use
In RStudio, open the DIANN_MaxQ_process_2.4.rmd file, click on Knit and follow tutorial. Think to check, only for the first time, if you have all packages.
