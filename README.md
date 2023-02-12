# Number-Recognition-using-Naive-Bayes

### Dataset Description
The given dataset is like the MNIST dataset. It consists of four files: trainingimages, traininglabels, validationimages, and validationlabels. The files trainingimges and validaionimages consist of a digit illustrated by characters '+' and '#'. 

### Goal
We aim to recognize the digit using the Naive Bayes algorithm and compare our estimation with the actual value of the digit and then find the model's accuracy.

### Naïve Bayes Classifier Algorithm

* Naive Bayes algorithm is a supervised learning algorithm, which is based on the Bayes theorem and used for solving classification problems.
* It is mainly used in text classification that includes a high-dimensional training dataset.
* Naïve Bayes Classifier is one of the simple and most effective Classification algorithms which helps in building fast machine learning models that can make quick predictions.
* It is a probabilistic classifier, which means it predicts on the basis of the probability of an object.
* Some popular examples of the Naive Bayes Algorithm are spam filtration, Sentimental analysis, and classifying articles.

### Bayes' Theorem
* Bayes' theorem is also known as Bayes' Rule or Bayes' law, which is used to determine the probability of a hypothesis with prior knowledge. It depends on the conditional probability.
* The formula for Bayes' theorem is given as:

![image](https://user-images.githubusercontent.com/125180530/218305218-7c23b093-a73b-4508-8ab9-10bba49fd029.png)

Where,

* P(A|B) is Posterior probability: Probability of hypothesis A on the observed event B.

* P(B|A) is Likelihood probability: Probability of the evidence given that the probability of a hypothesis is true.

* P(A) is Prior Probability: Probability of hypothesis before observing the evidence.

* P(B) is Marginal Probability: Probability of Evidence.

### Feature Extraction

For designing the classifier we use the following features:

![image](https://user-images.githubusercontent.com/125180530/218305359-8ced0e97-cf0c-4c06-a8bc-4bdd078d6211.png)
![image](https://user-images.githubusercontent.com/125180530/218305376-cd2cf823-e5f2-4f9c-8814-b35d126915f8.png)

### Implementing the algorithm
For implementing the Naive Bayes algorithm we should follow the below formula:

![image](https://user-images.githubusercontent.com/125180530/218305487-231408e4-6287-48d0-bf5e-479fcfdc7625.png)

Because the probability P(x) in all cases is the same, we can conclude the last equation. If we assume that the distribution of the features is all Gaussian, then we can say:

![image](https://user-images.githubusercontent.com/125180530/218306088-922a6936-273e-4fed-aa38-b7581f2f7713.png)

After calculating mean and variance for each of the ten classes, we can conclude:


So, for all the classes we should calculate the above equation, and then among the calculated probabilities we should choose the class which has the maximum probability. Finally, I implement a function for accuracy calculation and report the accuracy of the implemented model.
