# Bird-Classification
Bird Classification By Size of Bones
## Project Description
The purpose of this project is to see whether or not we can use PCA along with a decision tree or logistic regression
 to classify birds into ecological groups given their bone dimensions.
### Background Given:
Birds that belong to different ecological groups have different appearances: flying birds have strong wings 
and wading birds have long legs. Their living habits are somewhat reflected in their bones' shapes. 
As data scientists we may think of examining the underlying relationship between sizes of bones and 
ecological groups, and recognising birds' ecological groups by their bones' shapes.

### Methods Used

* PCA
* Data Visualization
* Predictive Modeling
* Decision Tree
* Linear Regression


### Technologies

* Jupyter Notebook
* Python
* Pandas and Numpy
* Scikit-Learn
* Seaborn and Matplotlib

### Data was obtained from:
Kaggle.com; This dataset is provided by Dr. D. Liu of Beijing Museum of Natural History.

Dataset: https://www.kaggle.com/zhangjuefei/birds-bones-and-living-habits


## Project Summary

Data was imported, cleaned, explored, and analyzed. After normalizing and scaling, cluster analysis was determined
 to be maximized at two (instead of the 6 we had anticipated given the classification of ecological types). PCA determined
 that 92% of the variance was explained by the first two components, dropping off significantly after that.
A decision tree was trained and then compared to a logistic regression model. Results using a cross-validation approach
 showed that both the decision tree (0.368) and logistic regression (0.497) had poor performance average scores after PCA.
 
Given the correlation of the features and the overlap of groups via these features, as well as the low dimensionality of the data,
 it is not surprising that we couldn't accurately group these subjects according to their ecologicical niches.

### Variables Used:

    SW: Swimming Birds
     W: Wading Birds
     T: Terrestrial Birds
     R: Raptors
     P: Scansorial Birds
    SO: Singing Birds
	
      huml, humw: Length and Diameter of Humerus
    ulnal, ulnaw: Length and Diameter of Ulna
      feml, femw: Length and Diameter of Femur
      tibl, tibw: Length and Diameter of Tibiotarsus
      tarl, tarw: Length and Diameter of Tarsometatarsus
