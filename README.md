# GP2 Bioinformatics Training Workshop, Argentina 2026
`GP2 ❤️ Open Science 😍`

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24085760.svg)](https://doi.org/10.5281/zenodo.24085760)

**Last updated:** September 2026

## Summary

This is the online repository for (1) ancestry-specific burden testing using SKAT-O analysis for single gene **LRRK2** and the combined **LRRK2–RAB32–VPS35** gene set as pathway-specific analysis, (2) copy number variant calling, (3) short tandem repeat analysis, (4) runs of homozygosity.

## Data statement
Data used in the preparation of this article were obtained from the Global Parkinson’s Genetics Program (GP2; https://gp2.org).

All GP2 data are hosted in collaboration with the Accelerating Medicines Partnership in Parkinson’s disease, and are available via application on the website (https://amp-pd.org/register-for-amp-pd). For up-to-date information on GP2 data acquisition, access, and policies, visit https://gp2.org/. Tier 1 data can be accessed by completing a form on the Accelerating Medicines Partnership in Parkinson’s Disease (AMP®-PD) website (https://amp-pd.org/register-for-amp-pd). Tier 2 data access requires approval and a Data Use Agreement signed by your institution.
In this analysis we used Tier 2 GP2 Release 12 data ([10.5281/zenodo.20932193](https://doi.org/10.5281/zenodo.20932193))

### Helpful Links

- [GP2 Website](https://gp2.org/)
  - [GP2 Cohort Dashboard](https://gp2.org/cohort-dashboard-advanced/)
- [Introduction to GP2](https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494)
  - [Other GP2 Manuscripts (PubMed)](https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22)

## Repository Orientation
- The `analysis/` directory includes all analyses discussed in the manuscript.

<pre> THIS_REPO/ 
  ├── analyses/ 
  |     ├── 00_Burden.ipynb
  |     ├── 01_CNV_calling.ipynb
  |     ├── 02_ExpansionHunter.ipynb
  |     └── 03_Homozygosity.ipynb
  ├── LICENSE
  └── README.md 
</pre>

## Analysis Notebooks
### Languages: Python, bash, and R
| Directory | Notebooks   | Description | 
|-----------|----------------|--------|
|`analyses/`| `00_Burden.ipynb`                | GP2 Release 12 WGS data for ancestry-specific SKAT-O single gene analysis|
|`analyses/`| `01_CNV_calling.ipynb`           | GP2 Release 12 WGS data for calling copy number variants (CNV)|
|`analyses/`| `02_ExpansionHunter.ipynb`       | GP2 Release 12 WGS data for short-tandem repeat analysis with ExpansionHunter|
|`analyses/`| `03_Homozygosity.ipynb`          | GP2 Release 12 WGS data for runs of homozygosity (ROH)|



## Software
| **Software** | **Version(s)** | **Resource URL** | **RRID** | **Notes** |
|--------------|----------------|------------------|----------|-----------|
|ANNOVAR|d.06.08.2020|http://www.openbioinformatics.org/annovar/|RRID:SCR_012821|Used for variant annotation.|
|BCFtools|v.1.17+|http://samtools.sourceforge.net/mpileup.shtml|RRID:SCR_005227|Used for genomic file manipulation.|
|ExpansionHunter|v.5.0.0|https://github.com/illumina/expansionhunter|NA|Used for STR analysis.|
|Manta|v.1.6.0| https://github.com/Illumina/manta| RRID:SCR_022997| CNV analysis| 
|PLINK|v.1.9,v. 2.0|http://www.nitrc.org/projects/plink|RRID:SCR_001757|Used for genetic analyses.|
|Python Programming Language|3.10|http://www.python.org/|RRID:SCR_008394|pandas ; Used for general data wrangling/plotting/analyses|
|RVTests|v.2.1.0|http://genome.sph.umich.edu/wiki/RvTests|RRID:SCR_007639|Used for burden analyses.|