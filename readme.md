Marci

Bilibók Bence - VRERYK

Péter István - TCTYJW

Rancz Máté - U7EHQC

Goal: The goal of this project is to realize a learning based on Variational Graph AutoEncoders. 

Achievements: For the moment the data collection is realized, extracted from a .xml file from our source. 
(https://drive.google.com/drive/folders/1hZa_Vc9dZf_oyNjQoCsO2eKVAOzz-78e)

To execute: [data generation](data_generation.ipynb) for dividing the graph, [feature extraction](creating_features.ipynb) for feature extraction

Github Gist: https://gist.github.com/peter-i-istvan/581eb0e0251a40b62ef3df76c3193b35

Folder structure:
|folder|use|
|--|--|
|data|Train. validation and test split|
|db|The database downloaded from the Google Drive link|

To run the training we need to:

- need to install dependencies

- set the hyperparameters

- define the model

- data preprocessing

- loading the data

 - creating the model and the optimizer
 
The db and data folders were created previously, so only two files needs to be in them, namely the "feature.csv" in the data folder, while the "ChCh-Miner_durgbank-chem-chem.tsv.gz" in the db folder.

For the metrics evalution it is not needed to add anything else, it is already implemented in the training part, during the epoches, every metric is displayed. At the end of the training, the AUC_ROC and AP metrics are displayed.
