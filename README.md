# GNN-Text-Classification
Text Classification using Graph Neural Network(GNN)

What does it classify? : News articles as Input text

Dataset used : AG News Dataset ( From Hugging Face)

Run on : Google Colab

**********************************************************************************************************************************************
# Steps on Running it in GColab:

* Mounts the GDrive(For any doubts refer to any instructions online)

> from google.colab import drive

> drive.mount('')

> %cd 'path'

> !ls

* Installs the requirements

> !pip install torch torch-geometric scikit-learn transformers

> !pip install datasets

> !pip install tqdm

* Downloads the needed data

> !python data_download.py

* The initial train module. No need to run a second time, since it downloads some dependencies and other for the model

> !python train.py

* The main training module. Can be run again and again for increasing prediction confidence 

> !python off_train.py

* A test non-gui version of main file

> !python predict.py

* Dependecy for GUI

> !pip install gradio

* Gui version of classifier

> !python gui_predict.py

***********************************************************************************************************************************************
