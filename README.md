# Ovarian-DataDescriptor

This project involves the analysis of immune repertoire data obtained from the blood samples of healthy donors (HD) and ovarian cancer (OC) patients. 
The immune repertoire data includes T-cell receptor alpha (TRA) and beta (TRB) sequences obtained through Repertoire Sequencing (Rep-Seq).

This repository accompanies the publication:

**Zuckerbrot-Schuldenfrei, M.**, *et al.*  
**"The compositional behavior of the human T cell receptor repertoire in ovarian cancer compared to healthy donors"**  
*Scientific Data*, 2025.  
[https://www.nature.com/articles/s41597-024-04335-4](https://www.nature.com/articles/s41597-024-04335-4)

## Data Collection and Processing

1. **Blood Collection:**
   - Blood samples were collected from healthy donors and ovarian cancer patients.

2. **Repertoire Sequencing (Rep-Seq):**
   - Repertoire Sequencing was performed on the collected blood samples to obtain TRA and TRB sequences.

3. **Data Processing with MiXCR:**
   - The obtained raw sequencing data went through the MiXCR pipeline for processing.

4. **Concatenation of TRA and TRB Files:**
   - The processed TRA and TRB files were concatenated for further analysis.

## Data Analysis

### Immunarch Analysis

- **initial_stats.Rmd:**
  - This script provides an initial analysis of the TCR repertoire data using the `immunarch` package. It calculates basic statistics including clone count, average clone count per sample, clonotype count, and average clonotype count per sample. The results of this analysis offer a comprehensive overview of the TCR repertoire characteristics for alpha and beta chains separately. 

- **subsampling_analysis.Rmd:**
  - After concatenation of TRA and TRB files per sample, this script performs subsampling and further analysis to compare unique clonotypes, clonality, and diversity between samples from OC and HD. Subsampling allows for an unbiased comparison of TCR repertoire features between groups by equalizing the sample sizes. 

## Usage

- The analysis can be reproduced by following the steps outlined in each analysis script.
- Immunarch package version 0.9 was used.

## Data Availability

- The raw data is available on Zenodo.
