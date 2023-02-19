# Sampling_102003161
# Comparing Sampling Techniques for 5 Machine Learning Models

## Introduction

This project explores the effectiveness of different sampling techniques for creating a balanced dataset for a machine learning model. The dataset used is initially unbalanced, so random over-sampling and under-sampling techniques are used to create a balanced dataset. Five different sampling techniques are then applied to this balanced dataset, and the accuracies of the resulting samples are compared using five different machine learning models.

## Sampling Techniques

The following five sampling techniques were used in this project:

1. **Simple Random Sampling:** A basic sampling technique where each data point in the dataset has an equal probability of being selected in the sample.

2. **Stratified Sampling:** A sampling technique where the population is divided into subgroups (strata) based on a specific characteristic, and samples are taken from each stratum in proportion to the population.

3. **Systematic Sampling:** A sampling technique where every nth element in the population is selected for the sample, with n being a fixed interval.

4. **Cluster Sampling:** A sampling technique where the population is divided into clusters, and a sample of clusters is randomly selected. Then, all members of the selected clusters are included in the sample.

5. **Convenience Sampling:** A non-probability sampling technique where the sample is chosen based on its convenience to the researcher.

## Comparison Table

The table below shows the accuracies of each sampling technique on five different machine learning models. The dataset used for all models is a balanced version of the original unbalanced dataset using random over-sampling and under-sampling techniques.

| Sampling Technique | Ada Boost Classifier | Decision Tree Classifier | Linear Discriminant Analysis | Ridge | K Neighbors Classifier |
|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|
| Simple Random Sampling | 0.9813 | 0.9778 | 0.8805 | 0.8581 | 0.8951 |
| Systematic Sampling | 0.9944 | 0.9813 | 0.9158 | 0.8878 | 0.9493 |
| Stratified Sampling | 0.9907 | 0.9851 | 0.8791 | 0.8696 | 0.9498 |
| Cluster Sampling | **0.9999** | 0.9868 | 0.8971 | 0.8809 | 0.9691 |
| Convenience Sampling | 0.9887 | 0.9849 | 0.8833 | 0.8739 | 0.9623 |

Based on these results, it can be concluded that Cluster Sampling performs the best on all five models. Simple random sampling performs the worst on all five models. The other sampling techniques have varying performance depending on the model. The model which gives the best accuracy for all 5 samples is Decision Tree.

## Conclusion

It is recommended to use cluster sampling for this dataset, as it consistently gives the best performance across all models. However, other sampling techniques may be worth considering for different datasets or models.
 
