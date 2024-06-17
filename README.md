### Approach:

1. Using prompt and huggingface Inference API (serverless), fetch the name of the parent entity of the given business entity.
2. Create clusters for each parent entity separately, using Kmeans cluster on the basis of the name of the business entity.
   1. Use TfidVectorizer to transform name of the business entity to numerical 
   2. Use silhouette_score to get the optimal number of clusters 

