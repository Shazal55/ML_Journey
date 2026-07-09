# 🌸 K-Nearest Neighbors (KNN) from Scratch on the Iris Dataset

This project implements the **K-Nearest Neighbors (KNN)** classification algorithm from scratch using **NumPy** and **Matplotlib**. The objective of this project is to understand the inner workings of KNN instead of relying on machine learning libraries such as Scikit-learn.

## Project Objective

The goal of this project is to learn:

* How the KNN algorithm works internally.
* How Euclidean distance is calculated.
* How nearest neighbors are selected.
* How majority voting determines the predicted class.
* Why feature standardization is important.
* How to visualize the KNN prediction process.

## Dataset

The project uses the **Iris Dataset** downloaded from Kaggle.

The dataset contains **150 flower samples** belonging to three species:

* Iris Setosa
* Iris Versicolor
* Iris Virginica

Each sample contains four features:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

## Workflow

The complete workflow followed in this project is:

1. Load the dataset using Pandas.
2. Convert species names into numerical labels.
3. Separate features (`X`) and labels (`Y`).
4. Remove the `Id` column.
5. Standardize all features using NumPy.
6. Shuffle the dataset.
7. Split the data into training and testing sets (80% / 20%).
8. Implement Euclidean Distance from scratch.
9. Find the K nearest neighbors.
10. Perform majority voting.
11. Predict the class of unseen samples.
12. Calculate model accuracy.
13. Visualize the nearest neighbors using Matplotlib.

## Euclidean Distance

The distance between two samples is calculated using:

[
d = \sqrt{\sum_{i=1}^{n}(x_i-y_i)^2}
]

where `n` is the number of features.

## Visualization

The project includes visualizations for:

* Training data
* Test sample
* K nearest neighbors
* Distance connections between the test sample and its neighbors

These plots help in understanding how KNN makes predictions.

## Result

Model Accuracy:

**96.67%**

The implementation was completed without using Scikit-learn's `KNeighborsClassifier`.

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Jupyter Notebook

## What I Learned

Through this project, I learned:

* Feature preprocessing and standardization
* Train-test splitting without external libraries
* Euclidean distance calculation
* Neighbor selection using `np.argsort()`
* Majority voting with `np.bincount()`
* Building a machine learning algorithm from scratch
* Visualizing the KNN decision-making process

## Future Improvements

* Add support for different distance metrics (Manhattan, Minkowski, etc.).
* Compare results with Scikit-learn's KNN implementation.
* Visualize decision boundaries.
* Experiment with different values of `k`.
* Build a reusable KNN class with `fit()` and `predict()` methods.

---

This project was created as a learning exercise to understand the mathematics and implementation of the K-Nearest Neighbors algorithm from first principles.
