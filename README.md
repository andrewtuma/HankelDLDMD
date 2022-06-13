# Hankel_DMD

Example:

To run the machine on pendulum dataset, navigate to examples/pendulum. Input the desired number of epochs, batch size, initial number of delay-dimensions (typically set to 1), and learning rate. 

Run Train_Pendulum.py

Data.py is used to create the dataset if it does not already detect a dataset for that example (be sure to make a new dataset if you make any changes to parameters).
DLDMD.py houses the encoder/hankel-dmd algorithm/decoder. HelperFuns.py contains functions used for plotting.
LossDLDMD.py defines the loss function (making a call to DLDMD.py to compute the dmdloss). 
Training.py runs each epoch for designated training/validation sets and produces command line updates on loss value and time/epoch as well as output plots in examples/pendulum/training_results/. 

The final model will be loaded into the folder examples/pendulum/trained_models/. 
