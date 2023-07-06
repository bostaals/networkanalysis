# PREDICTING POSITIVE AND NEGATIVE TIES IN SIGNED NETWORKS
## A Comparative Study on Wikipedia Adminship and School Friendship Networks

Bo Staals
06 July 2023

### Abstract

Network analysis is a growing area of research in various fields. While most existing studies focus on unsigned networks, this research explores the coexistence of positive and negative ties in signed online and real world networks. By combining topological features and social theories, this research investigates the gap in previous research. This leads to the following research question: "*To what extent can machine learning models predict positive and negative ties in online and real world networks?*" 

The network analysis is carried out on two signed networks. The Wikipedia network represents the online network, where every user is allowed to vote for other users that request for adminship. The school network represents the real world network and is based on data collected in the "Children of Immigrants Longitudinal Survey in Four European Countries" project. The final datasets used for the classification model contain 4627 nodes and 122767 ties for the Wikipedia network and 4284 nodes and 27333 ties for the school network.

Snowball sampling has been performed to obtain subsets of the networks due to computational bottlenecks. The final feature set includes every connection between nodes, which can be either negative, not observed or positive. It also includes important metrics such as node-level, network-level, similarity-based, social theory and path-based metrics. After model selection, hyperparameter tuning and feature selection on the subsets, the final datasets are evaluated on the tuned Light Gradient Boosting Machine model. 

The results show that the school network outperforms the Wikipedia network in terms of F1, recall and precision in all classes except the not observed class. Reasons for this difference could be the imbalanced datasets and different network structures. The Wikipedia network has biased predictions towards the not observed class while the school network shows consistent performance. 

In conclusion, the real world network has a higher performance compared to the online network. We must keep in mind that comparing these networks is challenging due to the different network structure. Therefore, future research could compare more similar networks to obtain more generalisable results. In addition, it is important to overcome the problem of imbalanced data in order to obtain reliable and consistent results.

**Keywords**: Network analysis, signed networks, positive and negative ties, machine learning models, online and real world networks, Python. 

### Data Sources
The Wikipedia network is an open-source network, extracted from Stanford Network Analysis Platform (SNAP) . The school dataset is not open source, however there is a possibility to apply for access . The participants are anonymized to protect the privacy and data will not be shared.

Wikipedia dataset: https://snap.stanford.edu/data/wiki-RfA.html

School dataset application: https://www.cils4.eu/index.php?option=com_content&view=article&id=5&Itemid=6

