# Project Part 3: Deep Learning with CNN

In this part, we will perform the classification task, using a convolutional neural network. The dataset is the CIFAR- 10 dataset. We will experiment with a convolutional neural network with the following parameter settings:

- The input size is the size of the image ( 32 x 32 x3).
- _First layer_ – Convolution layer with 32 kernels of size 3x3. It is followed by ReLU activation layer and batch normalization layer.
- _Second layer_ – Convolution layer with 32 kernels of size 3x3. It is followed by ReLU activation layer and batch normalization layer.
- _Third layer_ – Max pooling layer with 2x2 kernel.
- _Fourth layer_ – Dropout layer with 0.2 probability of setting a node to 0 during training.
- _Fifth layer_ – Convolution layer with 64 kernels of size 3x3. It is followed by ReLU activation layer and batch normalization layer.
- _Sixth layer_ – Convolution layer with 64 kernels of size 3x3. It is followed by ReLU activation layer and batch normalization layer.
- _Seventh layer_ – Max pooling layer with 2x2 kernel.
- _Eighth layer_ – Dropout layer with 0.3 probability of setting a node to 0 during training.
- _Ninth layer_ – Convolution layer with 128 kernels of size 3x3. It is followed by ReLU activation layer and batch normalization layer.
- _Tenth layer_ – Convolution layer with 128 kernels of size 3x3. It is followed by ReLU activation layer and batch normalization layer.
- _Eleventh layer_ – Max pooling layer with 2x2 kernel.
- _Twelfth layer_ – Dropout layer with 0.4 probability of setting a node to 0 during training.
- _Last layer_ – Fully connected layer with 10 nodes (corresponding to the 10 classes) and SoftMax activation function.

The padding for the layers is set as ‘same’ which means zero padding is added to keep the output
dimensions same as input for the layer.

We will train such a network with the training set and then test it on the testing set.

You will be given the baseline code. You are required to experiment with the code by changing some of
the hyper-parameters according to the following code and then report the test accuracy for each of them.

**Algorithm:** Convolutional Neural Network

**Resources:** CIFAR- 10 dataset, Google CoLab

**Workspace:** Google CoLab

**Language** : Python

Your specific tasks:


1. Get familiar with the Google CoLab platform.
2. Run the baseline code (provided in baseline.ipynb file) and report the test accuracy.
3. Change the following settings and report the test accuracy:
    a. Change learning rate to – i) 0. 05 ii) 0.00 01
    b. Change kernel size for first convolutional layer to 7 x 7
    c. Change optimizer to RMSProp
    d. Remove all the batch normalization layers in the network
    e. Change all dropout values (units to drop) - i) 0.
    f. Change batch size – i) 16 ii) 256

**Note:** Change in the parameters is meaningful to assist your understanding of the behavior/performance of the network. For each of the combinations mentioned above, you must explain what you think is the effect of change in the setting on the test accuracy (e.g., one or two sentences description).

**What to submit:**

1. Your code for the above steps.
2. A report summarizing the results with the following format-
    a. Introduction – start with problem statement, data description etc.
    b. Method – your understanding of using this svm package, steps followed
    c. Results and observation – the results asked in each of the steps like test accuracy (any
       intermediate results you want to show) along with your observations
    d. Conclusion
Note: There is no minimum or maximum length requirement for the report. Writing the
report is the opportunity for you to reflect on your understanding of the problems/tasks through
organizing your results.
3. The report should be typed ( _handwritten reports are not allowed_ ) and in a .pdf format (to be
    submitted as separate document, not included within the code file).
4. Do not submit a .zip file. Submit multiple individual files on Canvas instead.

**Code**

The code execution is available in the [`CSE 569 Project 3.ipynb`](./CSE%20569%20Project%203.ipynb) file.