# xai_benchmark

This repository has research analysis data for Explainable Artificial Intelligence - XAI.

The research group responsible for this study is composed of:

José Ribeiro - site: https://sites.google.com/view/jose-sousa-ribeiro

Raíssa Silva - site: https://sites.google.com/site/silvarailors

Lucas Cardoso - site: http://lattes.cnpq.br/9591352011725008

Ronnie Alves (Leader) - site: https://sites.google.com/site/alvesrco/

**Abstract**

Strategies based on Explainable Artificial Intelligence - XAI have emerged in computing to promote a better understanding of predictions made by black box models. Most XAI-based measures used today explain these types of models, generating attribute rankings aimed at explaining the same, that is, the analysis of Attribute Importance of Model. There is no consensus on which XAI measure generates an overall explainability rank. For this reason, several proposals for tools have emerged (Ciu, Dalex, Eli5, Lofo, Shap and Skater). An experimental benchmark of explainable AI techniques capable of producing global explainability ranks based on tabular data related to different problems and ensemble models are presented herein. Seeking to answer questions such as "Are the explanations generated by the different measures the same, similar or different?" and "How does data complexity play along model explainability?." The results from the construction of 82 computational models and 592 ranks shed some light on the other side of the problem of explainability: dataset complexity!

**Proposal**

This research raises discussions for the current moment in the XAI area through two main questions: --- Considering the current tools aimed at explaining black box machine learning models, it can be inferred that they generate global rankings of same, similar, or different explainabilities? --- Following the same idea as in the previous question, are the generations of equal, similar, or different explainabilities related to specific properties of a dataset?

Seeking to answer the two hypotheses presented above, this research emerges as a comparative analysis of different XAI metrics, capable of producing model-agnostic global explainability ranks based on tabular data related to different problems.

**Benchmark**

In the benchmark proposed by this research, the explanatory ranks of 6 different XAI metrics (Ciu, Dalex, Eli5, Lofo, Shap and Skater) are compared using Spearman coefficients, resulting in conclusive results.

The methodology is presented in the diagram below:

![alt text](https://github.com/josesousaribeiro/xai_benchmark/blob/main/General_Info/metodologia_1.png)

All the information needed for a better understanding and reproducibility of the procedures performed in the research can be accessed directly on the notebook (Google Colab) available at root, as well as in the files folders.






