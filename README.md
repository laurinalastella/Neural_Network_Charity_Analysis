# Neural_Network_Charity_Analysis
### Module 19
### Laurina LaStella
### October 2022
---
---


# Overview of the analysis:
With machine learning and neural networks, create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

---
---

# Results:

## Data Preprocessing
### What variable(s) are considered the target(s) for your model?
- IS_SUCCESSFUL

### What variable(s) are considered to be the features for your model?
- Objects
- - APPLICATION_TYPE
- - AFFILIATION
- - CLASSIFICATION
- - USE_CASE
- - ORGANIZATION
- - INCOME_AMT
- - SPECIAL_CONSIDERATIONS
- Integers
- - STATUS (Dropped in Optimization 3)
- - ASK_AMT

### What variable(s) are neither targets nor features, and should be removed from the input data?
- EIN
- NAME

---

### Compiling, Training, and Evaluating the Model

## Optimization 1
- First hidden layer: 5
- - Activation: Relu
- Second hidden layer: 5
- - Activation: Relu
- Epochs: 50
- Loss: 0.5703
- Accuracy: 0.7261

## Optimization 2
- First hidden layer: 8
- - Activation: Tanh
- Second hidden layer: 8
- - Activation: Tanh
- Epochs: 80
- Loss: 0.5529
- Accuracy: 0.7273

## Optimization 3
- Additional column "STATUS" filtered to = 1 ("Active") then dropped.
- First hidden layer: 12
- - Activation: Relu
- Second hidden layer: 6
- - Activation: Tanh
- Epochs: 100
- Loss: 0.6827
- Accuracy: 0.57307

---
---

# Summary:

The more complicated I made it, the lower the accuracy became. I don't understand the nuances of these models well enough to know how to recommend anything.
---
---

