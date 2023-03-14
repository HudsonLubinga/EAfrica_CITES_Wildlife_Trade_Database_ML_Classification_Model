# Machine Learning Classification Model for Identifying Wildlife Species in East Africa

# By Hudson Nandere Lubinga / Francis Lowu Xavier

### Dataset
We collected a comprehensive and accurate dataset of taxonomic features and other characteristics of wildlife species obtained from East African countries between 2018 and 2021 from CITES Wildlife Trade Database (https://www.kaggle.com/datasets/cites/cites-wildlife-trade-database)

## General OVerview:
The decline in global biodiversity is a pressing concern due to human activities, leading to millions of species at risk of extinction.
East Africa is especially affected by habitat destruction, poaching, and climate change, resulting in significant losses in wildlife
populations. Machine learning (ML) has demonstrated potential in identifying species, especially in camera trap images, acoustic
recordings, and genetic data. However, there is a need to further explore the use of ML in identifying wildlife species in East Africa.
To address this need, we developed ML classification models to identify wildlife species in East Africa. Our dataset included
taxonomic features and characteristics of wildlife species from East African countries between 2018 and 2021. We used the random
forest algorithm, which is suitable for complex datasets with multiple features. Our evaluation achieved an accuracy of 63.4% and
a baseline score of 8.02%, showing the potential of our models in identifying wildlife species in East Africa. Our study could
contribute to wildlife conservation by detecting and preventing illegal wildlife trade activities, monitoring population trends,
assessing the impact of human activities on different species in East Africa, and preserving biodiversity.

## Discussion of Findings:
The machine learning-based classification models developed in this study aim to identify wildlife species in East
Africa with implications for conservation and management. The dataset used for this study was collected from CITES
Wildlife Trade Database, which contained comprehensive and accurate information on the taxonomic features and
other characteristics of wildlife species obtained from East African countries between 2018 and 2021.

Data pre-processing steps were performed to prepare the dataset for analysis, including dropping irrelevant columns,
filling missing values, and encoding categorical variables into numerical variables. The most important features for
identifying wildlife species were identified by using the corr() function and creating a heatmap of the correlations
between each feature and the target variable. 

The top 5 features with the highest absolute correlation coefficients were
selected, and a new dataset with the selected features and the target variable was created. Based on our dataset and
research topic, we selected the Random Forest algorithm for developing the classification model. We split the dataset
into training and testing sets and trained the random forest classifier on the training set. We evaluated the performance
of the model on the testing set and obtained an accuracy of 0.63, indicating that the model correctly predicts the
wildlife species around 63% of the time. While an accuracy of 0.63 is reasonable, we should keep in mind that accuracy
alone may not be the best metric to evaluate the performance of a classification model. Especially when the dataset is
imbalanced or the misclassification of certain classes is more costly than others, other metrics such as precision, recall,
F1 score, and confusion matrix must be considered. In our case, we have multiple classes of wildlife species, and the
distribution of the classes might not be balanced.

We used the precision score as a performance metric. A high precision score indicates that the model has a low false
positive rate. In our case, the precision score of 0.5659 indicates that out of all the positive predictions made by the
model, 56.6% were true positive predictions. This means that the model has moderate accuracy in identifying the
correct wildlife species in East Africa. We used the weighted averaging method to calculate the precision score
because we have multiple classes in our target variable, and the weighted method calculates a precision score for each
class and then takes the weighted average based on the number of samples in each class. 

Furthermore, we analyzed the confusion matrix to gain insights into the performance of our model. The confusion matrix revealed that the model
was particularly good at predicting wildlife species in the "Reptilia" and "Insecta" classes, achieving a precision score
of 0.93 and 0.77, respectively. However, the model struggled to predict the "Aves" and "Mammalia" classes, achieving
a precision score of 0.45 and 0.53, respectively. This could be due to class imbalance or a lack of sufficient features
to distinguish between these classes.

More so, the baseline score was 8.02%. It is great that our model accuracy was much better than the baseline score.
To interpret these scores, the baseline score represents the accuracy achieved by a naive model that simply predicts
the most frequent class for all instances in the dataset. Therefore, any model with an accuracy score above the baseline
is considered to be useful. In our case, the model accuracy of 0.6337 means that the model is correctly predicting the
target variable around 63.37% of the time.

## 
