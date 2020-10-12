# Music-Genre-Classification
The digital shift in the distribution of music has
presented the need for effective automated classification of large
volumes of music into various categories. In this project automatic
music genre classification is tackled by first identifying and
extracting representative aspects of a music piece. Subsequently
music features are tested for their significance in the task of
genre classification using mutual information gain in order to
make the feature vector compact, comprehensive and efficient.
After several off-the-shelve classifiers were used, Support Vector
Machines with a radial basis function kernel turned out to be
the best performing model achieving an accuracy of 80.80% in
classifying music pieces into 1 of 10 genres in GTZAN. A detailed write up
can be found in the report pdf.

## Notebooks
- data_preparation.ipynb (creates a csv file that will be used to access audio and initial labelling)
- low_level_feature_extraction.ipynb (extracts low level features from audio files, featured detailed in report)
- model_fitting.ipynb (fits the different models and fine tuning of model parameters)
- model analysis (evaluation of models accuracy, precision and confusion matrices)

## Models and Accuracy
- Support Vector Machines (80.80 %)
- Multilayer Perceptron (77.30 %)
- Logistic regression (75.80 %)
- Random Forests (72.40 %)
- k Nearest Neighbours (69.70)
- Naive Bayes (54.50 %)

## Feature Selelction
Classification accuracy with different number of significant features, there is a cut off point indicated by red vertical line in which a number of features can be dropped without having significant impact on classification accuracy. The graph was generated using support vector machines.

![Alt text](https://github.com/phantom820/Music-Genre-Classification/blob/master/images/graph.png)

## Confusion Matrices
### Support Vector Machine
![Alt text](https://github.com/phantom820/Music-Genre-Classification/blob/master/images/svm.png)

### Multilayer Perceptron
![Alt text](https://github.com/phantom820/Music-Genre-Classification/blob/master/images/mlp.png)
