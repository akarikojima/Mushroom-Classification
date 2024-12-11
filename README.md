jup![](UTA-DataScience-Logo.png)

# Mushroom Classification Machine Learning

* This repository holds an attempt to apply a Decision Tree Classifier to mushroom features using data from
"Mushroom Classification" Kaggle challenge (https://www.kaggle.com/datasets/uciml/mushroom-classification/data). 

## Overview

  * **Challenge:** The task, as defined by the Kaggle challenge is to use categorical features from 23 different species of gilled mushrooms to predict the edibility of a given mushroom.
  * **Approach:** The approach in this repository formulates the problem as a classification task, using deep recurrent neural networks, where one-hot encoding is applied to the categorical features to convert them into numerical format. The transformed features are used as input for the model, and the performance of Decision Tree Classifier used to predict mushroom edibility (e.g. edible or poisonous).
  * **Summary:** The Decision Tree Classifier was able to predict the edibility of mushrooms with 100% accuracy.

### Data

  * Type: Categorical
    * Input: Mushrooms characteristics
  * Size: 8124 rows, 23 features, CSV file: 365.2 KB
  * Instances (Train, Test, Validation Split): 4784 characteristics for training, 1625 for testing, 1625 for validation

#### Preprocessing / Clean up

![image](https://github.com/user-attachments/assets/5f9c2dcd-8a0c-4084-b47d-0801dc0657e0)
* In the feature, 'stalk-root', there were unknown values.
  * These were converted to characteristics depending on the frequency of the class
* The features, 'gill-attachment' and 'veil-type', were dropped due to their irrelevancy

#### Data Visualization

![image](https://github.com/user-attachments/assets/9c3abd8c-1f4e-4f03-aeea-bb89692d5edf)
![image](https://github.com/user-attachments/assets/15bac698-b851-4365-94a9-a31706f83ce9)

There were various features that were great to be used to train the algorithm just as seen in the figures above. There were clear differences between the frequencies of bruises and odor depending on their edibility.

### Problem Formulation

* Define:
  * Input: Mushroom Characteristics / Output: Predicted edibility
  * Models
    * Decision Tree Classifier: Handles categorical and numerical values and efficient and fast
    
### Training

* Decision Tree Classifier with default parameters

### Conclusions

![image](https://github.com/user-attachments/assets/c7ccacd4-f89d-4dcd-87ce-2a3d3564559c)

* The algorithm was able to predict the edibility of the mushroom 100% of the time. 

## How to reproduce results

* Convert the '?' values in the feature 'stalk-root' into the characteristics with the highest frequency depending on the classes
* Split the features into separate characteristics and hot encode the categorical values into numerical
* Set the target as 'class'
* Run a Decision Tree Classifier algorithm
* 
### Overview of files in repository

* Follow the Mushroom_classfication.ipynb file.

### Software Setup
* Used modules:
  * pandas as pd
  * numpy as np
  * seaborn as sns
  * matplotlib.pyplot as pltList
  * sklearn.model_selection import train_test_split
  * sklearn.tree import DecisionTreeClassifier
  * sklearn.metrics import accuracy_score




