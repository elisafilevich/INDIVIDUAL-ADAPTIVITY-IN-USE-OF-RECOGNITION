# Individual_Adaptivity_in_use_of_Recognition
Experimental scripts, data and analysis scripts for Filevich, Horn and Kühn, Psychological Research (2017) 

The experiment requires JATOS (www.jatos.org) to run. It was designed to run on a server but can be easily run locally. 

To reproduce the results and all figures, run:

    fullPath = 'your/path/to/files/here'
    setwd(fullPath)

The following command will run all analyses and produce all result figures included in the main text
`rmarkdown::render(paste(fullPath,'/scripts/Filevichetal_1_AllSubjs.R', sep=""))`

The following command will run all analyses and produce all result figures included in the Supplementary Material
`rmarkdown::render(paste(fullPath,'/scripts/Filevichetal_2_SI_and_cleanSubjs.R', sep=""))`

You will need multiple R packages:

    library(ggplot2)
    library(BayesFactor)
    library(gridExtra)
    library(lsr)        # compute effect sizes (cohensD) in ttests
    library(R.matlab)
    library(plyr)       # to summarize data and required before dplyr
    library(dplyr)      # for renaming columns 
    library(reshape)    # melt and cast functions
    library(knitr)


