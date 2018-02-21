
Summary:
One of the most exciting areas in all of data science right now is wearable computing - see for example this article . Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. 

Sources:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
Data:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Files:   run_analysis.R 
I have added a function to perform all the required tasks & added comment Question 1 - 5.

This file contains the main code to perform the various activities required:

1.Merges the training and the test sets to create one data set.
	# Download File , 
	# Question 1 Reading Data 
	#  Reading Training Data:
	#  Reading testing Data:
	#  Reading Features Data:
	# Reading Activity Labels Data:
	# Assigning Column Names:
	# Merging Train Data, Test Data & All:
	

2. Extracts only the measurements on the mean and standard deviation for each measurement.
	# Reading column names:
	# Creating Vector for defining ID, Mean and Standard Deviation:
	# Making necessary subset from setAllInOne:
		

3. Uses descriptive activity names to name the activities in the data set
	# Added the activitylabel & merged

4. Appropriately labels the data set with descriptive variable names.
	# Mentioned the names in Step 2 & 3 above
	# activityId, subjectId, activityType

5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
	# Creating the secondTidySet
	# Writing to a file

Output File Generated:
1. Once you run the script, it will generate secondTidySet.txt file with tidy data set.

Variables Used:

1. datafile —> Variable to store the downloaded file data/datafile.zip
2. x_train —> Reading X_train.txt
3. y_train —> Reading y_train.txt
4. subject_train —> subject_train.txt

5. x_test —> Reading X_test.txt
6. y_test —> Reading y_test.txt
7. subject_test —> subject_test.txt

8. features —> reading features data
9. activityLabels —> reading activity labels data

10. mrg_train —> Adding  columns data from x_train, y_train & subject_train 
11 mrg_test —> Adding column data from x_test, y_test & subject_test

12. mean_and_std —> Vector for defining mean , SD & IDs

13. setForMeanAndStd —> Filtering data set where mean_and_std is true

14. setWithActivityNames —> Added activityLabel & merged

15. secondTidySet —> Created a second tidy data set 




