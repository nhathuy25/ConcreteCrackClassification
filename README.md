# Concrete Crack Detection in Buildings
### H.N.Huy NGUYEN

This project is a part of the final assignment of the specialization that I'm currently pursuing called [**IBM AI Engineering** on Coursera]("https://www.coursera.org/professional-certificates/ai-engineer").

The project is about training a Deep Neural Network using pretrained model <code>resnet18</code> and a dataset of 40000 images of concrete samples with labels.

The aim is to understand the basic concepts of training and evaluating a Deep Neural Network, how to set up parameters for a simple Neural network like
<ul>
  <li>Choosing criterion, here I used <i>Cross entropy loss function</i></li>
  <li>Organize and annotate data samples for training dataset and validation dataset</li>
  <li>Choosing optimizer for the model</li>
  <li>Train the model, define the number of <code>epoch</code> and <code>batch size</code> for each training/validation loader</li>
  <li>Evaluate the trained model and find the misclassfiied examples</li>
</ul>

### Training process
For the training process, we use a training dataset of 30,000 annotated examples, changing the output layer of the pre-trained model for binary classification, the training epoch is 1 and for the mini-batch size of 100, the training process took 300 iterations to complete. The training time is approximately 37 mins.

![alt text](https://github.com/nhathuy25/ConcreteCrackClassification/blob/main/imgs/loss_by_iteration.png)


### Misclassified samples
Example of some misclassified samples, the trained model has 99.86% accuracy on the validation loader, here are some examples of the misclassfied ones:
![alt text](https://github.com/nhathuy25/ConcreteCrackClassification/blob/main/imgs/misclassifed_samples.png)
