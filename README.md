# CleaningDataProject
Getting and Cleaning Data Course Project

The file run_analysis.R loads the data, transforms it and generates the result.

The script first defines a generic functions to load the different data files for the measurements, training label, subject etc. These functions also include appropriate definition of column headers. The functions are then executed to obtaint that data for test and training. Note, the function assume that the directory structure in train and test is similar. The type of data (train or test) can be specified along with the directory for this dataset.

The results of these functions are then combined to form a training and test set. These two dataframes are then merged into one dataset.

Afterwards the measurements for mean and std are extracted by regular expression on the column names.

The data ist then melted down into the id variables subject and Label (Label represents the acitivity). The melted down data is then aggregated per subject and Label by mean aggregate function.

All steps are described in detail in the script.




