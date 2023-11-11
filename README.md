# Collaborative Research: SCH: Improving Diagnostic Efficiency and Patient Care

## Project Scope:

This project aims to establish a clear path for signed and weighted graph construction from unstructured data and scalable training-free analysis of such graph topology at scale. Unsigned (un)directed models have been extensively studied in the literature [^1^], while heterogeneous graph neural network algorithms are still in their infancy for large real unstructured data applications [^2^]. This project focuses on modeling edges as signed, extended signed, and weighted graphs for fully evolved and static networks. It will propose scalable algorithms and methods for graph analysis and construction. The approaches will be validated on existing social network analysis, recommender system benchmarks, and multi-omics data and electronic health records (EHR) at scale.

## Goal:

The goal is to start with Weight Management Group curation, extend it to HMC data curation and storage in a relational database, and apply methods developed by TXST in-house for improving data representation and collection. The aim is to mitigate algorithmic assumptions on their side that do not hold true for EMHR, focusing on accurate identification of diabetes patients and delineating key factors for successful diabetes management prognostication. Simultaneously, the groundwork for standardized metadata entry for HMC patients at the EMHR will be laid, benefiting future endeavors for patients diagnosed with other diseases.

## Problem Statement:

The primary objective is to enhance the accuracy of rehospitalization prediction, providing evidence-based recommendations that consider long-term consequences. The research seeks to assist healthcare providers and policymakers in resource allocation, effective intervention strategies, and targeted support for high-risk individuals. Bridging the gap between data analysis and actionable insights, the study aims to contribute to improving diabetic patient care, including challenges posed by Long COVID.

Electronic Health Medical Records have a long tail of categorical values, as illustrated in Table 1. The high dimensionality and sparsity of datasets make it extremely challenging to elicit meaningful insights, even with a high number of subjects.

## Proposed Solution:

Our initial data cleaning, integration, and analysis reveal characteristics typical of tabular data from multiple heterogeneous sources. To address challenges posed by unique entry values and complexities of the N3C, this study aggregates and organizes variables relevant to diabetic re-hospitalization. Relevant features and data are used for diabetes management, employing minMaxScaler normalization for uniform feature scaling. Class labeling imbalance is addressed by dividing the dataset into two classes and balancing the sample dataset using under-sampling and stratified sampling. Appropriate encoding methods and aggregation strategies for diabetic data are utilized. Different gradient boosting models, including GBM, XGBoost, LightGBM, and CatBoost, are applied in a comparative study for classification tasks, focusing on hyperparameter optimization techniques. Various classifiers, including Support Vector Classifier, Random Forest Classifier, Gradient Boosting Classifier, XGBoost Classifier, and LightGBM Classifier, are leveraged to predict rehospitalization and ER visit outcomes. A Sequential Model with Dense Layers and ReLU activation functions is introduced, employing Binary Cross-Entropy as the loss function and the Adam optimizer to fine-tune the model using clinical characteristics selected from demographic, drug, condition, observation, procedure, measurement, and device records provided in the N3C. Initial results on the Diabetes Kaggle dataset show progress, with the GBDT model implemented with LightGBM exhibiting higher reliability and accuracy compared to LR, highlighting the potential of machine learning for reliable prediction models in diabetes prevention [^3^]. The next step proposes the utilization of deep learning and GBDT models in tabular data analysis, with the potential to significantly improve patient care and reduce healthcare costs.

Definitions:

1. Diabetes mellitus (DM) is a chronic metabolic disorder characterized by elevated levels of blood sugar, or glucose. It is caused by either the body's inability to produce insulin, the hormone that regulates blood sugar levels, or the body's cells becoming resistant to insulin.
2. Type 1 diabetes is an autoimmune disease in which the body's immune system attacks the beta cells in the pancreas, the cells that produce insulin. This can cause a complete lack of insulin production. Type 1 diabetes is usually diagnosed in children and adolescents, but can develop at any age
3. Type 2 diabetes is the most common type of diabetes. It is caused by a combination of insulin resistance and insufficient insulin production. Insulin resistance occurs when the body's cells do not respond normally to insulin. This can cause blood sugar levels to rise. Type 2 diabetes is usually diagnosed in adults, but can also develop in children and adolescents.
Diabetes can lead to a number of serious health complications, including:

    Heart disease
    Stroke
    High blood pressure
    Nerve damage (neuropathy)
    Eye damage (retinopathy)
    Foot problems
    Kidney disease
    Liver disease
    Alzheimer's disease
    Depression
    Sexual dysfunction

The risk of developing complications from diabetes increases with the length of time you have the disease and how well you control your blood sugar levels.

## References:

[^1^]: Lia Nogueira de Moura and Jelena Tešić. pytwanalysis: Twitter data management and analysis at scale. In 2021 Seventh International Conference on Social Networks Analysis, Management and Security (SNAMS), 2021.

[^2^]: Michelle M Li, Kexin Huang, and Marinka Zitnik. Graph representation learning in biomedicine and healthcare. Nature Biomedical Engineering, 6(12):1353–1369, 2022.

[^3^]: Hiroe Seto, Asuka Oyama, Shuji Kitora, Hiroshi Toki, Ryohei Yamamoto, Juníchi Kotoku, Akihiro Haga, Maki Shinzawa, Miyae Yamakawa, Sakiko Fukui, et al. Gradient boosting decision tree becomes more reliable than logistic regression in predicting probability for diabetes with big data. Scientific Reports, 12(1), 2022.
