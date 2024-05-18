# Multitask_Learning_on_MultiEMNIST_using_MGDA-UB

This project applies Multi-Task Learning on the MultiMNIST dataset using a U-NET architecture. The loss calculation is performed using the Multiple Gradient Descent Algorithm – Upper Bound (MGDA-UB).

# Overview


Multi-Task Learning (MTL) aims to improve the performance of multiple tasks by learning them jointly. In this project, we use the MultiMNIST dataset, a variant of the MNIST dataset where each image contains multiple handwritten digits. The U-NET architecture, typically used for image segmentation tasks, is employed to handle the multi-task nature of the problem. The MGDA-UB approach is used to balance the gradients from different tasks during training, ensuring that the model does not prioritize one task at the expense of others.

# Dataset


The MultiMNIST dataset is used in this project. You can download the dataset from Kaggle.

# Downloading the Dataset


Visit the Kaggle dataset page.
Click on the "Download" button to download the dataset files.
Extract the downloaded files to a directory of your choice.
Architecture
We use the U-NET architecture for this project. U-NET is an encoder-decoder network typically used for image segmentation. It is well-suited for our multi-task learning scenario where each task corresponds to the segmentation of a digit in the image.

# Loss Calculation


The loss is calculated using the Multiple Gradient Descent Algorithm – Upper Bound (MGDA-UB). This approach ensures balanced learning across multiple tasks by considering the gradient norms of each task. The combined gradient norm (MGDA-UB) is used to guide the optimization process.

# Code Structure


Data Preparation: We prepare the data using TensorFlow's tf.data.Dataset API. The data is batched for efficient processing.
U-NET Model: We define the U-NET model architecture. The U-NET consists of an encoder path, a bottleneck, and a decoder path.
MGDA-UB Loss Function: We implement the MGDA-UB loss function to compute the gradient norms for each task and combine them.
Training the Model: We train the model using the U-NET architecture and the MGDA-UB loss function.
# Results


The results of the training process will be displayed and evaluated using various metrics appropriate for multi-task learning.

# How to Run


Download the dataset from the provided link.
Prepare the dataset and place it in the appropriate directory.
Run the training script to start the training process.
Conclusion
This project demonstrates the application of multi-task learning on the MultiMNIST dataset using a U-NET architecture and MGDA-UB for loss calculation. This approach ensures balanced learning across multiple tasks, leveraging the strengths of both the U-NET architecture and the MGDA-UB method.

# Acknowledgements


The MultiMNIST dataset was obtained from Kaggle.
The U-NET architecture is inspired by the original paper by Olaf Ronneberger et al.
License
This project is licensed under the MIT License - see the LICENSE file for details.






