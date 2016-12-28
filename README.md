![CRISPRAnalyzeR](https://github.com/boutroslab/crispr-analyzer/blob/master/images/CRISPRAnalyzR_logo5.png)
# CRISPRAnalyzeR - Fully-interactive Analysis and Documentation of Pooled CRISPR Screens
Welcome to the CRISPRAnalyzeR Github page!

CRISPRAnalyeR is a web-based, fully interactive suite for the analysis and documentation of pooled CRISPR Screens.

#### See the live-demo of [CRISPRAnalyzeR](http://crispr-analyzer.dkfz.de)

CRISPRAnalyzeR has been specifically developed to provide a fully-interactive, hollistic and exploratory analysis of pooled CRISPR Screens especially for those people that perform the screens themselves.
You can easily analyse your screen using 6 different hit calling and 1 essential gene calling methods as well as perform gene annotation enrichment, gene set analysis and get detailed information about your sgRNAs - all in a convenient web-browser interface.

**All you need is your sequencing data and the pooled CRISPR screen library file (we provide you with the most common ones) - and CRISPRAnalyzeR will help you to go from rawdata to potential followup candidates!**


## What makes CRISPRAnalyzeR the perfect tool to analyze pooled CRISPR Screens?

CRISPRAnalyzeR uses a **guided-analysis** approach. This means you will be **guided through the whole analysis, so that you can focus on the most important thing - your data**.

In brief, CRISPAnalyzeR consists of **four sections**, all paired with a great user-friendly UI:
- Screen Quality Estimation
- Hit Calling using multiple published hit calling methods
- Hit Confirmation with extensive Gene information, sgRNA information, Gene Set Analysis and much more
- Download of the interactive report that provides a comprehensive documentation of your screen

<img src="https://github.com/boutroslab/crispr-analyzer/blob/master/images/CRISPRAnalyzeR_5columns.png" alt="alt text" width="50%" style="align:center;" >

### The principle CRISPRAnalyzeR Guided-Analysis Workflow
<img src="https://github.com/boutroslab/crispr-analyzer/blob/master/images/CA_workflow.png" alt="alt text" width="50%" style="align:center;" >


**Analysing CRISPR Screens has never been easier - and has never been so much fun!**

### What does CRISPRAnalyzeR offer?

CRISPRAnalyzeR is easy-to-use and assists you with the analysis of your screening data.
It contains **4 different steps**, each filled with nice visualizations, interactive tables and all the information you need.

#### Quality Control
<img src="https://github.com/boutroslab/crispr-analyzer/blob/master/images/CA_QC.png" alt="alt text" width="50%" style="align:center;" >

#### Hit Calling
<img src="https://github.com/boutroslab/crispr-analyzer/blob/master/images/CA_HC.png" alt="alt text" width="50%" style="align:center;" >

#### Hit Confirmation and Gene Annotation
<img src="https://github.com/boutroslab/crispr-analyzer/blob/master/images/CA_HConfirmation.png" alt="alt text" width="50%" style="align:center;" >

#### Interactive OFFLINE Report Containing all the Data
<img src="https://github.com/boutroslab/crispr-analyzer/blob/master/images/CA_Report.png" alt="alt text" width="50%" style="align:center;" >


## How to download the CRISPRAnalyzeR

#### Please check our [live demo](http://crispr-analyzer.dkfz.de), which you can also use to analyse your screening data.

You can get the CRISPRAnalyzeR suite as source code or as a ready-to-use Docker Container.

#### Minimum System Requirements
CRISPRAnalyzeR is based on R Shiny-Server and uses many different R packages and tools.
For a source code installation, we recommend the use of Ubuntu.

 | Source Code Installation | Docker Container Installation
----|---|----
Operating System|Ubuntu|Any supported OS by Docker
CPU|Dual Core (Quad Core recommended)| Dual Core (Quad Core recommended)
RAM|8 GB| 8GB
HDD|512 GB (SSD recommended)| 512 GB (SSD recommended)
Additional Software Packages | **See list below!** | All included in container


#### Licenses
CRISPRAnalyzeR is published under the GPL-2 license and is **free for non-commercial use only**.
While CRISPRAnalyzeR does not require an additional license for commercial use itself, some included tools strictly require additional licensing.
**Please note that Highcharts, the COSMIC database and the Enrichr API access require additional licensing for commercial use**.


### Source Code


### Ready-to-use Docker Container

## What CRISPRANalyzeR offers you

## How to Install CRISPRAnalyzeR using the provided Source Code

## How to Install CRISPRAnalyzeR using the provided Docker Container

## How to Install CRISPRAnalyzeR using the provided Docker File

## How to Start and Restart the CRISPRAnalyzeR

## How to use the COSMIC Database and Enrichr API
### COSMIC (Catalogue Of Somatic Mutations In Cancer)

The COSMIC database can be found [here](https://cancer.sanger.ac.uk/cosmic).
By default, we do not provide the COSMIC database due to licensing compatibility.
In case you want to use the COSMIC database, please proceed as follows.

- Visit the [COSMIC Database Website](https://cancer.sanger.ac.uk/cosmic)
- If you aim for a commercial use, please see the [COSMIC Licensing Information Page](https://cancer.sanger.ac.uk/cosmic/license)
- Head to the [COSMIC download section](https://cancer.sanger.ac.uk/cosmic/download)
- Download the __COSMIC Mutation Data__ database file
- Extract the CosmicMutantExport.tsv.gz file to the __database__ folder within the CRISPR AnalyzeR
- Open the __config.R__ in the main folder of the CRISPRAnalyzeR Shiny directory and edit it 
```r
# COSMIC database file, needs to be located in database_path
# DEFAULT is NULL, as CRISPRAnalyzeR is not provided with COSMIC Database
config[["COSMIC_database"]] <- "CosmicMutantExport.tsv" # NULL if not available
```
- Restart the CRISPRAnalyzeR

*Please note that the COSMIC database is loaded during the analysis procedure and requires 1 GB of RAM.*

### Enrichr API
By default, CRISPRAnalyzeR has the Enrichr API access disabled.
You can activate the Enrichr API access during the installation by setting XXXXX.

Please not that you require a license for commercial use.

## How to perform an Analysis using CRISPRAnalyzeR
*YOUTUBE VID HERE*

## Sample Data

## Pre-made sgRNA library FASTA files

## Common settings for published CRISPR libraries
