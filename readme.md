Team Marci

Bilibók Bence - VRERYK

Péter István - TCTYJW

Rancz Máté - U7EHQC

Goal: The goal of this project is to realize training a neural network to spot drug-drug interactions, based on Variational Graph AutoEncoders. 
Run `training_example.ipynb` to train the model. Training and evaluation is in the same notebook, because of the simplicity of the latter.

We based the data collection on a scraped version of the DrugBank database, provided to us by Dániel Unyi, extracted from a .xml file in our source. 
(https://drive.google.com/drive/folders/1hZa_Vc9dZf_oyNjQoCsO2eKVAOzz-78e). The `features.csv` file extracted by us can be found by accessing [this](https://drive.google.com/drive/folders/1V450xFIj2X1OLxBPbVAt0IWokYd_FOpp?usp=sharing) Google Drive link.

To run data preparation: [data generation](data_generation.ipynb) for dividing the graph, [feature extraction](creating_features.ipynb) for feature extraction.
The former is no longer relevant, as the data provided by it was not used in the final version of the training script, but it is an interesting theoretical possibility for sampling in order to train GAEs. 

The whole Milestone 1 submission, consisting of the above, plus some data visualization, can be found in this Github Gist: https://gist.github.com/peter-i-istvan/581eb0e0251a40b62ef3df76c3193b35

The submission for Milestone 2, updated to be the final submission, is [`training_example.ipynb`](training_example.ipynb). 

To run the training one needs to install the [dependencies](requirements.txt).

The db and data folders were created previously, so only two files needs to be in them, namely the "feature.csv" in the data folder, and the "ChCh-Miner_durgbank-chem-chem.tsv.gz" in the db folder.

The evaluation metrics are printed during training, at the end of each epoch, as well as after the training process, so there is no need for a separate notebook for evaluation. At the end of the training, the AUC_ROC and AP metrics are displayed.

The final report in PDF format can be found in the root of the repository.
