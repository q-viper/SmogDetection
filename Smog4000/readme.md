# SmogDetection
## Description
* Libraries used: keras 2.2.4, numpy, matplotlib etc
* Trained: On google Colab
* Dataset Used: Smog4000 

## About dataset:
Our team member Agata have written everything about dataset on her [repo](https://github.com/agatagruza/SmogDetection).

## Preprocessing of data
* Rescale range: 1./255
* shear and zoom: 0.2
* color: RGB
* Outshape: 224 X 224

## About the model
Custom CNN model is used here. Complete summary of model architecture is given below:
<img src = 'https://github.com/q-viper/SmogDetection/blob/master/Smog4000/Assets/model.JPG'>
<br/>
The Sequential model have 3 blocks of CNN layers and one final linear layer. In each CNN block we have:
* Convolution layers of same out filters(32, 32, 64, 64, 128, 128)
* Filter shape: (3, 3)
* Activation Function: relu(Rectified Linear Unit)
* MaxPooling: pool size(3, 3)
* BatchNormalization
* Dropout: 0.25

The Final block is for linear layers. It has:
* Flatten
* Dense of out 256 and relu
* BatchNormalization
* Dropout of 0.5
* Classification layer with sigmoid

* Total parameters: 1,469,346

## Model Compilation
* Optimizer: Adam(Adaptive Momentum) Optimizer is used on this model.
* Learning rate: default(0.001)
* Loss function: Categorical_crossentropy (categories: clear, smog)

## Training
* Epochs:  10
* Batch Size: 32


## Performance
* Train Accuracy: 0.9968
* Validation Accuracy: 0.9921
* Test Accuracy: 0.985
* Train time: 750s per epochs

## Future Implementations:
* Usage of less parameters
* Test with different optimizer and loss functions

## Find the Pytorch code for this project [here](#). 
