# Reproducibility files
[![DOI](https://zenodo.org/badge/754193560.svg)](https://zenodo.org/doi/10.5281/zenodo.10631233)

## Uccheddu, Damiano, and Ester Lucia Rizzi. ‘Intergenerational Ties and COVID-19 Contagion: A Study on European Adults Aged 50 Years and Older Using SHARE Data’. *The Journals of Gerontology*: Series B 78, no. 4 (2023): 749–63. [DOI: 10.1093/geronb/gbac196](https://doi.org/10.1093/geronb/gbac196).

This README provides a guide for replicating the study "Intergenerational Ties and COVID-19 Contagion" [DOI: 10.1093/geronb/gbac196](https://doi.org/10.1093/geronb/gbac196).


## Instructions

1. **Source Data Acquisition:** Download the source data from the Survey of Health, Ageing and Retirement in Europe (SHARE) website into your working directory: [SHARE Data Portal](https://releases.sharedataportal.eu/login/) at `"A:\Encrypted datasets\Source\SHARE"`.
2. **Do-file Preparation:** Navigate to `"C:\Users\Damiano\Dropbox\_Projects\FRS-FNRS_PER - Paper 1\Data analysis\Reproducibility files\0. Master do-file"` and open the do-file `"[FRS-FNRS_PER] - 01 - First Paper - Master do-file.do"` for editing.
3. **File Path Adjustment:** Modify the file paths (lines 85 to 115 in the master do-file) to align with your computer's directory structure.
4. **Data Analysis Execution:** Run the do-file `"[FRS-FNRS_PER] - 01 - First Paper - Master do-file.do"` in Stata from its location to replicate the data analysis.


## Data availability

This paper uses data from the SHARE Wave 8 COVID-19 Survey 1 (DOI: https://doi.org/10.6103/SHARE.w8ca.800) and SHARE Wave 9 COVID-19 Survey 2 (DOI: https://doi.org/10.6103/SHARE.w9ca.800). In addition, this paper uses data from the regular SHARE Waves 1, 2, 4, 5, 6, 7, and 8 (DOIs: https://doi.org/10.6103/SHARE.w1.800, https://doi.org/10.6103/SHARE.w2.800, https://doi.org/10.6103/SHARE.w4.800, https://doi.org/10.6103/SHARE.w5.800, https://doi.org/10.6103/SHARE.w6.800, https://doi.org/10.6103/SHARE.w7.800, and https://doi.org/10.6103/SHARE.w8.800). Data were retrieved from https://releases.sharedataportal.eu/login/ (on 19 December 2022).

The Survey of Health, Ageing and Retirement in Europe (SHARE) data are distributed by SHARE-ERIC (Survey of Health, Ageing and Retirement in Europe – European Research Infrastructure Consortium) to registered users through the SHARE Research Data Center. The official SHARE Research Data Center website (https://releases.sharedataportal.eu/users/login) is the sole online access point to the SHARE data. Here SHARE users can download the SHARE data after a successful registration. For further details regarding SHARE microdata access, please visit http://www.share-project.org/data-access.html.


## Codebooks and questionnaires

Original questionnaires can be found at https://share-eric.eu/data/data-documentation/questionnaires. Original codebooks can be found at https://www.share-datadocutool.org.


## Notes

- **Do-files:**
  - The master do-file contains Stata code for dataset creation, cleaning, and analysis execution.
  - Separate do-files are dedicated to dataset creation (`"[FRS-FNRS_PER] - 01 - First Paper - Dataset Creation.do"`), data cleaning (`"[FRS-FNRS_PER] - 01 - First Paper - Data Cleaning.do"`), and statistical analysis (`"[FRS-FNRS_PER] - 01 - First Paper - Data Analysis.do"`).

- **Output Storage:**
  - Tables will be stored in `"A:\Encrypted datasets\Derived\FRS_FNRS_PER-Paper_1\Output folder\Tables"`.
  - Figures will be stored in `"A:\Encrypted datasets\Derived\FRS_FNRS_PER-Paper_1\Output folder\Figures"`.

- **Logging:**
  - Log files will be stored in `"A:\Encrypted datasets\Derived\FRS_FNRS_PER-Paper_1\Output folder\Log folder"`.

- **Codebooks:**
  - Codebooks will be stored in `"A:\Encrypted datasets\Derived\FRS_FNRS_PER-Paper_1\Output folder\Codebook"`.


## Directory Structure

### Do-files
		C:.
		|   README.md
		|
		+---0. Master do-file
		|       [FRS-FNRS_PER] - 01 - First Paper - Master do-file.do
		|
		+---1. Dataset Creation
		|       [FRS-FNRS_PER] - 01 - First Paper - Dataset Creation.do
		|
		+---2. Data Cleaning
		|       [FRS-FNRS_PER] - 01 - First Paper - Data Cleaning.do
		|
		\---3. Data Analysis
				[FRS-FNRS_PER] - 01 - First Paper - Data Analysis.do


### Datasets
		A:.
		\---Encrypted datasets
			+---Derived
			|   \---Output folder
			|       +---Codebook
			|       +---Figures
			|       +---Log folder
			|       +---SCS
			|       +---Tables
			|       \---W_All
			\---Source
				\---SHARE
					\---Release 8.8.0
						+---NL_mmExp_sharew6_rel1-0-0_ALL_datasets_stata
						+---NL_mmExp_sharew7_rel1-0-0_ALL_datasets_stata
						+---sharetom5_stata
						|       sharetom5.ado
						|       sharetom5.hlp
						|       sharetom5_readme.txt
						|
						+---sharew1_rel8-0-0_ALL_datasets_stata
						+---sharew2_rel8-0-0_ALL_datasets_stata
						+---sharew3_rel8-0-0_ALL_datasets_stata
						+---sharew4_rel8-0-0_ALL_datasets_stata
						+---sharew5_rel8-0-0_ALL_datasets_stata
						+---sharew6_rel8-0-0_ALL_datasets_stata
						+---sharew7_rel8-0-0_ALL_datasets_stata
						+---sharew8ca_rel8-0-0_ALL_datasets_stata
						+---sharew8_rel8-0-0_ALL_datasets_stata
						+---sharew8_rel8-0-0_gv_accelerometer_epochs_stata
						|   \---dta
						|       +---be_fr
						|       +---be_nl
						|       +---cz
						|       +---de
						|       +---dk
						|       +---es
						|       +---fr
						|       +---it
						|       +---pl
						|       +---se
						|       \---si
						+---sharew9ca_rel8-0-0_ALL_datasets_stata
						+---sharewX_rel8-0-0_easySHARE_stata
						+---sharewX_rel8-0-0_gv_allwaves_cv_r_stata
						+---sharewX_rel8-0-0_gv_job_episodes_panel_stata
						+---sharewX_rel8-0-0_gv_linkage_stata
						+---sharewX_rel8-0-0_gv_longitudinal_weights_stata
						\---SHARE_computing_calibrated_weights_stata
							\---Analysis
								+---ado
								\---SHARE Examples
									\---data