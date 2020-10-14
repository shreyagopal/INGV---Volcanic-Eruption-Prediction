# Data Files

* train.csv Metadata for the train files.

* `segment_id`: ID code for the data segment. Matches the name of the associated data file.
* `time_to_eruption`: The target value, the time until the next eruption.

* [train|test]/*.csv: the data files. Each file contains ten minutes of logs from ten different sensors arrayed around a volcano. The readings have been 
normalized within each segment, in part to ensure that the readings fall within the range of int16 values. If you are using the Pandas library you may find 
that you still need to load the data as float32 due to the presence of some nulls.
