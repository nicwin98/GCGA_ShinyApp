[![DOI](https://zenodo.org/badge/527985404.svg)](https://zenodo.org/badge/latestdoi/527985404)

# GCGA Shiny App

This app displays RNA sequencing data from livers of female mice treated for eight weeks with the glucagon analogue, NNC9204-0043, compared to female mice treated with PBS (control group) as presented in

## Publication
"Opposing effects of chronic glucagon receptor agonism and antagonism on amino acids, hepatic gene expression, and alpha cells"

Emilie Elmelund, Katrine D. Galsgaard, Christian D. Johansen, Samuel A. J. Trammell, Anna B. Bomholt, Marie Winther-Sørensen, Jenna E. Hunt, Charlotte M. Sørensen, Thomas Kruse, Jesper F. Lau, Trisha J. Grevengoed, Jens J. Holst, and Nicolai J. Wewer Albrechtsen.

iScience (2022), DOI: https://doi.org/10.1016/j.isci.2022.105296

## Local App Launch
If you wish to view the app online, it is accessible here:
  
https://weweralbrechtsenlab.shinyapps.io/GCGA/ 

If you would like to run the app from github, you will need a few R packages:

```{r}
install.packages(c(shiny, EnhancedVolcano, tidyverse, DT, tidyverse, shinyjs, writexl, plotly))
```

Once you have all the packages installed, simply run these lines in R. It will download the app and display it in a browser window:

```{r}
library(EnhancedVolcano)
library(tidyverse)
library(DT)
library(shiny)
library(shinyjs)
library(shinythemes) 
library(writexl)
library(plotly)

runGitHub(rep = "GCGA_ShinyApp", username = "nicwin98", ref = "main")
```
