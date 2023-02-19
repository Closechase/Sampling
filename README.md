# Sampling
Assignment on Sampling for UCS654


## Sampling Technique Description and Sampling Size Formula
1. Simple Random Sampling
A simple random sample is a subset of a statistical population in which each member of the subset has an equal probability of being chosen.

n = (z^2*(p)*(1-p))/e^2
Z = 1.96 (for 95% confidence)
p = 0.5
E = 0.03 (assumed 3%)
n = 1067

2. Stratified Sampling
Stratified sampling is a method of sampling that involves the division of a population into smaller subgroups known as strata.

n = (z^2*(p)*(1-p))/(e/s)^2
Z = 1.96 (for 95% confidence)
p = 0.5
E = 0.07 (assumed 7%)
S = 2
n = 784 (392 for each class)

3. Systematic Sampling
Systematic sampling is a probability sampling method where we select members of the population at a regular interval.
Samples taken on every 5th interval

4. Cluster Sampling
Cluster sampling is a probability sampling method in which we divide a population into clusters and then randomly select some of these clusters as sample.

>Rows per Cluster = 20
>
>Number of Clusters = 28 (sqrt(n/2) where n is the total number of rows)

5. Multi-Stage Sampling
In this method we have used a combination of sampling technique, i.e. cluster and simple random. The dataset is divided into clusters and then random samples are chosen from those clusters.


## Final Result Table
|                        | Simple Random | Stratified | Systematic | Cluster | Multi-Satge |
| ---------------------- | ------------- | ---------- | ---------- | ------- | ----------- |
| Logistic Regression    |91.01          |91.32       |79.22       |91.30    |94.00        |
| Decision Tree          |99.62          |96.42       |92.20       |95.65    |92.00        |
| Support Vector Machine |69.66          |63.26       |70.12       |72.17    |70.00        |
| Gaussian Naive Bayes   |76.02          |75.00       |77.92       |66.95    |58.00        |
| Random Forest          |100.00         |100.0       |100.00      |100.0    |100.00       |

## Conclusion
In this case we can clearly see that regardless of the sampling method use, Random Forest classifier gives the highest accuracy of 100%

___

## Author
Aayush Asrey
102003745
