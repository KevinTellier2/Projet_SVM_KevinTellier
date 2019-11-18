# <strong>Support Vector Machine - Project</strong>

&nbsp;


<p style="text-align:justify";>This project has been made by Caroline ROBLIN, Maxime YE and Kevin TELLIER, students at the <a href="https://www.univ-orleans.fr/deg/masters/ESA/" title="ESA Master"> ESA Master</a>'s degree, for the Big Data Analytics : Support Vector Machine course, instructed by <a href="https://sites.google.com/view/christophe-hurlin/home?authuser=0" title="Christophe Hurlin">Christophe Hurlin</a>.</p>

<p style="text-align:justify";>The datasets we used in this project are FREE and disponible <a href="https://www.kaggle.com/mlg-ulb/creditcardfraud" title="here">here</a>.</p>

&nbsp;

### <strong>Content</strong>

<p style="text-align:justify";>The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.</p> 

<p style="text-align:justify";>It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, ... V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.</p>

&nbsp;

### <strong>Implementation procedure</strong>

Internally, we used about 15 libraries and a mostly package to manage all the calculations, the package 'mlr'.

&nbsp;

#### <strong>References</strong>


For a description of the implementation and details of the algorithms used, please refer to : 

- <a href="https://cran.r-project.org/web/packages/mlr/mlr.pdf" title="MLR : A library for Machine Learning in R">MLR : A library for Machine Learning in R</a>

&nbsp;

### <strong>Benefits and limitations of the SVM</strong>

- Benefits :

  * <p style="text-align:justify";>It handles non-parametric cases : the RBF kernel SVM is considered as non-parametric learning algorithm since the number of  parameters grows with the size of the training set. In the RBF kernel of the SVM, we construct the kernel matrix by computing the pairwise distances between the training points, so it's non-parametric.</p> 

  * Ability to process a high number of variables. 

  * The choice of penalty C allows flexibility and resistance to overfitting.

&nbsp;

- Limitations :

  * <p style="text-align:justify";>The processing time is generally longer than other Machine Learning methods, especially with the increase in the number of observations.</p> 
  * <p style="text-align:justify";>Difficulty identifying the right parameter values and hypersensitivity of penalization parameters.</p>
  * <p style="text-align:justify";>There is no explicit model for non-linear kernels, hence the use of support points. It is also difficult to visualize the support when the number of variables becomes high.</p>
