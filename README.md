# Dog-sentiment-analysis
This project takes a dog image and classifies it into sad, happy or angry!



# The Api code is contained inside the zip file
The main file (techdome.ipynb) contains two methods of making a model for recognizing dog emotions, the first model is however more succesful and used for our api.
there are some differences in pre processing and data generation techniques used for the two models apart from their architectures.

The final model is available at: https://drive.google.com/file/d/11CwNHMxTkEpl-qlypckDuGsJfV6E5qYb/view?usp=share_link .

Please put the model in the same directory as the code.


![image](https://github.com/Rakshit2214/Dog-sentiment-analysis/assets/75312508/1357b310-ebf2-4536-aad2-ab8ceb833d2a)


The first model is composed of several convolutional and pooling layers, followed by a series of fully connected layers. It has a final softmax activation layer with as many neurons as the number of classes to be predicted. This model is compiled with an RMSprop optimizer and trained with sparse categorical cross-entropy loss and accuracy as a performance metric.

The second model is a similar Convolutional Neural Network, but with different configuration of the layers. It has 6 convolutional layers with progressively increasing filter size followed by batch normalization and activation functions. After each convolutional layer there is a max pooling and dropout layer to improve model generalization. It ends with a dense layer and a softmax activation layer with 4 neurons. This model is compiled with the Adam optimizer and trained with sparse categorical cross-entropy loss and accuracy as a performance metric.
