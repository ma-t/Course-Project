# Coursera Getting and Cleaning Data_Course Project

1. Unzip the source ( https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip ) into a folder on your local drive, say /Users/yourname/Coursera/

2. Put run_analysis.R to  /Users/yourname/Coursera/UCI HAR Dataset/

3. Do in RStudio: setwd("/Users/yourname/Coursera/UCI HAR Dataset/") and then: source("run_analysis.R")
The latter will run the R script, it will read the dataset and write these files:

  merged_clean_data.txt  -- 8.35 Mb, a 10299x68 data frame
  data_averages.txt  -- 0.225 Mb, a 180x68 data frame

The script normally runs for ~30 seconds, but the exact number depends on your system.

4. Use data <- read.table("data_averages.txt") to read the latter.
It is 180x68 because there are 30 subjects and 6 activities, thus "for each activity and each subject" means 30*6=180 rows.
  
