# Deep-Learning-Project

Company Name: CodeTech It Solutions

Name : Prem M

Domain : Data Science

Duration : 4 Weeks

Intern ID : CTIS6711

Desprition of the task:

This Python script presents a complete and practical example of training a neural network for image classification using modern deep learning tools such as PyTorch and torchvision. The main objective of the program is to train a model that can accurately recognize handwritten digits from the widely used MNIST dataset, which is a standard benchmark in the field of computer vision.

The script begins by importing essential libraries. PyTorch is used for defining and training the neural network, while torchvision simplifies working with image datasets and transformations. Matplotlib is included for visualizing the training performance. A transformation is defined using transforms.ToTensor(), which converts input images into tensor format and scales pixel values to a range between 0 and 1. This normalization step is important because neural networks perform better when input data is standardized.

Next, the MNIST dataset is loaded. It contains thousands of grayscale images of handwritten digits, each with a resolution of 28×28 pixels. By setting train=True, the script uses the training portion of the dataset, and the download=True argument ensures that the dataset is automatically fetched if not already available. A data loader is then created to divide the dataset into smaller batches of 64 images. This batching process improves computational efficiency and allows the model to learn more effectively. Shuffling is enabled to ensure that the data is presented in a random order during training, which helps prevent the model from learning unintended patterns.

The neural network model is defined using nn.Sequential, which provides a simple way to stack layers. The first layer, Flatten, converts each 2D image into a one-dimensional vector of size 784 (28×28). This is followed by a fully connected layer with 128 neurons, which learns important features from the input data. A ReLU activation function is applied to introduce non-linearity, enabling the model to capture complex patterns. Finally, another linear layer maps the features to 10 output classes, representing the digits from 0 to 9.

To train the model, a loss function and optimizer are specified. The CrossEntropyLoss function is suitable for multi-class classification tasks, as it compares the predicted class probabilities with the actual labels. The Adam optimizer is used to update the model’s parameters efficiently, with a learning rate of 0.001.

The training process runs for three epochs. In each epoch, the model processes all batches of data. For each batch, gradients are reset, predictions are generated, and the loss is calculated. Backpropagation is then performed to compute gradients, and the optimizer updates the model weights. The total loss for each epoch is accumulated and stored in a list, allowing progress tracking. The loss is printed after each epoch to monitor improvement.


After training, the script visualizes the loss values using Matplotlib. A line graph is plotted to show how the loss decreases over epochs, indicating that the model is learning effectively. Overall, this script provides a clear and structured introduction to neural network training, covering data preparation, model design, optimization, and performance evaluation.

output of the task :

<img width="1160" height="847" alt="Image" src="https://github.com/user-attachments/assets/3adda0bc-fea5-4715-9476-0dc32b9a04eb" />
