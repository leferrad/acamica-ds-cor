Semana 20 - Unsupervised Learning
=================================

### Descripción

En esta semana se desarrollan técnicas relacionadas a Aprendizaje No Supervisado en Machine Learning. En esta rama, se trata de obtener un modelo a partir de las variables o "features" de entrada únicamente, sin contar con una variable de etiquetas o "ground truth" que guíe la tarea a realizar de forma supervisada. Se definen los tipos de tarea de Machine Learning que pueden realizarse en esta rama, así como los algoritmos más populares y las técnicas de evaluación para problemas de esta índole.

### Tipos de Tareas

1. **Clustering**
    - Algoritmos
        - K-means
        - GMM     
        - Mean-Shift
        - Spectral
    - Métricas
        - Supervisado (usando Ground Truth)
            - Adjusted Rand Index
            - Jaccard
            - Adjusted Mutual Information 
            - V-measure
        - No supervisado (sin GT)
            - Silhouette Coefficient
            - Calinski-Harabasz Index
            - Contingency Matrix

2. **Reducción de dimensiones**
    - Algoritmos
        - SVD
        - PCA      
        - Neural Networks
            - AutoEncoder
            - Word2Vec
        - t-SNE
        
    - Métricas
        - Explained variance
        - MSE (reconstrucción)      

3. **Sistema de recomendaciones**
    - To be filled...
    
4. **Detección de anomalías**
    - To be filled...
    
  
###  Tutoriales y ejemplos

- K-means
    - https://www.aprendemachinelearning.com/k-means-en-python-paso-a-paso/
    - https://bigdata-madesimple.com/possibly-the-simplest-way-to-explain-k-means-algorithm/
    - https://www.datacamp.com/community/tutorials/k-means-clustering-python
    - https://codeahoy.com/2017/02/19/cluster-analysis-using-k-means-explained/
    - https://blog.easysol.net/machine-learning-algorithms-3/
- Gaussian Mixture Models
    - https://jakevdp.github.io/PythonDataScienceHandbook/05.12-gaussian-mixtures.html
    - https://medium.com/clustering-with-gaussian-mixture-model/clustering-with-gaussian-mixture-model-c695b6cd60da
    - https://scikit-learn.org/stable/modules/mixture.html
    - https://towardsdatascience.com/gaussian-mixture-model-clusterization-how-to-select-the-number-of-components-clusters-553bef45f6e4
- Mean-shift clustering
    - https://spin.atomicobject.com/2015/05/26/mean-shift-clustering/
    - https://scikit-learn.org/stable/modules/generated/sklearn.cluster.MeanShift.html
    - https://towardsdatascience.com/machine-learning-algorithms-part-13-mean-shift-clustering-example-in-python-4d6452720b00
    - http://efavdb.com/mean-shift/
- Spectral clustering
    - https://towardsdatascience.com/spectral-clustering-aba2640c0d5b
    - https://calculatedcontent.com/2012/10/09/spectral-clustering/
    - https://medium.com/@tomernahshon/spectral-clustering-from-scratch-38c68968eae0
    - https://scikit-learn.org/stable/modules/generated/sklearn.cluster.SpectralClustering.html
- Clustering metrics
    - https://scikit-learn.org/stable/modules/clustering.html#clustering-performance-evaluation
    - https://medium.com/@ODSC/assessment-metrics-for-clustering-algorithms-4a902e00d92d
    - https://towardsdatascience.com/k-means-clustering-algorithm-applications-evaluation-methods-and-drawbacks-aa03e644b48a
- PCA & SVD
    - https://towardsdatascience.com/a-step-by-step-explanation-of-principal-component-analysis-b836fb9c97e2
    - https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html
    - https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.TruncatedSVD.html#sklearn.decomposition.TruncatedSVD
    - https://machinelearningmastery.com/calculate-principal-component-analysis-scratch-python/
    - https://towardsdatascience.com/pca-and-svd-explained-with-numpy-5d13b0d2a4d8
    - http://setosa.io/ev/principal-component-analysis/
    - https://georgemdallas.wordpress.com/2013/10/30/principal-component-analysis-4-dummies-eigenvectors-eigenvalues-and-dimension-reduction/
    