Getting and Cleaning Data Course Project
========================================

This file describes how to run run_analysis.R script works.

* First unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and rename the folder with "data".
* The downloaded data from above and the script 'run_analysis.R' should be in the same folder.
* Use `source("run_analysis.R")` command in RStudio.
* You will find two output files are generated in the current working directory (i.e inside 'data' folder)
    * 'merged_clean_data.txt': It contains a data frame called cleanedData.
    * 'result_set_averages.txt': It contains a data frame called result.
* Finally, use `data = read.table("result_set_averages.txt")` command in RStudio to read the file. Since we are required to get the average of each variable for each activity and each subject, and there are 6 activities in total and 30 subjects in total, we have 180 rows with all combinations for each of the 66 features.