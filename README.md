# Reproduce analyses for Gunn et al. [DATE]
<font size="+1">Follow the steps listed below in the <b><i>Analyses</i></b> section to reproduce analyses for Gunn et al. [DATE]. Each step below gives a summary of the analysis and directs you to a general code file which then works through the analysis step-by-step. This general file will usually point you to other Rmd code, bash shell scripts, or python scripts. Each analysis is contained within subdirectories of the same name in the main R project directory.</font>

<b>Find the article here</b>: <a href="url">...</a> 

<b>Citation here</b>: 

## Project: Assessing transgenerational phenotypic responses to insecticide exposure in Colorado Potato Beetles (<i>Leptinotarsa decemlineata</i>; CPB) 
We assessed inter- and trans-generational effects of sublethal insecticide exposure on four larval performance phenotypes (mobility, herbivory, development, and fecundity) in Colorado potato beetles (<i>Leptinotarsa decemlineata/i>; CPB). We implemented a highly replicated, full-sibling inbreeding pedigree experimental design beginning with 12 "founder" mated pair lineages and continuing for four successive generations (full siblings within lineages were paired for mating in each generation). For the transgenerational experiment, F<sub>0</sub> larvae (offspring of founder pairs) were divided into two treatment groups (exposed, i.e., exposed to a sub-lethal dose of the neonicotinoid insecticide imidacloprid; and control, i.e., exposed to an equivalent dose of molecular-grade water). A subset of beetles were collected from each treatment within each lineage for each generation and monitored for four performance traits, including larval movement (mobility), feeding rate (herbivory), and time to discrete life stages (development). Performance traits were monitored in three successive generations (F<sub>1</sub>-F<sub>3</sub>) without treatment exposure and compared to the F<sub>0</sub> generation to test for inter- and transgenerationally-inherited phenotypic variation. An additional subset of larvae from each generation were re-exposed to treatments, both experimental (insecticide-exposed) and control (water), to test for potential selection of phenotypic variation across generations.

## General information on repository structure
This is a publicly visible GitHub repository storing code (and a small amount of data, although we have done our best to avoid uploading large amounts of data due to the limited storage in GitHub) for Gunn et al. [DATE]. In the home directory of the repository (CPB_Phenotype), you will find a README.md file (the source script for this information), the R Project file (CPB_Phenotype.Rproj), a project info folder (project_info, which includes all important information on data procurement for this project), a .gitignore file, and "analysis" directories, each of which corresponds with a specific analysis conducted in our study:

1) 01_data_summary_analysis
2) 02_ld_analysis
3) 03_fecundity_analysis
4) 04_mobility_analysis
5) 05_herbivory_analysis
6) 06_development_analysis

Within each analysis directory, you will find an R markdown script (.Rmd) with the name of the analysis, which contains all of the code needed to run the full analysis. Additionally, you will find:

1) code

The code directory will store all source code, shell scripts, lists of bash commands, and software packages needed for analysis. 

Once you have downloaded the repository and located the code directory, you should create two additional sub-directories within each analysis (on the same level as the code directory):

2) data
3) figures

The data directory will store all processed data and metadata needed for analysis. The figures folder will contain any raw figures generated in ggplot for each analysis. Ideally, the Rmd script should have paths set up so that the code reads all data and scripts and generates figures seamlessly.

## Using the code
To reproduce all analyses in Gunn et al. [DATE], download this data repository and place in a desired home directory. This may be done on your local machine, but we recommend downloading to a high-performance computing cluster so that all code will run seamlessly in one environment, as long as Rstudio is installed and the GUI can be called on the cluster.

Once all directories are downloaded, create a new sub-directory within the home directory (same level as the five analysis directories, .Rproj, README.md, etc.) called "raw_data". This is where you will store the raw genetic data and associated sample metadata (see <i><b>Data</i></b> section below).

## Data

Raw genotype data, accompanying metadata, and data descriptions are available on Dryad: https://doi.org/10.5061/dryad.xksn02vr6. Data descriptions are also provided in the Rmarkdown files associated with each analysis in this Rproject. Detailed instructions are given for 

Download these data into to your `/raw_data` directory within the home working directory.

You should have 4 new items in the directory: <br>

1.   <br>
2.   <br>
3.   <br>
4.   <br>

If you have any questions or issues with data and/or code, please don't hesitate to contact me: jcgunn@uvm.edu

## Analyses

### Analysis 1: Data summarization and preparation
In this analysis, 

#### Run the code: `01_data_summary_analysis/cpb_phenotype_data_summary_analysis.Rmd`

### Analysis 2: Lethal concentration dose determination
In this analysis, 

#### Run the code: `02_ld_analysis/cpb_phenotype_ld_analysis.Rmd`

### Analysis 3: Fecundity analysis
In this analysis, 

#### Run the code: `03_fecundity_analysis/cpb_phenotype_fecundity_analysis.Rmd`

### Analysis 4: Mobility analysis
In this analysis, 

#### Run the code: `04_mobility_analysis/cpb_phenotype_mobility_analysis.Rmd`

### Analysis 5: Herbivory analysis
In this analysis, 

#### Run the code: `05_herbivory_analysis/cpb_phenotype_herbivory_analysis.Rmd`

### Analysis 6: Development analysis
In this analysis, 

#### Run the code: `05_development_analysis/cpb_phenotype_development_analysis.Rmd`
