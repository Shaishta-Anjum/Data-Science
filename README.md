# Data Science Lab Programs

This repository contains various data science programs written in Python. Each program demonstrates different concepts and techniques used in data science, such as data visualization, clustering, classification, and more. Below are the descriptions and potential viva questions for each program.

## Program 1: Effect of Hours Studied on Exam Score

### Explanation and Working

This program visualizes the relationship between the number of hours studied and the scores achieved on an exam using a line chart. It starts by creating lists of hours studied and corresponding scores. The `plot` function from the `matplotlib.pyplot` library is used to create a line chart with markers indicating each data point. The chart is then enhanced by adding labels to the x and y axes, as well as a title. Finally, the plot is displayed with a grid to improve readability.

### Potential Viva Questions and Answers

1. **What is the purpose of the `marker` parameter in the `plot` function?**
   - The `marker` parameter is used to specify the shape of the data points on the plot. In this program, the marker is set to `'*'` which represents a star-shaped marker.

2. **How do you add labels and a title to a plot in Matplotlib?**
   - You can add labels to the x and y axes using `plt.xlabel('label')` and `plt.ylabel('label')` respectively. The title can be added using `plt.title('title')`.

3. **What does the `grid` function do in Matplotlib?**
   - The `grid` function adds a grid to the plot, making it easier to visualize and interpret the data points relative to the axes.

## Program 2: Histogram of Miles per Gallon (mpg)

### Explanation and Working

This program loads the `mtcars` dataset and plots a histogram of the miles per gallon (mpg) values. The dataset is read from a CSV file into a Pandas DataFrame. The `hist` function from `matplotlib.pyplot` is used to plot the histogram, which shows the distribution of `mpg` values across different ranges. The histogram is customized by specifying the number of bins, the color of the bars, and the color of the edges. Labels and a title are added to the plot for clarity.

### Potential Viva Questions and Answers

1. **How do you load a CSV file into a Pandas DataFrame?**
   - You can load a CSV file into a Pandas DataFrame using the `pd.read_csv('file_path')` function.

2. **What is a histogram and what information does it provide?**
   - A histogram is a graphical representation of the distribution of numerical data. It shows the frequency of data points within specified ranges (bins).

3. **How do you customize the appearance of a histogram in Matplotlib?**
   - You can customize a histogram by specifying parameters such as `bins` for the number of bins, `color` for the bar color, and `edgecolor` for the color of the bar edges.

## Program 3: Cleaning the BL-Flickr-Images-Book Dataset

### Explanation and Working

This program cleans the `BL-Flickr-Images-Book.csv` dataset by removing irrelevant columns, setting the index, and tidying up fields. The dataset is loaded into a Pandas DataFrame, and columns that are not relevant for the analysis are dropped. The `Identifier` column is set as the index for better data management. The `Date of Publication` column is cleaned using a regular expression to extract the year, and the `Place of Publication` column is tidied up using NumPy operations to standardize the location names.

### Potential Viva Questions and Answers

1. **How do you drop columns from a DataFrame in Pandas?**
   - You can drop columns using the `drop` method, e.g., `df.drop(columns=['col1', 'col2'], inplace=True)`.

2. **What is the purpose of setting an index in a DataFrame?**
   - Setting an index helps in uniquely identifying rows and can be used to improve data retrieval and management.

3. **How can you use regular expressions to clean data in Pandas?**
   - Regular expressions can be used with the `str.extract` method to extract specific patterns from text data, e.g., extracting the year from a date string.

## Program 4: Logistic Regression on the Iris Dataset

### Explanation and Working

This program performs logistic regression on the Iris dataset using a pipeline that includes standard scaling and regularization. The Iris dataset is loaded and split into training and testing sets. A pipeline is created using `StandardScaler` for feature scaling and `LogisticRegression` for the classification model. The pipeline is then trained on the training data and evaluated on the testing data. The accuracy of the model is printed to assess its performance.

### Potential Viva Questions and Answers

1. **What is the purpose of using a pipeline in scikit-learn?**
   - A pipeline allows for the sequential application of multiple data processing steps, making it easier to manage and replicate preprocessing and modeling steps.

2. **How does logistic regression work?**
   - Logistic regression is a statistical method for binary classification that models the probability of a binary outcome based on one or more predictor variables.

3. **What is the role of the `StandardScaler` in the pipeline?**
   - `StandardScaler` standardizes the features by removing the mean and scaling to unit variance, which is important for many machine learning algorithms.

## Program 5: Clustering with K-means and Hierarchical Clustering

### Explanation and Working

This program performs clustering on a dataset using K-means and hierarchical clustering methods, and evaluates the clustering performance using the adjusted Rand Index. The dataset is loaded and visualized to show the true clusters. K-means clustering and hierarchical clustering (single-link and complete-link) are applied to the data. The adjusted Rand Index is calculated to measure the similarity between the predicted clusters and the true clusters. The results are printed and compared to determine the best clustering method.

### Potential Viva Questions and Answers

1. **What is K-means clustering and how does it work?**
   - K-means clustering partitions the data into K clusters by minimizing the within-cluster variance. It iteratively assigns data points to the nearest cluster centroid and updates the centroids.

2. **What is hierarchical clustering and how does it differ from K-means?**
   - Hierarchical clustering builds a hierarchy of clusters using either agglomerative (bottom-up) or divisive (top-down) approaches. Unlike K-means, it does not require the number of clusters to be specified in advance.

3. **What is the adjusted Rand Index and how is it different from the Rand Index?**
   - The adjusted Rand Index measures the similarity between two clustering results, adjusted for the chance grouping of elements. It ranges from -1 to 1, with higher values indicating better clustering.

## Program 6: Decision Tree Classifier

### Explanation and Working

This program creates a decision tree classifier using a custom dataset, trains it, calculates its accuracy, and visualizes the decision tree. The dataset is created and converted into a DataFrame, with categorical variables converted into numerical ones using one-hot encoding. The data is split into training and testing sets, and a decision tree classifier is trained on the training data. The model's accuracy is calculated on the testing data. The decision tree is visualized using Graphviz to show the decision rules.

### Potential Viva Questions and Answers

1. **What is a decision tree and how does it work?**
   - A decision tree is a model that splits the data into branches based on feature values, leading to a decision (classification or regression) at the leaves. It uses conditions on feature values to partition the data.

2. **How do you handle categorical variables in a dataset?**
   - Categorical variables can be handled using one-hot encoding, which converts categorical values into binary vectors.

3. **What is one-hot encoding and why is it used?**
   - One-hot encoding transforms categorical variables into a binary matrix, with each category represented by a column. It is used to allow machine learning models to interpret categorical data.

## Program 7: Clustering with K-means and Agglomerative Clustering

### Explanation and Working

This program performs clustering on a spiral dataset using K-means and agglomerative clustering, and evaluates the performance using the adjusted Rand Index. The dataset is loaded and visualized to show the true clusters. K-means clustering and agglomerative clustering (single-link and complete-link) are performed on the data. The adjusted Rand Index is calculated to assess the clustering performance by comparing the predicted clusters with the true clusters. The results are printed for comparison.

### Potential Viva Questions and Answers

1. **What is the difference between K-means and agglomerative clustering?**
   - K-means partitions data into K clusters by minimizing within-cluster variance, while agglomerative clustering builds a hierarchy of clusters by merging the closest pairs of clusters.

2. **How do you evaluate the performance of clustering algorithms?**
   - The performance of clustering algorithms can be evaluated using metrics like the adjusted Rand Index, which measures the similarity between the predicted clusters and the true clusters.

3. **What is the adjusted Rand Index and how is it different from the Rand Index?**
   - The adjusted Rand Index adjusts the Rand Index for chance grouping, providing a more accurate measure of cluster similarity. It ranges from -1 to 1, with 1 indicating perfect agreement.
