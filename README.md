# Neural-Network-to-Classify-Handwritten-Digits
A Neural Network implementation, designed from scratch, to classify the MNIST Database of Handwritten Numbers

# Description
This is an implementation of a Neural Network Deep Learning Model, (designed from the groud up, without using existing libraries) to identify and classify Handwritten digits from the MNIST Dataset.

This particular implementation is based on the multi-layer perceptron (MLP, just another term for fully connected feedforward networks), which is shown as following. It is designed for a K-class classification problem.

![](images/MLP_diagram.png)

# MLP Definitions
Let  (x∈ℝD,y∈{1,2,⋯,K})  be a labeled instance, such an MLP performs the following computations:

![](images/MLP_description.png)

For a  K -class classification problem, one popular loss function for training (i.e., to learn  W(1) ,  W(2) ,  b(1) ,  b(2) ) is the cross-entropy loss. Specifically we denote the cross-entropy loss with respect to the training example  (x,y)  by  l :

![](images/cross_entropy_loss.png)

Note that one should look at  l  as a function of the parameters of the network, that is,  W(1),b(1),W(2)  and  b(2) . For ease of notation, let us define the one-hot (i.e., 1-of- K ) encoding of a class  y  as:

![](images/onehotencoder_1.png)

so that

![](images/onehotencoder_2.png)

We can then perform error-backpropagation, a way to compute partial derivatives (or gradients) w.r.t the parameters of a neural network, and use gradient-based optimization to learn the parameters.

# Model Performance

    *** At epoch 1 ***
    Training loss at epoch 1 is 479.4455301319439
    Training accuracy at epoch 1 is 0.8496
    Validation accuracy at epoch 1 is 0.874
    
    *** At epoch 2 ***
    Training loss at epoch 2 is 358.9095593325671
    Training accuracy at epoch 2 is 0.8932
    Validation accuracy at epoch 2 is 0.909
    
    *** At epoch 3 ***
    Training loss at epoch 3 is 306.4451982897476
    Training accuracy at epoch 3 is 0.9106
    Validation accuracy at epoch 3 is 0.915
    
    *** At epoch 4 ***
    Training loss at epoch 4 is 264.1638585148052
    Training accuracy at epoch 4 is 0.9256
    Validation accuracy at epoch 4 is 0.919
    
    *** At epoch 5 ***
    Training loss at epoch 5 is 250.87838492388042
    Training accuracy at epoch 5 is 0.9248
    Validation accuracy at epoch 5 is 0.918
    
    *** At epoch 6 ***
    Training loss at epoch 6 is 228.51312766305165
    Training accuracy at epoch 6 is 0.9342
    Validation accuracy at epoch 6 is 0.92
    
    *** At epoch 7 ***
    Training loss at epoch 7 is 206.9570664226602
    Training accuracy at epoch 7 is 0.9444
    Validation accuracy at epoch 7 is 0.922
    
    *** At epoch 8 ***
    Training loss at epoch 8 is 194.84799192940756
    Training accuracy at epoch 8 is 0.9446
    Validation accuracy at epoch 8 is 0.927
    
    *** At epoch 9 ***
    Training loss at epoch 9 is 177.9126169745046
    Training accuracy at epoch 9 is 0.9556
    Validation accuracy at epoch 9 is 0.927
    
    *** At epoch 10 ***
    Training loss at epoch 10 is 170.2862888707467
    Training accuracy at epoch 10 is 0.954
    Validation accuracy at epoch 10 is 0.934
