# Getting_and_Cleaning_Data_Course_Project

### Introduction ###

* The objective of this Getting and Cleaning Data course project is to show the ability to collect, work with and clean a data set. The goal 
is to produce a tidy data that can used for later analysis.

* This repository is a submission for the course project. The course project has the instructions on how to conduct analysis on Human Activity
Recognition Using Smartphones dataset.

### Data for the course project ###

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

### Files ###

* **run_analysis.R** deals with data preparation and the 5 steps required as stated in the course project's instruction:
   1. Merges the training and the test sets to create one data set.  
   2. Extracts only the measurements on the mean and standard deviation for each measurement.
   3. Uses descriptive activity names to name the activities in the data set
   4. Appropriately labels the data set with descriptive variable names. 
   5. From the data set in step 4, creates a second, independent tidy data set with the average 
      of each variable for each activity and each subject.
      
* **FinalTidyData.txt** is the exported data which is clean and tidy. It generated after executing all the 
  steps described above.

* **CodeBook.md** is a code book that shows the variables, the data, and progressions to generate clean data for later analysis. 
