# Cifar10
Learning via Trial and Error

 torchvision for loading popular data sets
 torchvision.transforms for performing transformation on the image data
 torch.nn is for defining the neural network
 torch.nn.functional for importing functions like Relu
 torch.optim for implementing optimization algorithms such as Stochastic Gradient Descent (SGD)

-------------------------------------------------------------------------------------------------
 ToTesor() - converts the images from the CIFAT10 dataset made up of PIL images
 into tensors to be used with the torch library

 Normalize(mean, std) the number of parameters we pass into the mean and std arguments
 depends upon the type of image, her we have RGB channels so 3.
 What does 0.5 signify ?
 
------------------------------------------------------------------------------------------
 What is the use of num_workers ?
 when the value of num_workers >0 then it allows Pytorch to switch to perform multi-process data loading
 here we have set the value to 2, which means that there are 2 workers simaltaneously putting putting data into the computers RAM
 This is used to speed up the training process by utilizing machines with multiple cores. By the time the key process for the next batch of samples, the next batch is
 already loaded and ready to go

---------------------------------------------------------------------------------------------------

LOADING THE TEST AND TRAIN DATASET

using torchvision.datasets and CALL the CIFAR10 data . Inside the function I pass multiple arguments and the output to  be the trainset

-> root = './data' creates a folder named data at the root directory
-> transform = transform We pass the previously defined transformation to transform the data as it loaded in

 using torch.utils.data.DataLoader 
 
-------------------------------------------------------------------------------------------------

then I define the classes into a set in Python to gurantee that there are no duplicates

----------------------------------------------------------------------------------------------

BUILDING THE CNN MODEL

![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)




