# Deep Classification of Cancer Cells

This is an Assessed Coursework for the [Deep Learning](https://www.gla.ac.uk/coursecatalogue/course/?code=COMPSCI5103) postgraduate course at the [University of Glasgow](https://www.gla.ac.uk) during the academic year 2022-2023.

This project was part of a [Kaggle competition](https://www.kaggle.com/competitions/deep-learning-for-msc-2022-23).

## Coursework Specification

The overall goal for this data science coursework is to train two deep neural network which can take a 100x100 pixel images with a cell nuclei in the centre of the image and classify it into one of the following types:
* Normal epithelial cell nuclei with label 0.
* Cancer epithelial cell nuclei with label 1.
* Muscle cell nuclei with label 2.
* Immune leukocyte cell nuclei with label 3.

The overall goal is to develop a deep learning method that can predict the cell type of the images of cell nuclei. You need to develop two models in your notebook:
1. `model1` should be your own small ConvNet with no more than 8 layers total. You should train this from scratch yourself.
2. `model2` should be an existing torchvision model which is pre-trained on ImageNet. You will need to modify this model for your particular task and then train it on the nucleus data – essentially using transfer learning.

For each model you should demonstrate carrying out some suitable hyperparameter optimization using Ray Tune. For each model you should look at producing loss and accuracy curves to assess how your training is working and diagnosing any issues. For each model you should produce a confusion matrix to understand what classes may be getting confused in terms of prediction and try to do something to resolve any confusion. For each model you should try to interpret the model using Captum to understand how it is working.

## Results

`model1`: training accuracy: *99.5%*; validation accuracy: *90.8%*.
`model2`: training accuracy: *99.9%*; validation accuracy: *97.8%*.

**Final test accuracy on Kaggle: 98.1%.**
