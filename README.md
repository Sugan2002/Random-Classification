### EX NO: 01
### DATE: 01.04.2022
# <p align="center"> RANDOM CLASSIFICATION</p>
## AIM:
To write a python program to perform random classification.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## Related Theoritical Concept:

Random classifier:
It creates a set of decision trees from randomly selected subset of training set. It then aggregates the votes from different decision trees to decide the final class of the test object. Random Forest is suitable for situations when we have a large dataset, and interpretability is not a major concern.

Purpose of Random classifier:
One of the most important features of the Random Forest Algorithm is that it can handle the data set containing continuous variables as in the case of regression and categorical variables as in the case of classification.

## Algorithm

Step 1 − First, start with the selection of random samples from a given dataset.

Step 2 − Next, this algorithm will construct a decision tree for every sample. Then it will get the prediction result from every decision tree.

Step 3 − In this step, voting will be performed for every predicted result.

Step 4 − At last, select the most voted prediction result as the final prediction result.

## Program:
```python
/*
Program to implement random classification.
Developed by   :  P.SUGANYA
RegisterNumber :  212220230049
*/

import matplotlib.pyplot as plt
from sklearn import datasets
X,y = datasets.make_blobs(n_samples=100,n_features=2,centers=2,
                               cluster_std=1.05,random_state=2)

fig=plt.figure(figsize=(10,8))
plt.plot(X[:,0][y==0], X[:,1][y==0],'rs')
plt.plot(X[:,0][y==1], X[:,1][y==1],'go')
plt.xlabel("Feature 1")
plt.ylabel("Feaure 2")
plt.title("Random Classification Data with 2 classes")

```

## Output:
![output](./static/img/expO1NN.PNG)

## Result:
Thus, the random classifier was successfully implemented using python programming.
