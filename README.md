---
output:
  html_document: default
  pdf_document: default
---

![](eLTER_SC_Logo.png)

# Analyzing Remote Sensing Data with R

## Getting Started

This [Github repository](https://github.com/micha-silver/elter-workshop-2025)
lists the preparatory steps in advance of the workshop, 
and contains the practice exercises that will be covered.

### Required Software

- Install a recent version of `R`, for your operating system from [CRAN](https://cran.r-project.org)
- Windows users should add the Rtools toolchain from:
  - [RTools](https://cran.r-project.org/bin/windows/Rtools/)
  - matching the version of `R` that was installed
- Install RStudio from [Posit](https://posit.co/download/rstudio-desktop/)
- Once `R` is installed, the following packages should also be added:
  - `terra`, `sf`, `remotes`, `CDSE`, `rOPTRAM`
  - At the R command line, run:
  - `install.packages(c("terra", "sf", "remotes"), dependencies = TRUE)`
  - `remotes::install_github("zivankaraman/CDSE")`
  - `remotes::install_github("ropensci/rOPTRAM")`

### Exercise data

## License

eLTER Workshop-Analyzing Remote Sensing Data in R 

© 2025 by Micha Silver 

is licensed under Creative Commons Attribution-ShareAlike 4.0 International.

To view a copy of this license, visit https://creativecommons.org/licenses/by-sa/4.0/