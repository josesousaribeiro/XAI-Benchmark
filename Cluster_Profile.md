

## Description of dataset properties by cluster

Seeking to better understand the characteristic of each dataset cluster found from its 15 properties analyzed, this research performed initial analyzes by inspecting the value ranges of each of the properties in each cluster (Figure 1), as well as performing analysis through Multiple Correspondence Analysis – MCA in order to identify which dataset property values best characterized each cluster found.

To identify each different dataset profile, an inspection of the value ranges of each cluster for each property was carried out. In this analysis, the possible existence of specific property values for datasets of specific clusters was verified. At this stage, it was identified that the quantity of datasets in cluster 2 had a small $n$ and, therefore, this cluster was disregarded from these results (The datasets for this cluster are: \textit{kr-vs-kp, Phishing Web sites,} and \textit{SPECT}). Keeping only clusters 0 and 1.

Through inspection analysis, it was possible to verify different distributions of property value ranges for each of the two main clusters. The result is shown in Figure 1.

![alt text](https://github.com/josesousaribeiro/XAI-Benchmark/blob/main/Figures/full_properties_by_cluster_in_frame_.png)
**Figure 1 - Dataset properties for each cluster.**

Each inspection analysis found on each property in Figure 1 is listed below.

**1 - AutoCorrelation:** Existence of datasets with high values of autocorrelations in cluster 0 than in cluster 1. 

**2 - NumberOfInstances:** It is clear that this property did not present relevant differences in values for the two clusters.

**3 - Dimensionality:** It is clear that this property did not present relevant differences in values for the two clusters.

**4 - PercentageOfBinaryFeatures:** Cluster 0 has a high number of datasets with few binary variables, different from cluster 1 datasets. 

**5 - StdvNominalAttribute:** The datasets present in cluster 1 present fixed values for this property, that is, they are more uniform in this perspective.

**6 - MeanNominalAttDistinctValues:** The datasets present in cluster 1 present fixed values for this property, that is, they are more uniform in this perspective.

**7 - ClassEntropy:** It perceives the existence of a high number of datasets with high class entropy values ​​in cluster 1, that is, the existence of higher levels of information in these datasets.

**8 - NumberOfFeatures:** Existence of a greater number of datasets with smaller quantitative of attributes in cluster 1 than in cluster 0.

**9 - NumberofNumericFeatures:** Existence of a greater number of datasets with smaller amounts of numerical attributes in cluster 1 than in cluster 0.

**10 - NumberOfSymbolicFeatures:** The datasets of cluster 0 present concentrated values ​​of this property.

**11 - NumberOfBinaryFeatures:** The datasets of cluster 0 present concentrated values ​​of this property.

**12 - PercentageOfSymbolicFeatures:** Most of the datasets in cluster 0 have the lowest percentages of symbolic attributes.

**13 - PercentageOfNumericFeatures:** Most of the datasets in cluster 0 have high percentages of numerical attributes.

**14 - MajorityClassPercentage:** Most of the datasets present in cluster 0 have high imbalances between classes.

**15 - MinorityClassPercentage:** Most of the datasets present in cluster 0 have high imbalances between classes.


From the above, it can be inferred that cluster 0 has datasets with greater complexity than the datasets present in cluster 1. However, aiming to consolidate this finding, an MCA was performed in order to identify which properties each dataset cluster has higher ratio.

Note, to perform this analysis the [dataset with values of each of the 15 properties](https://github.com/josesousaribeiro/XAI-Benchmark/blob/main/Openml/df_dataset_properties.csv) of the datasets had to be converted to [a new binary dataset](https://github.com/josesousaribeiro/XAI-Benchmark/blob/main/Openml/df_properties_binarized.csv). With this, each value of the 15 properties were replaced by 'h' (equal to or above the mean of attribute values) and 's' (below the mean of attribute values), according to the literature itself. It should be noted that the attributes: 'StdvNominalAttDistinctValues', 'MeanNominalAttDistinctValues', 'NumberOfSymbolicFeatures', and 'NumberOfBinaryFeatures' were the only non-binarized attributes due to their insignificant variance in new dataset.

A summary of the relationships found through MCA can be seen in Figure 2.

![alt text](https://github.com/josesousaribeiro/XAI-Benchmark/blob/main/Figures/mca_dataset_properties.png)
**Figure 2 - Multiple Correspondence Analysis - MCA with rows (datasets) and columns (properties) depending on the first and second PCA components.**

In Figure 2, the existence of the three clusters identified in the research can be clearly seen (remembering that cluster 2 was discarded due to the small number of datasets).

In the MCA shown in Figure 2,by inspection, it is notable the relationship (shorter distances) of high quantity of datasets in cluster 0 with values above average (symbol h) for properties (bigger circles) such as _MajorityClassPercentage, Dimensionality, NumberOfInstances, NumberOfFeatures, PercentageOfNumericFeatures_ and _AutoCorrelation_. As well, it is also noticed a relation of high quantity of datasets of cluster 0 with values below the average (symbol s) for properties such as _ClassEntropy, PercentageOfSymbolicFeatures_ and _PercentageOfBinaryFeatures_.

Also with regard to the MCA shown in Figure 2, by inspection, it is possible to assess the existence of a relationship (shorter distances) of high quantity of datasets in cluster 1 with values above the average (symbol h) for properties (bigger circles) such as ClassEntropy, PercentageOfSymbolocFeatures, PercentageOfBinaryFeatures, NumberOfBinaryFeatures and MinorityClassPercentage. It is also possible to identify a relation of high quantity of datasets in cluster 1 with values below average (symbol s) for properties sush as _AutoCorrelation,NumberOfFeatures, PercentageOfNumericFeatures, NumberOfNumericFeatures, NumberOfInstances, Dimensionality,_ and _MajorityClassPercentage._

Note, some properties were not mentioned above because they appear at very close distances for the two dataset clusters.

**However, from the inspection of MCA's results, it is concluded that cluster 0 is formed by significant amount of datasets with greater complexities, whereas cluster 1 is formed by significant amount of datasets with minors complexities.**

