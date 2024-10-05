
# Model Training for Road Detection on Satellite Imagery

This repository contains two Python notebooks aimed at training a deep learning segmentation model for road detection on satellite imagery.

## Notebooks

### Data Acquisition

**File:** `data_acquisition.ipynb`

This notebook contains code to download and preprocess satellite and cartographic data. The prepared data is used in the second notebook.

### Model Training and Evaluation

**File:** `model_training.ipynb`

This notebook includes code to prepare the input data, train the model, track experiments, visualize results, and reconstruct road geometry from the model output.

## Run environments

These notebooks can be run locally or on Google Colab. 

### Local

If the notebooks are run locally, the output data of each notebook is written to local subfolders. 

It is possible to run only the *model_training* notebook, using already existing data. You can download the data from the link below. Unzip the packaged file to the *data/* folder in the notebook's location.

https://drive.usercontent.google.com/download?id=1--iKvkhO7M_dtXPaq1ptQUasDWnhd07b&export=download&confirm=t

### Google Colab

When run in Google Colab, it will export the results to a folder in Google Drive. Please make sure to update the desired path in your Google Drive beforehand.

## MLFlow credentials

The model_training notebook uses MLFlow and Dagshub for experiment tracking. You need to provide valid URL and credentials to an MLFlow server you have access to to run the "Training with experiment tracking" and "Explore results" sections.

It's also possible to modify the code to use a local model in the "Explore results" section to use a model available locally or from a different remote source.