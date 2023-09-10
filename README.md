# FASnet
Frequency domain audio separation network

### Data
Relies on BirdClef2022 Challenge Dataset (which is sample from xeno-canto) available via Kaggle API: `kaggle competitions download -c birdclef-2022`

### To-do
* Get a subset (3-4 species) of BirdClef on Google Drive
* Port to Google Collab for GPU access (data access through Google Drive)
* Fix: Labels should be pre-generated and saved with one-hot encoding (not on-fly while training as it consumes time)
* Fix: Loss > 1 Error something to do with softmax and using cross-entropy loss together
* Finetune a TIMM model for this use-case seresnext, efficientnet for better accuracy
