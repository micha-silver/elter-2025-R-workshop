---
title: eLTER Science Conference - 2025 - Tampere,FI
output:
  html_document: default
  pdf_document: default
linkcolor: blue
urlcolor: blue
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
- Windows users should add the Rtools toolchain from:
  - [RTools](https://cran.r-project.org/bin/windows/Rtools/)
  - matching the version of `R` that was installed
- Install RStudio&trade; from [Posit](https://posit.co/download/rstudio-desktop/)
- Once `R` is installed, the following packages should also be added:
  - `terra`, `sf`, `remotes`, `CDSE`, `rOPTRAM`
  - At the R command line, run:
  - `install.packages(c("terra", "sf", "remotes"), dependencies = TRUE)`
  - `remotes::install_github("zivankaraman/CDSE")`
  - `remotes::install_github("ropensci/rOPTRAM")`

### Authentication on Copernicus DataSpace (CDSE)

- Browse to CDSE [portal](https://dataspace.copernicus.eu)
- Follow steps below to register on CDSE and prepare clientid and secret.
- Save both the clientid and secret to a `csv` text file.

| CDSE Authentication | Steps |
| ----------------------------------- | ----------------------------------- |
|![CDSE-1](../Presentation/figures/CDSE_1.png)|![CDSE-2](../Presentation/figures/CDSE_2.png)|
|![CDSE-3](../Presentation/figures/CDSE_3.png)|![CDSE-4](../Presentation/figures/CDSE_4.png)|
| Create a new OAuth client | Set expiration date and click Create |
|![CDSE-5](../Presentation/figures/CDSE_5.png)|![CDSE-6](../Presentation/figures/CDSE_6.png)|
| Copy both the clientid and the secret... | ... and **save** to `credentials.csv` file |
|![CDSE-7](../Presentation/figures/CDSE_7.png)|![CDSE-8](../Presentation/figures/CDSE_8.png)|

## Exercise data

Each participant can download the exercises and data in advance in one of three ways:

- Particpants who are familiar with `git` can clone the repository: 

`git clone https://github.com/micha-silver/elter-2025-R-workshop.git`

- The same result can be achieved within RStudio&trade; by starting a new Version Control based project, pointing to the same repository;

- Otherwise, the workshop material can be downloaded as a zip archive from [here](https://github.com/micha-silver/elter-2025-R-workshop/archive/refs/heads/main.zip) .


Put your `credentials.csv` file into the same directory as the exercise.

Start RStudio&trade; and load the project "elter-2025-R-workshop".


## License

eLTER Workshop-Analyzing Remote Sensing Data in R 

© 2025 by Micha Silver 

is licensed under Creative Commons Attribution-ShareAlike 4.0 International.

To view a copy of this license, visit https://creativecommons.org/licenses/by-sa/4.0/