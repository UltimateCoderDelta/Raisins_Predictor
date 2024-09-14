Raisins Type Classifier 
=======================

Project's Purpose
-----------------

This project is designed to test the effectiveness of two different classifiers with the primary goal of \
ensuring no model overfitting or underfitting occurs; in certain instances when designing machine learning\
algorithms, models may become too dependent on training data, which in turn causes said models to perform \
remarkably well on data it has seen before, with an unfortunate inverse result occuring with new (test) data.\
Therefore, as a means of ensuring the classifier in this project is capable of detecting the correct raisin type,\
of which there are two, namely: Kecimen and Besni, the dataset is tested with the following classifiers for accuracy\
comparison purposes:

1. DecisionTreeClassifier
   
   This classifier is used in tandem with GridSearchCV; GridSearchCV can be used to improve a model's accuracy\
   due to its "k-fold" processing capabilities, which ensures that all of our training data is placed within our\
   test data at least once; the the higher the value of k, the better the final outcome can be. Furthermore, by \
   making use of different hyperparameters, GridSearchCV will aid us in finding the optimal model parameters for our classification \
   purposes!

2. LogisticRegression with RandomizedGridCV

   This classifier is used with RandomizedGridCV, which works in a similar manner, with the only difference being\
   the process used for the tuning of hyperparameters (for LogisticRegression these are alpha and/or C). Hyperparameters \
   in this case are randomized, as opposed to being statically established.  

**NOTE:** Machine learning algorithms can only work accurately with numeric data. Therefore, the class/target categories for this dataset\
  of Kecimen and Besni have been converted to the following binary alternatives:

0. Kecimen
1. Besni

Libraries and Technologies Used
-----------

To ensure the following project runs successfully, there are a plethora of Python-based development environments\
out there; the preferred choice for this project is _Jupyter Notebook_.

To successfully run or replicate this project locally, please ensure the following libraries are installed:

- Python Pandas (install via bash)

  ```
  pip install pandas
  
  ```

- Python NumPy (install via bash)

  ```
  pip install numpy

  ```

- Scikit-Lean library

  ```
  pip install -U scikit-learn
  ```


Sources Used
-----------
UCI Machine Learning repository: https://archive.ics.uci.edu/dataset/850/raisin

**Acknowledgements**
CINAR I., KOKLU M. and TASDEMIR S., (2020), Classification of Raisin Grains Using Machine Vision and Artificial Intelligence Methods. Gazi Journal of Engineering Sciences, vol. 6, no. 3, pp. 200-209, December, 2020. 

Code License
------------
MIT License

Copyright (c) [2024] [Yvar Joseph]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


