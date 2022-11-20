To run the training we need to: 

- need to install dependencies
- set the hyperparameters
- define the model
- data preprocessing
- loading the data
- creating the model and the optimizer

The db and data folders were created previously, so only two files needs to be in them,
namely the "feature.csv" in the data folder, while the "ChCh-Miner_durgbank-chem-chem.tsv.gz"
in the db folder.

For the metrics evalution it is not needed to add anything else, it is already implemented 
in the training part, during the epoches, every metric is displayed. At the end of the training, the AUC_ROC and
AP metrics are displayed.