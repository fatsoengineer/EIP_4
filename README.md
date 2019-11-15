# EIP_Week_1

Assignment Score: [0.032171424890264276, 0.9918]

Group Members:
Sakthi Ganesh M - https://github.com/yasuo19/EIP4-Week-1 


## Convolution:
 
 Convolution is the process or method by which we try to project or extract the features or information of multiple pixels onto one pixel which can be also called as receptive field on the pretext that one pixel contains the the information of the multiple pixels the convolution was applied on, using which they could possibly extract edges and gradients to define distinct features, which in turn helps the neural network to define the combination of edges and textures required to define an object. It combines the image matrix (values ranging between 0-1 after standardization) and the kernel matrix (randomly initialized).


 ## Filters/Kernels
Filters/Kernels is a N*N matrix which contains information of a particular features/edges/textures/parts/ objects. They distinguish and filter out distinct edges and features. They are randomly initialised and updated after every epoch.


## Epochs
Epoch is the number of times the entire training set is used to update the weights of the kernel. After every epoch, the loss is calculated and back-propogation is done to reduce the loss, update the weight and refine the model.


## 1*1 Convolution

1*1 matrix is used to reduce the no of channels of an N*N*M matrix, where M is the no of channels. It mainly focuses on one pixel rather than the surrounding pixel to reduce the number of channels, hence providing more accurate features.


## 3*3 Convolution

3*3 Convolution is an operation which extracts the features or information of 3*3 pixels onto 1*1 pixel which can be also called as receptive field on the pretext that one pixel contains the the information of the multiple pixels the convolution was applied on, using which they could possibly extract edges and gradients to define distinct features.


## Feature Maps

Feature maps are the end-result of filters to an input or intermediate images which helps us to identify the distinct features the neural network has detected after certain layer.


## Activation Function

Activation function clips the outlier weights to normalise it within certain range and then adds a bias to the weight.

## Receptive Field

Receptive Field is the culmination of information/features of N*N kernel matrix. Receptive Field of the last layer (Global Receptive Field) must atleast be equal to the size of the object. Also, the Local Receptive Field is equal to the size of the kernel. For every 3x3 Convolutional Layer, the Global Receptive Field increases by 2 (3*3 -> 5*5 -> 7*7 -> 9*9 and so on) while the Local receptive field remains constant at(3x3).

