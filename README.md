## Building a decision tree classifier and putting on PyPi

#### Overview
The purpose of this project is getting familiar with putting self-built tool on PyPi.

#### PyPi Project Page
This is the PyPi project [page](https://pypi.org/project/playground-decision-tree/)

#### Project Description
Built a decision tree classifier from sratch using gini index as split criterion. 

Please using `pip install playground-decision-tree` to install the package from PyPi.

Below is an example of using the package

```
from playground_decision_tree import DecisionTreeClassifier
from sklearn.datasets import load_iris

dataset = load_iris()
X, y = dataset.data, dataset.target

clf = DecisionTreeClassifier(max_depth=5)

# fit
clf.fit(X, y)

# predict
print(clf.predict([[5.1, 3.5, 1.4, 0.2]]))

```


