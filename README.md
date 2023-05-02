# CS598DL4H_Final_Pj
This project is about reproducing the ConCare model presented in the paper "ConCare: Personalized Clinical Feature Embedding via Capturing the Healthcare Context" by Zhang et al. The paper can be accessed at [here](https://arxiv.org/abs/1911.12216).

## Requirements
All the code is completed in Google Colab Pro environment.

## Dataset
The project uses MIMIC-III dataset to do the in-hospital mortality prediction task. You need to gain access and download the dataset from https://mimic.physionet.org/ by yourself. Once you have downloaded the data, place it in the folder called **mimic-iii-clinical-database-1.4**. To build the dataset, run the file **prepare_dataset.ipynb**. It takes over 20 hours to build the dataset in Google Colab Pro environment. The project uses the same code from https://github.com/YerevaNN/mimic3-benchmarks/ to build the task-specific dataset.

In addition, the static demographic data can be downloaded from https://drive.google.com/file/d/1TXn4UdtQCzfd7TdDJAo_6_IcnO2LUa1a/view?usp=sharing, which is provided by the original author. Since the number of files in the demographic data is very large, you need to separate them into 5 folders demo1, demo2... Save it in the directory **data/hospital-mortality**. Run the file **demographic.ipynb** to process the demographic data.

## Model
To build and train the ConCare model, run the file **ConCare.ipynb** directly. The trained model is in the directory **model/concare0**. It takes 4 hours to load the training data and 1 hour to train the model in the Google Colab Pro environment.

If you have any questions or comments about this project, please feel free to contact me. Thank you!
