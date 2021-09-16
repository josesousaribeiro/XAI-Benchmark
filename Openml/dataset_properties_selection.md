

## Description of dataset properties by cluster

Seeking a better understanding of how the 15 properties characterize each of the clusters. 15 graphs were created, which allow a clear understanding of how value ranges of different properties are presented in each of the clusters in quantitative terms, Figure 1.

![alt text](https://github.com/josesousaribeiro/XAI-Benchmark/blob/main/Openml/full_properties_by_cluster_in_frame.png)
**Figure 1 - Frame with all properties plots.**

**- AutoCorrelation:** Selected, even with the intersection of existing densities, there are important differences to be considered in the range of values ​​of the x axis.

**- NumberOfInstances:** Not selected, because the two densities have very similar characteristics in both clusters. Since, they have the same range of values ​​in x.

**- Dimensionality:** Not selected, because the two densities have very similar characteristics in both clusters. Since, they have the same range of values ​​in x.

**- PercentageOfBinaryFeatures:** Not selected, because this property is calculated based on a percentage dependent on more than one other properties (such as number of attributes and number of binary attributes).

**- StdvNominalAttribute:** Not selected, as they have density values ​​centered in the same range of x values.

**- MeanNominalAttDistinctValues:** Not selected, because they present density values ​​centered in the same range of values ​​in x.

**- ClassEntropy:** Selected, even with the intersection of existing densities, there are important differences to be considered in the range of values ​​of the x axis.

**- NumberOfFeatures:** Selected, even with the intersection of existing densities, there are important differences to be considered in the range of values ​​of the x axis.

**- NumberofNumericFeatures:** Not selected, as it is almost directly proportional to the NumberOfFeatures property.

**- NumberOfSymbolicFeatures:** Not selected, as they have density values ​​centered on the same range of x values.

**- NumberOfBinaryFeatures:** Not selected, as they have density values ​​centered on a similar range of x values.

**- PercentageOfSymbolicFeatures:** Not selected, because this property is calculated based on a percentage dependent on more than one other properties (such as number of attributes and number of symbolic attributes).

**- PercentageOfNumericFeatures:** Not selected, because this property is calculated based on a percentage dependent on more than one other property (such as number of attributes and number of numerical attributes).

**- MajorityClassPercentage:** Selected, due to important differences in value ranges unique to each cluster, observed on the x-axis.

**- MinorityClassPercentage:** Not selected, as it is inversely proportional to MajorityClassPercentage.


