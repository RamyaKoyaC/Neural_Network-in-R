# Neural_Network-in-R
How to create a simple neural network using R 

## This is an already in built library which has dataset 
library(datasets) 


## This gives information on what are the input variables in dataset considered. 
names(infert) 
## Loading the neural net library
library(neuralnet)

# Here we are trying to build a neural net with 2 input variables and one fixed output. 
# The hidden layers are numbered 2 here. We are traning the network here
nn <- neuralnet(
  case~age+parity, hidden=2, linear.output=FALSE)
# To know what a neural network data has  
nn 
# plotting the neural network with 2 hidden layers and 2 inputs 
plot(nn) 
