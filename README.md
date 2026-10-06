# ML_Final_Project

Unsupervised machine learning analysis and clustering with K-means and PCA on the Seeds dataset.

<br>

#### Problem Statement  
A cooperative business has received deliveries of mixed wheat grain, of which its varieties are unlabelled. Some basic measurements of each kernel are known, which the model uses to predict the number of varieties in the mixed deliveries and depict its separability.

#### Data Set  
The data set, the Seeds dataset, contains a total of seven measurements describing the structure of 210 kernels of the delivery. The included variables such as area, perimeter, compactness, etc. all focus on the structure of the kernels and their physical properties, which are the parameters needed for their sorting.

#### Method(s)  
The variables are preprocessed through feature scaling and dimensionality reduction (PCA). Our main clustering model is KMeans, with the Elbow method and the Silhouette analysis also used as decisive tools. Finally, we used cross-tabulation, purity score and plots for validation.

#### Results  
Among the results, we conclude that PCA captured a total of 71.8%+17,1% of the total variance of the set, resulting in 3 groups. The model returns a purity score of 91.9% which indicates a mostly sucessful prediction. Through cross tabulation we can conclude the varieties; variety 1 is represented by cluster 2, variety 2 is represented by cluster 1 and variety 3 is represented by cluster 0. With inverse feature transform we also access the physical profile of each variety.

#### Interpretation  
The results showed a total of 3 groups. with the model recovering majority of the variety of the kernel structure. Due to the use of PCA and the discrepancy of the Elbow and the Silhouette methods, it's reasonable to assume that the results do not accurately reflect reality. It is useful for predictions, but its results should not be used without further validation as that could result in miscategorization of the seeds.

#### Reflection  
Reflecting back, the model achieved a high accuracy in its predictions, separating the seeds with minimal mistakes. Difficulties were also present, especially since the number of clusters could not be concluded through pure math and human judgement was required. As such, if I had more time I would try other clustering algorithms too to see if they agree with the results and try other dimensionality reduction methods such as t-SNE.

(Special thanks to the instructors and the LEAP program for guiding this project)
