# GNN-Text-Classification
Text Classification using Graph Neural Network(GNN)

What does it classify? : News articles as Input text

Dataset used : AG News Dataset ( From Hugging Face)

Run on : Google Colab

# Repo Info

Here I am going to include all the files that I have pulled from the Colab Notebook, which includes the model and dataset. If you wish you can delete it, as all the modules here help create a new model, and download the new dataset. Or you can keep it, but no harm in keeping it new. 

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

# Result

Predicts the user input text to 4 different labels: 1. World, 2. Business, 3. Sports, 4. Sci/Tech

If the confidence score is low, you can keep training the model or if not, go through all the code to make changes.
