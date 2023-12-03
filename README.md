# MLCS-Lab2: Backdoor Attacks

## Overview
This project is dedicated to the design of a backdoor detector for neural networks, specifically targeting BadNets. By employing a pruning defense mechanism, the detector evaluates the robustness and reliability of these networks against backdoored test data, as well as their performance on clean data.

## Prerequisites
- **Python Version**: 3.8 or higher.
- **Required Libraries**: 
  - `h5py`
  - `numpy`
  - `tensorflow`
  - `keras`
  - `sklearn`

## Installation and Setup

### Install Dependencies
To set up your environment for running the code, install the necessary libraries using pip:
```bash
pip install h5py numpy tensorflow keras sklearn
```

### Load the Notebook

Open the Jupyter notebook named ML_Lab_2.ipynb in your preferred Jupyter environment.

Execution Guide
Run the Notebook
Follow these steps within the notebook:

### Import Libraries: Start by importing all the necessary libraries.

Load the Model: Load the BadNet model from the file bd_net.h5.
Prune the Model: Implement pruning on the last pooling layer of the model at various levels (2%, 4%, 10%).
Evaluate Models: Assess the performance of each pruned model on both clean and backdoored test data.
Save Models: The pruned models will be saved for future reference or use.

### Model Evaluation

The notebook is designed to automatically output the accuracy and attack success rate for each pruned model level.

### Additional Notes

Ensure the presence of the BadNet model file bd_net.h5 and the necessary validation dataset in the same directory as the notebook.
The pruned models will be stored in a directory named models.
