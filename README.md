# QMEE
Bio 708

Assignment 2:
My first script reads a csv of startle response assay data. I checked and corrected the R classes of my variables, then plotted the total distance travelled, and max velocity in the first 20s as histograms to visualize the data and determine if there were any errors. The data showed all positive values (as expected), and the only NAs found were the expected blanks before the first measurement, so they were removed from analysis.  Because my variables of interest are maximum velocity in the first 20s of the assay, and total distance over the whole assay time, i made seperate dataframes for each of these variables, and saved them as rds. I set up these rds files to go to my gitignore. 
My second script reads in my two rds files, and confirms that they are dataframes. Then I calculate mean, standard deviation, and standard error by genotpe for maximum velocity for the first 20s and total distance travelled. I don't really know what statistical tests are most appropriate for this type of data, so i hope to increase the complexity of analysis in future assignments as we learn about statistical tests. I didn't have the chance to update my code to reflect the cleaner pipes and groupings we learned in class, but will modify for next assignment and future coding!
The directory that the first file should be run from QMEE/Assignment2_File1_Bio708.Rmd and the second file should be run from QMEE/Assignment2_File2_Bio708.Rmd



Assignment 1:
SETBP1-HD is a genetic disorder in humans caused by a knockout of the SETBP1 gene. SETBP1-HD currently has no treatment. This project aims to test if zebrafish are a good model for SETBP1-HD by inducing the same genetic mutation (SETBP1 knockout) in zebrafish. If zebrafish are a good biomedical model, they can be used to test theraputics for SETBP1-HD in high-throughput. 
SETBP1-HD causes neurodevelopmental disorders in humans, impacting behaviour. Thus, if zebrafish are a good biomedical model for SETBP1-HD, we would expect to see modified behaviour in SETBP1 knockout fish relative to wildtype fish. This is measured through a startle response assay. 
The startle response behavioural assay aims to measure the response of animals to a sudden stimulus (similar to a startle response to a predator).  I want to determine if SETBP1 knockout zebrafish display a "hyperactive" response to startle stimulus. To do so I ask, do SETBP1 knockout zebrafish display a greater distance moved in response to a startle than wildtype fish do? I also ask do SETBP1 knockout fish display a higher maximum velocity swim in response to startle stimulus than wildtype fish (immediately following startle)? Finally, I ask if a hemizygous knockout of SETBP1 has the impacts on velocity and distance travelled as a homozygous knockout does?
This dataset contains four groups of zebrafish, who have been subjected to an auditory startle response stimulus. The first two groups of fish are control fish, one is wildtype ("WT") , and one is another group of wildtype control with a different parent backgroud ("WTSK"). The next group is an experimental group, SETBP1 hemizygous knockouts (KO). The final group is also an experimental group, SETBP1 homozygous knockouts ("KOKO"). 
This makes a boxplot of the total distance travelled during the assay by each of these four groups, with the median noted on the plot.
This also makes a boxplot of the maximum velocity immediately following the startle(first 20s) for each of the groups, with the median value noted on the boxplot. 

In the future I hope to complete statistical tests to identify if differences between any of the groups are statistically significant - but maybe I can do that later in the course once we have learned when to do different tests!
