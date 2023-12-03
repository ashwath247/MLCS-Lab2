# MLCS-Lab2

Backdoor Attacks

Overview
This project focuses on designing a backdoor detector for BadNets using a pruning defense. The detector prunes the last pooling layer of a BadNet model and evaluates its performance on clean and backdoored test data.

Prerequisites
Python 3.8 or higher
Libraries: h5py, numpy, tensorflow, keras, sklearn
Steps to Run the Code
Install Dependencies: Install the required libraries using pip:

Copy code
pip install h5py numpy tensorflow keras sklearn
Load the Notebook: Open the Jupyter notebook ML_Lab_3.ipynb.

Run the Notebook: Execute each cell in sequence. Key steps include:

Importing necessary libraries.
Loading the BadNet model.
Pruning the last pooling layer of the model at different levels (2%, 4%, 10%).
Evaluating the pruned models on clean and backdoored test data.
Saving the pruned models.
Model Evaluation: The notebook will output the accuracy and attack success rate for each pruned model.

Additional Notes
Ensure the BadNet model file bd_net.h5 and the validation dataset are in the same directory as the notebook.
The pruned models are saved in the models directory.
