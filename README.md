
# Teen-Marketing-Classification-using-Kmeans-and-PCA

#### Problem Statement
 
The many millions of teenage consumers using social networking 
sites have attracted the attention of marketers struggling to 
find an edge in an increasingly competitive market. One way to 
gain this edge is to identify segments of teenagers who share 
similar tastes, so that clients can avoid targeting advertisements 
to teens with no interest in the product being sold. 

Build K-means clustering model to classify the interest of 
teenagers by using various attributes. 

## Data Analysis

#### Data Description 

The SNS dataset contains 30000 observations (rows) each represents
 a high school student and 40 features (columns) that provides 
 information for the student. 
*  Gradyear: Graduation year of the student (2006, 2007, 2008, 2009) 
* Gender: Gender of the student (male, female) 
* Age: Age of the student 
* Friends: No of friends

For clustering, 36 words were chosen to represent five categories 
of interests: namely extracurricular activities, fashion, 
religion, romance, and antisocial behaviour. The 36 words include 
terms such as football, sexy, kissed, bible, shopping, death, and 
drugs. The final dataset indicates, for each person, how many 
times each word appeared in the person’s SNS profile. 

## Approach

Our Main goal is to know that whether which check whether person 
belongs to extracurricular activities, fashion, religion, 
romance, and antisocial behaviour .

* Data Exploration : Exploring dataset using pandas, numpy, 
  matplotlib and seaborn.
* Data visualization :Ploted graphs to get insights about 
  independed variables.
* Model Selection I : Tested best k-value using elbow method or 
  the given k-value in problem statement.
* Post Data visualization : Plot graph of clusters and centroids.
* Pickle File : Selected model as per best K-value and created
  pickle file using pickle library.

## Technologies Used

* Jupyter notebook, Spyder, VScode Is Used For IDE.
* For Visualization Of The Plots Matplotlib , Seaborn Are Used.
* Git Hub Is Used As A Version Control System.
* os is used for creating and deleting folders.
* csv is used for creating .csv format file.
* numpy is for arrays computations and mathematical operations
* pandas is for Manipulation and wrangling structured data
* scikit-learn is used for machine learning tool kit
* pickle is used for saving model
## Conclusion

We developed K-Means Clusterring model which is capable to predict
whether the teen belong to which category. In this dataset 40 features
 and 30000 records.

* Our 1st step is to import dataset and check all
  the details like shape, info(), describe() for getting better knowledge
  about data or each variable.

* 2nd step is to checking missing value and datatype of missing variable
  by looking at info(). after that we have to delete those 
  variable whose missing value is more than 50% of data. Other 
  variable should be treat as repect to their datatype

* 3rd step After handling all this we have to do data 
  visualization for getting some insight for eg. we have to check 
  for ouliers, imbalanced variable or imbalanced data so we have to 
  remove ouliers or do upsampling for those. In this there is no 
  need to treat oulier so after doing visualization we can say 
  that maximum people who died is from class 3 and count of 
  male died is more as compared to female.

* 4th step is to do Preprocessing using labelencoder and perform 
  StandardScalar for scaling data

* 6th step is find k-value from elbow point method or we have to 
  use that k-value which is mention in problem statement

* 6th We have to plot graph of all the data points and and centroids
  belongs to. or we can wse PCA(Principal Component Analysis) and then we plot.

* Last step is model Deployment using Flask Framework.
  For model deployment we have to dump our model using pickle library
  and can save our model in .pkl or .sav extension.
