File with R script "run_analysis.R" performs the data preparation and then followed by the 5 steps required in the course project's instruction.

**i. Download the dataset**
    Dataset downloaded and extracted through the folder named UCI HAR Dataset.
   
**ii. Assign all data frames to variables**
  * features <- features.txt
       * File features.txt contains 561 rows and 2 columns.  
         Accelerometer and gyroscope embedded in a smartphone are used to provide the features for this database.
  * activities <- activity_labels.txt
       * File activity_labels.txt contains 6 rows and 2 columns.  
         Activities list collected during the related measurements were taken and its code labels.
  * subject_test <- test/subject_test.txt
       * File subject_test.txt contains 2947 rows and 1 column.  
         30% of 30 volunteer test subjets being observed and gathered in this test data.
  * x_test <- test/X_test.txt
       * File X_test.txt contains 2947 rows and 561 columns.  
         Test data which recorded features.
  * y_test <- test/y_test.txt
       * File y_test.txt contains 2947 rows and 1 column.  
         Test data which recorded code labels of activities.
  * subject_train <- train/subject_train.txt
       * File subject_train.txt contains 7352 rows and 1 column.  
         70% of 30 volunteer subjects being observed and gathered in this train data.
  * x_train <- train/X_train.txt
       * File X_train.txt contains 7352 rows and 561 columns.
         Train data which recorded features.
  * y_train <- train/y_train.txt
       * File y_train.txt contains 7352 rows and 1 column.  
         Train data which recorded code labels of activities.
         
 **iii. Merges the training and the test sets to create one data set.** 
 * X - Used rbind() function to merge x_train and x_test.  
 * Y - Used rbind() function to merge y_train and y_test.  
 * Subject - Used rbind() function to merge subject_train and subject_test.  
 * Merged_Data - Used cbind() function to merge Subject, X and Y.  
  
 **iv. Extracts only the measurements on the mean and standard deviation for each measurement.**    
 * TidyData is produced by subsetting Merged_Data. Choosing columns("subject", "code" and the measurements) on the mean
      and standard deviation for each measurement.

 **v. Uses descriptive activity names to name the activities in the data set.**  
  * All the numbers in column of "code" of the TidyData replaced with the corresponding activity taken from the second
      column of "activities" variable.  
       
  
