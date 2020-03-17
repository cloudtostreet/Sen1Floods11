# Sen1Floods11
Sen1Floods11: a georeferenced dataset to train and test deep learning flood algorithms for Sentinel-1 (Example)

The dataset is available for download at: gs://cnn_chips/

You can download the dataset to the folder that notebooks expect it to be in by running

mkdir /home/files3
gsutil -m rsync gs://cnn_chips /home/files3

Main_Training_Stuff.ipynb runs shows how to go through the training loop with the dataset.

Test_Models.ipynb runs shows how to go evaluate a model on the test sets.
