# Human_Activity_Recognition

The aim of this project was to predict the type of exercise that each volunteer did, according to the data provided by a smartphone (Samsung Galaxy S II) they were wearing on the waist. 

### Installations

This project requires **Python 3.x** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [XGBoost](https://xgboost.readthedocs.io/)

### Summary

The experiments were carried out with a group of 30 volunteers within an age bracket of 19-48 years. They performed a protocol of activities composed of six basic activities: three static postures (standing, sitting, lying) and three dynamic activities (walking, walking downstairs and walking upstairs). The experiment also included postural transitions that occurred between the static postures. These are: stand-to-sit, sit-to-stand, sit-to-lie, lie-to-sit, stand-to-lie, and lie-to-stand. All the participants were wearing a smartphone (Samsung Galaxy S II) on the waist during the experiment execution. The purpose was to predict these activities based on the data provided by the smartphone.

### Data

The experiments were video-recorded to label the data manually, and the obtained dataset was randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

The dataset is an extended version of the UCI Human Activity Recognition Using smartphones Dataset that can be found at: https://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

The dataset is then divided in two parts and they can be used separately.  

1. Inertial sensor data 
- Raw triaxial signals from the accelerometer and gyroscope of all the trials with with participants. 
- The labels of all the performed activities.
  
2. Records of activity windows. Each one composed of:
- A 561-feature vector with time and frequency domain variables. 
- Its associated activity label. 
- An identifier of the subject who carried out the experiment.

The dataset includes the following files:

- **'RawData/acc_expXX_userYY.txt'**: The raw triaxial acceleration signal for the experiment number XX and associated to the user number YY. Every row is one acceleration sample (three axis) captured at a frequency of 50Hz. 

- **'RawData/gyro_expXX_userYY.txt'**: The raw triaxial angular speed signal for the experiment number XX and associated to the user number YY. Every row is one angular velocity sample (three axis) captured at a frequency of 50Hz. 

- **'RawData/labels.txt'**: include all the activity labels available for the dataset (1 per row). 
   Column 1: experiment number ID, 
   Column 2: user number ID, 
   Column 3: activity number ID 
   Column 4: Label start point (in number of signal log samples (recorded at 50Hz))
   Column 5: Label end point (in number of signal log samples)

- **'features_info.txt'**: Shows information about the variables used on the feature vector.

- **'features.txt'**: List of all features.

- **'activity_labels.txt'**: Links the activity ID with their activity name.

- **'Train/X_train.txt'**: Training set.

- **'Train/y_train.txt'**: Training labels.

- **'Test/X_test.txt'**: Test set.

- **'Test/y_test.txt'**: Test labels.

- **'Train/subject_id_train.txt'**: Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30. 

- **'Test/subject_id_test.txt'**: Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30. 


**Notes:**
- Features are normalized and bounded within [-1,1].
- Each feature vector is a row on the 'X' and 'y' files.
- The units used for the accelerations (total and body) are 'g's (gravity of earth -> 9.80665 m/seg2).
- The gyroscope units are rad/seg.


### Author
Jessica Garre Morales
