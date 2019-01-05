# Getting-Cleaning_Data_Project
This repository is for Week 4 assignment of Getting and Cleaning Data. 
Find below the details of the R scripts used in this project to get and clean the data for the project.The project is based on the data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

run_analysis.R

The run_analysis.R script is the main script which creates a merged data set and then clean the same to calculate the average of each variable for each activity and each subject as per the requirement of the assignment. The main objective of this script id to :
 1. Merges the training and the test sets to create one data set.
 2. Extracts only the measurements on the mean and standard deviation for each measurement.
 3. Uses descriptive activity names to name the activities in the data set
 4. Appropriately labels the data set with descriptive variable names.
 5. From the data set in step 4, creates a second, independent tidy data set with 
 6.   the average of each variable for each activity and each subject.
To prepare all the above mentioned requirements the run_analysis.R script takes help of the run_analysis_metadata.R script , which help the main script to look clean and evaluations much understandable by defining some functions.

run_analysis_metadata.R

This is a supporting script, which contains the functions required by main script. A brief description for the  functions used in this the script are : 
•	merge_data :  This function take input the path and the 2 files which need to be merged. It appends file1 data to file2 data.
•	get_feature_cols_means_std : It takes the features file name as i/p and return the tidy set of column names and numbers which match with “mean” and “std” as per the requirement.
•	get_activity_names : It read the read the file that contains activity names and numbers.

