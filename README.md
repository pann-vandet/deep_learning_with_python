# deep_learning_with_python
This repository includes my notebooks on the book "Deep Learning with Python" by Francois Chollet (2018). This series of notebooks show how to build neural networks using Keras.   
- [Keras documentation](https://keras.io)
- [Official GitHub page](https://github.com/fchollet/deep-learning-with-python-notebooks) by Francois Chollet.
- [Manning publications](https://www.manning.com/books/deep-learning-with-python)  

## [chap2-1_first_neural_network_for_recognizing_handwritten_digits](https://github.com/ksonod/deep_learning_with_python/blob/master/chap2-1_first_neural_network_for_recognizing_handwritten_digits.ipynb)  
MNIST handwritten digits are classified using a fully-connected neural network.

## [chap3-1_binary_classification_IMDB](https://github.com/ksonod/deep_learning_with_python/blob/master/chap3-1_binary_classification_IMDB.ipynb)
<strong>Abstract</strong>    
In this notebook, neural networks will be build for classifying movie reviews provided by IMDB. This is a <strong>binary classification</strong> example.   

<strong>Reference</strong>    
See pages 68-77 of "<strong>Deep Learning with Python</strong>" by Francois Chollet (2018).  

<strong>Summary (page 77)</strong>    
- For a binary classification problem, the final activation function should be sigmoid, which returns a value between 0 and 1.
- An appropreate loss function is binary_crossentropy.
- Check whether there is a problem of overfitting.


## [chap3-2_multiclass_classification_reuters](https://github.com/ksonod/deep_learning_with_python/blob/master/chap3-2_multiclass_classification_reuters.ipynb)  
<strong>Abstract</strong>  
In this notebook, neural networks will be build for classifying topics of Reuters' newswires. This is a multiclass classification example.  

<strong>Reference</strong>  
See pages 78-84 of "Deep Learning with Python" by Francois Chollet (2018).  

<strong>Summary (page 84)</strong>  
- For a multiclass classification problem, the final activation function should be softmax, which returns a value between 0 and 1.
- An appropreate loss function is categorical_crossentropy.
- If you want to classify data with N labels, try to avoid using layers whose nodes are less than N.


## [chap3-3_regression_house_prices](https://github.com/ksonod/deep_learning_with_python/blob/master/chap3-3_regression_house_prices.ipynb)
<strong>Abstract</strong>   
In this notebook, neural networks will be build for predicting house prices. This is a <strong>regression</strong> example.

<strong>Reference</strong>   
See pages 85-91 of "<strong>Deep Learning with Python</strong>" by Francois Chollet (2018). 

<strong>Summary (page 91)</strong>   
- Regression is done using different loss functions. Mean squared error (MSE) is a loss function commonly used for regression.
- As an evaluation metric, mean absolute error (MAE) can be used.
-  When little training data is available, <strong>K-fold cross-validation</strong> is a powerful method to reliably evaluate a model.
- When little training data is available, it is preferable to use a small network with few hidden layers (typically one or two) in order to avoid overfitting. 

## [chap4-1_overfitting_regularization_dropout](https://github.com/ksonod/deep_learning_with_python/blob/master/chap4-1_overfitting_regularization_dropout.ipynb)  
<strong>Abstract</strong>  
In this notebook, various neural networks will be build to learn <strong>overfitting</strong> and <strong>regularization</strong>.

<strong>Reference</strong>  
See pages 104-118 of "<strong>Deep Learning with Python</strong>" by Francois Chollet (2018). 

<strong>Summary (page 118)</strong>  
Below are knacks for avoiding overfitting:
- Get more training data.
- Reduce the capacity of the network.
- Add weight regularization.
- Add dropout.


## [chap5-1_basics_of_convolutional_neural_network](https://github.com/ksonod/deep_learning_with_python/blob/master/chap5-1_basics_of_convolutional_neural_network.ipynb)

<strong>Abstract</strong>  
In this notebook, a convolutional neural network will be build using [Keras](https://keras.io). A basic usage will be described.
- Number of parameters.
- Sizes of inputs and outputs.
- [Convolution](https://keras.io/layers/convolutional/)
- [Max pooling](https://keras.io/layers/pooling/)
- Padding

<strong>Reference</strong>  
See pages 120-129 of "<strong>Deep Learning with Python</strong>" by Francois Chollet (2018). 

<strong>Summary</strong>  
- Convolution layers learn local patters in contrast to dense layers that learn global patters (page 122, 123, see also Fig. 5.2).  
- The patterns that the convolutional neural networks learn are translation invariant (page 123). 
- The convolution is typycally done with the convolution window is 3 x 3 or 5 x 5 (page 124) and no stride (page 128).
- The max-pooling operation is used (page 127) to downsample the feature map, which results in reducing the number of feature-map coefficients to process (page 128). This operation is done with 2 x 2 windows with stride 2 in order to downsample the feature maps by a factor of 2 (page 127-128). 
- Even though there are other ways to achieve downsampling, max pooling tends to work better (page 129).


## [chap5-2_cats_vs_dogs](https://github.com/ksonod/deep_learning_with_python/blob/master/chap5-2_cats_vs_dogs.ipynb)
<strong>Abstract</strong>  
In this notebook, convolutional neural networks will be build to classify cats and dogs. You will see how to build convolutional neural networks, implement data augmentation, do feature extraction, and perform fine-tuning. 

<strong>Reference</strong>  
See pages 130-159 of "<strong>Deep Learning with Python</strong>" by Francois Chollet (2018). 

<strong>Summary (page 159)</strong>  
- Data augmentation is a powerful method to avoid overfitting when working with image data.
- You can reuse an existing convolutional neural networks on a new dataset via feature extraction.
- As a complement to feature extraction, you can use fine-tuning.  
  
 
## [chap5_3_visualizing_intermediate_activations](https://github.com/ksonod/deep_learning_with_python/blob/master/chap5_3_visualizing_intermediate_activations.ipynb)

<strong>Abstract</strong>  
In this notebook, Intermediate outputs of convolutional neural networks will be visualized.

<strong>Reference</strong>  
See pages 160-166 of "<strong>Deep Learning with Python</strong>" by Francois Chollet (2018). 

<strong>Summary (page 160)</strong>  
Visualization of intermediate outputs of convnet (intermediate activations) is useful for understanding how successive convnet layers transform their input and for getting an idea of the meaning of individual convnet filters.
