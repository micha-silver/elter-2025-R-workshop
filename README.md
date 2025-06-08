---
title: eLTER Science Conference - 2025 - Tampere,FI
output:
  pdf_document: default
  html_document: default
linkcolor: blue
urlcolor: blue
bibliography: references.bib
---

![](eLTER_SC_Logo.png)

# Analyzing Remote Sensing Data with R

## Getting Started

This [Github repository](https://github.com/micha-silver/elter-workshop-2025)
lists the preparatory steps in advance of the workshop, 
and contains the practice exercises that will be covered.

### Required Software

Each workshop participant should do the following on her laptop:

- Install a recent version of `R`, for your operating system from [CRAN](https://cran.r-project.org)
- Windows users should add the Rtools toolchain;
  - from: [RTools](https://cran.r-project.org/bin/windows/Rtools/)
  - matching the version of `R` that was installed
- Install RStudio&trade; from [Posit](https://posit.co/download/rstudio-desktop/)
- Once `R` is installed, the following packages should also be added:
  - `terra`(@hijmans_2025_terra), `sf`, `remotes`, `CDSE`(@R-CDSE), `rOPTRAM`(@silver_2023_roptram), `leaflet`, `ggplot2`;
  - At the R command line, run:
  - `install.packages(c("terra", "sf", "remotes", "ggplot2", "leaflet"), dependencies = TRUE)`
  - `remotes::install_github("zivankaraman/CDSE")`
  - `remotes::install_github("ropensci/rOPTRAM")`

### Authentication on Copernicus DataSpace (CDSE)

- Browse to CDSE [portal](https://dataspace.copernicus.eu)
- Follow steps below to register on CDSE and prepare clientid and secret.
- Save both the clientid and secret to a `csv` text file.

| CDSE Authentication | Steps |
| ----------------------------------- | ----------------------------------- |
|![CDSE-1](../Presentation/figures/CDSE_1.png)|![CDSE-2](../Presentation/figures/CDSE_2.png)|
| Browse to portal | Register for an account (of Login if you already have an account)
|![CDSE-3](../Presentation/figures/CDSE_3.png)|![CDSE-4](../Presentation/figures/CDSE_4.png)|
| Go to Sentinel Hub | Open User settings | 
|![CDSE-5](../Presentation/figures/CDSE_5.png)|![CDSE-6](../Presentation/figures/CDSE_6.png)|
| Create a new OAuth client | Set expiration date and click Create |
|![CDSE-7](../Presentation/figures/CDSE_7.png)|![CDSE-8](../Presentation/figures/CDSE_8.png)|
| Copy both the clientid and the secret... | ... and **save** to `credentials.csv` file |

## Workshop Exercise

### Code and data

The exercise focuses on Doñana Park in Spain. (@green_groundwater_2024).

Each participant can download the exercises and data in advance in one of three ways:

- Particpants who are familiar with `git` can clone the repository: 

`git clone https://github.com/micha-silver/elter-2025-R-workshop.git`

- The same result can be achieved within RStudio&trade; by starting a new Version Control based project, pointing to the same repository;

- Otherwise, the workshop material can be downloaded as a zip archive from [here](https://github.com/micha-silver/elter-2025-R-workshop/archive/refs/heads/main.zip);

Put your `credentials.csv` file into the same directory as the exercise.

Start RStudio&trade; and load the project "elter-2025-R-workshop".

### Exercises

- Load packages, set parameters;
- Query CDSE catalog for available images;
- Filter for low cloud cover, and only a single Copernicus tileId;
- Loop over list of available image dates;
- Derive MNDWI index for each image;
- Threshold MNDWI to obtain open water surfaces;
- Plot time series of MNDWI values;
- Prepare OPTRAM model from list of available dates;
- Derive soil moisture for one date using model coefficients.


## License

eLTER Workshop-Analyzing Remote Sensing Data in R 

© 2025 by Micha Silver 

is licensed under Creative Commons Attribution-ShareAlike 4.0 International.

To view a copy of this license, visit https://creativecommons.org/licenses/by-sa/4.0/

## References