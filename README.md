We analyzed a labeled dataset of Persian tweets using three topic modeling algorithms: Latent Dirichlet Allocation (LDA), Combined Topic Modeling (CTM), and BERTopic. For BERTopic, we experimented with two clustering methods: HDBSCAN and K-Means.

Each algorithm grouped related tweets into clusters, and we evaluated the purity of these clusters based on the predefined labels of the tweets within them. The table below presents the number of clusters, average purity, and the minimum and maximum purity for each method.

As shown in the table, BERTopic with K-Means achieved the highest average purity, demonstrating the best overall performance among the tested algorithms.

| Algorithm               | Number of Clusters | Average Purity | Min Purity | Max Purity |
|-------------------------|-------------------|---------------|------------|------------|
| LDA                    | 7                 | 0.2482            | 0.1919         | 0.3679         |
| CTM                    | 7                 | 0.5739            | 0.4127         | 0.8974         |
| BERTopic (HDBSCAN)     | 9                 | 0.6613            | 0.2632         | 0.9359         |
| BERTopic (K-Means)     | 7                 | **0.7232**        | 0.5699         | 0.8795         |
