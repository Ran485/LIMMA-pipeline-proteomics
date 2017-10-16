# LIMMA-pipeline-proteiomics
Implementation of LIMMA pipeline for two group comparision in proteomics data as described in the paper http://www.sciencedirect.com/science/article/pii/S2212968515000069
If you have a proteingroups file (see Example folder) then just run lima_main.R code. The helper functions must be in the same directory as the main. After successful run it will create two volcano plots and a txt file with data in the present working directory. One plot is using limma moderated pval and the other one using ordinary t-test.
The code will force you to provide as input correct names for treatment and control as it appers in the proteingroups file. Part of the name (case insensitive) should also be fine.
If columns 'Potential contaminant', 'Reverse' and 'Only.identified by site' is not present in the proteingroups file the code terminates with a message.
