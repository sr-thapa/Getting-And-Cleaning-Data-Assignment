#Code Book
This code book includes information about the source data, the transformations performed after collecting the data and some information about the variables of the resulting data sets.

#Study Design

The source data was collected from the UCI Machine Learning Repository to complete an assignment for a Coursera course named Getting and Cleaning Data instructed by Jeff Leek. 

#Section 1. Merge the training and the test sets to create one data set.

 Read  from the data set the data located in

features.txt
activity_labels.txt
subject_train.txt
x_train.txt
y_train.txt
subject_test.txt
x_test.txt
y_test.txt
Assign column names and merge to create one data set.

#Section 2. Extract only the measurements on the mean and standard deviation for each measurement.

Create a logcal vector that contains TRUE values for the ID, mean and stdev columns and FALSE values for the others. Subset this data to keep only the necessary columns.

#Section 3. Use descriptive activity names to name the activities in the data set

Merge data subset with the activityType table to cinlude the descriptive activity names

#Section 4. Appropriately label the data set with descriptive activity names.

 gsub() function for pattern replacement to clean up the data labels.

#Section 5. Create a second, independent tidy data set with the average of each variable for each activity and each subject.

 We need to produce only a data set with the average of each veriable for each activity and subject