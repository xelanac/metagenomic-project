# Metagenomic project
Application of Recurrent Neural Network to Metagenomic

The scope of this experiment is to train a RNN with two type of datasets: 
* DNA NOT SANITIZED: this one contains informations about microorganisms present into an environment before the sanitizing action;
* DNA SANITIZED: this one contains information after the sanitized action;

After the train, the algorithm should predict a DNA SANITIZED given in input a string of DNA NOT SANITIZED.
For experiment i used Tensorflow with Keras and Nucleus Library (https://nucleus-for-genomics-and-ml.readthedocs.io/en/stable/source/nucleus/io/fastq/) to read and manage the fastQ file.

# PREDICION TASK
Given a character, or a sequence of characters, what is the most probable next character? This is the task which allows to train the model. The input to the model will be a sequence of characters, and training the model to predict the output (the following character at each time step).

During the training of the model i notice that the accuracy of the model is fine for DNA's string length equal or lower to 30. For higher lengths the training need a lot of DNA's string, much bigger datasets.
