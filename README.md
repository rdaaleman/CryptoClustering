# CryptoClustering

In my Visualize and Compare results my first Elbow graphcs, I recognize that the first graph looks like a line because the y index is so high on the graph. Which is showing lack of that curve. 

Support from BCBS for the following code: 
# Create a scatter plot using hvPlot by setting 
# `x="PC1"` and `y="PC2"`. 
# Color the graph points with the labels found using K-Means and 
# add the crypto name in the `hover_cols` parameter to identify 
# the cryptocurrency represented by each data point.

cryto_pca_predictions_graph = df_crypto_pca_predictions.hvplot.scatter(
    x="PCA1",
    y="PCA2",
    by="predicted_clusters",
    hover_cols="coin_id"
)
cryto_pca_predictions_graph

