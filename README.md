![](UTA-DataScience-Logo.png)

# Mushroom Classification Machine Learning

* **One Sentence Summary** This repository holds an attempt to apply a Decision Tree Classifier to mushroom features using data from
"Mushroom Classification" Kaggle challenge (https://www.kaggle.com/datasets/uciml/mushroom-classification/data). 

## Overview

  * **Challenge:** The task, as defined by the Kaggle challenge is to use categorical features from 23 different species of gilled mushrooms to predict the edibility of a given mushroom.
  * **Approach:** The approach in this repository formulates the problem as a classification task, using deep recurrent neural networks, where one-hot encoding is applied to the categorical features to convert them into numerical format. The transformed features are used as input for the model, and the performance of Decision Tree Classifier used to predict mushroom edibility (e.g. edible or poisonous).
  * **Summary:** The Decision Tree Classifier was able to predict the edibility of mushrooms with 100% accuracy.

### Data

  * Type: Categorical
    * Input: Mushrooms characteristics, CSV file: characteristics -> edibility
  * Size: 8124 rows, 23 features, CSV file: 365.2 KB
  * Instances (Train, Test, Validation Split): 4784 characteristics for training, 1625 for testing, 1625 for validation

#### Preprocessing / Clean up

* In the feature, 'stalk-root', there were unknown values.
  * These were converted to characteristics depending on the frequency of the class
* The features, 'gill-attachment' and 'veil-type', were dropped due to their irrelevancy

#### Data Visualization

![image](https://github.com/user-attachments/assets/9c3abd8c-1f4e-4f03-aeea-bb89692d5edf)
![image](https://github.com/user-attachments/assets/15bac698-b851-4365-94a9-a31706f83ce9)

There were various features that were great to be used to train the algorithm just as seen in the figures above. There were clear differences between the frequencies of bruises and odor depending on their edibility.

### Problem Formulation

* Define:
  * Input: Mushroom Characteristics / Predicted edibility
  * Models
    * Decision Tree Classifier: Handles categorical and numerical values and efficient and fast
    * 
### Training

* Describe the training:
  * How you trained: software and hardware.
  * How did training take.
  * Training curves (loss vs epoch for test/train).
  * How did you decide to stop training.
  * Any difficulties? How did you resolve them?

### Performance Comparison

* Clearly define the key performance metric(s).
* Show/compare results in one table.
* Show one (or few) visualization(s) of results, for example ROC curves.

### Conclusions

* State any conclusions you can infer from your work. Example: LSTM work better than GRU.

### Future Work

* What would be the next thing that you would try.
* What are some other studies that can be done starting from here.

## How to reproduce results

* In this section, provide instructions at least one of the following:
   * Reproduce your results fully, including training.
   * Apply this package to other data. For example, how to use the model you trained.
   * Use this package to perform their own study.
* Also describe what resources to use for this package, if appropirate. For example, point them to Collab and TPUs.

### Overview of files in repository

* Describe the directory structure, if any.
* List all relavent files and describe their role in the package.
* An example:
  * utils.py: various functions that are used in cleaning and visualizing data.
  * preprocess.ipynb: Takes input data in CSV and writes out data frame after cleanup.
  * visualization.ipynb: Creates various visualizations of the data.
  * models.py: Contains functions that build the various models.
  * training-model-1.ipynb: Trains the first model and saves model during training.
  * training-model-2.ipynb: Trains the second model and saves model during training.
  * training-model-3.ipynb: Trains the third model and saves model during training.
  * performance.ipynb: loads multiple trained models and compares results.
  * inference.ipynb: loads a trained model and applies it to test data to create kaggle submission.

* Note that all of these notebooks should contain enough text for someone to understand what is happening.

### Software Setup
* List all of the required packages.
* If not standard, provide or point to instruction for installing the packages.
* Describe how to install your package.

### Data

* Point to where they can download the data.
* Lead them through preprocessing steps, if necessary.

### Training

* Describe how to train the model

#### Performance Evaluation

* Describe how to run the performance evaluation.


## Citations

* Provide any references.







