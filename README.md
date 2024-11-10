# Microarray-brain-tumor-diagnostics

## Part 1
In this project, we introduce exploratory data analysis and multiclass classification on microarray data regarding brain tumors. Microarray data experiments monitor gene expression in different tissues. The experiment is equipped with an additional response variable such as a cancer type. In this dataset, we have 5 different tumor types in the response variable - class. Furthermore, the number of measured genes is more than 5 thousand. It is assumed that only a few marker components of this gene subset determine the type of tissue. The identification of these significant groups is crucial for tumor classification in medical diagnostics, as well as for understanding how the genome as a whole works.

Accordingly, before exploratory data analysis, we performed feature selection to focus only on the most meaningful features for the whole dataset. The feature selection procedure and its stability will be described in the following part of the project. In the analysis, we took into account various aspects of the data like distribution in classes, different statistics, discriminative ability of each feature, correlation between chosen genes, data visualization, etc. Based on the knowledge that we gained in this part, we could move to the classification problem.

In the classification part, we took into account various classification algorithms: K Nearest Neighbors, Linear and Quadratic Discriminant Analysis, Multinomial Logistic Regression, Decision Tree and Random Forest. Since we faced a problem of a large number of features and a very small number of observations (p ≫ n), we incorporated a feature selection procedure into our model selection pipeline. We performed leave-one-out cross-validation on the algorithms to extract the best parameters for our models. Finally, we compared our models with chosen parameters based on misclassification errors and macro-averaged F1 score. We also investigated their stability using box plots. At the end, we suggested further research directions that might improve our work.

The main research problem is the evaluation of the chosen feature selection method based on the comparison of models’ results with feature selection and with randomly chosen features. Another important problem is the selection of the best model for our research, investigating the stability of the feature selection procedure, and the stability of chosen models. This study might yield a better diagnostic method, where doctors might get suggestions on tumor type from the model.

## Part 2
In this phase of our research, we continue with further exploration of the brain tumor microarray dataset, which comprises data related to five distinct types of brain tumors. Notably, this dataset is characterized by its large number of features in oposition to a very limited number of observations. In this part, we investigate the application of selected dimensionality reduction techniques — PCA (Principal Component Analysis) and MDS (Multidimensional Scaling). We aim to visualize the outcomes of these methods. Subsequently, we integrate them into our classification assessment and contrast the results with the previous phase where feature selection was involved instead of dimensionality reduction.

In our classification analysis, we consider a range of algorithms, including K Nearest Neighbors, Linear and Quadratic Discriminant Analysis, Multinomial Logistic Regression, Decision Tree, and Random Forest. For each algorithm, we perform parameter tuning utilizing leave-one-out cross-validation. We then compare our models, optimized with chosen parameters, based on misclassification errors and macro-averaged F1 score.

Moving forward, we transition to cluster analysis with a focus on quality assessment. Here, we compare the outcomes of approaches involving dimensionality reduction and unsupervised feature selection using the medoids from PAM (Partitioning Around Medoids) algorithm. We evaluate the per- formance of selected partitioning and hierarchical methods, namely KMeans, PAM, DIANA, and AGNES.

Additionally, we offer suggestions for further research directions that could enhance our findings. Our primary research objectives revolve around comparing feature selection with dimensionality reduction in the context of classification results. We also aim to uncover underlying patterns within our dataset through cluster analysis and compare the effectiveness of clustering with dimensionality reduction and unsupervised feature selection methods. Furthermore, we explore whether the results of our cluster analysis align with predefined classes. Our research potentially leads to improved diagnostic methods that provide tumor type suggestions based on various classification and clustering approaches. This study holds promise for aiding medical professionals in making more informed decisions regarding tumor diagnosis and treatment.

The project consists of:
- two Rnw files (knitr, R) with the whole reports,
- two pdf versions of reports.


Authors:
- [Joanna Matuszak](https://github.com/vsiv00)
- Joanna Wojciechowicz
