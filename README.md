# EVA 5 - Session 5
## Step 1
Target:
Set-up the file by importing all the required libraries.
Create the train and test transforms.
Loading the MNIST dataset and setting up the data loader.
Calculate some statistics related to the data and vizualize how the data actually looks like.
Setup a working model; nothing fancy.
Results:
Parameters: 194,884
Best Training Accuracy: 99.54%
Best Test Accuracy: 99.11%
Analysis:
The model is very heavy (too many parameters) for this problem.
From the graph, we can observe that the model is over-fitting.
## Step 2
Target:
To make the model lighter by reducing the total number of parameters.
Reduce the total number of epochs to 14.
Results:
Parameters: 8,488
Best Training Accuracy: 98.90%
Best Test Accuracy: 98.57%
Analysis:
This model is good and can be modified further to improve accuracies.
The model is not over-fitting.
## Step 3
Target:
Addition of Batch-norm to improve the models efficiency.
Addition of Dropout to the layers.
Results:
Parameters: 8,664
Best Training Accuracy: 99.57%
Best Test Accuracy: 99.24%
Analysis:
The model has been regularized.
The overall accuracy of the model has increased. However, we still have not achieved the desired accuracy. Further modification is required.
## Step 4
Target:
Addition of Image Augmentation (Random Rotation).
Addition of GAP (Global Average Pooling) layer to the network.
Addition of scheduler.
Results:
Parameters: 9,608
Best Training Accuracy: 99.25%
Best Test Accuracy: 99.48%
Analysis:
The model has achieved accuracies greater than 99.4% consistently towards the end.
Less than 10k parameters were used for this model.
The model is not over-fitting (Train and Test accuracies are close to each other).
