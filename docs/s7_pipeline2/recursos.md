Semana 7 - Data Pipelines
=========================

### Descripción

En esta semana se continúa el desarrollo de data pipelines para el tratamiento de un conjunto de datos. El objetivo de esta tarea es especificar y desarrollar un tratamiento de estos datos para obtener una versión "curada" de los mismos que sirva para desarrollar una tarea analítica definida (e.g. análisis de correlación de variables, análisis descriptivo, predecir una variable de interés, clustering de datos, etc). 

Esta es una propuesta de los posibles pasos a seguir para implementar un pipeline de datos abarcativo (no estrictamente en ese orden):


- **Carga de datos:** Lectura de fuente de datos (e.g. CSV, base de datos, streaming, etc) en uno o más DataFrames. 

- **Definición del objetivo del pipeline:** Se debe documentar de forma abstracta lo que se pretende obtener a partir del pipeline a desarrollar, en términos de una tarea analítica a desarrollar sobre los datos de entrada que agregue valor al negocio o dominio.

- **Select de columnas a utilizar:** Acotar pipeline a un conjunto conocido de columnas a ser tratadas para optimizar el desempeño computacional del mismo. 

- **Limpieza de datos:** Para remover observaciones no deseadas (e.g. outliers, valores faltantes o nulos, etc).

- **Transformación de datos:** Convertir columnas de entrada en otro formato o representación conveniente (e.g. normalizado, escalado, categorías numéricas, etc).

- **Chequeo final y guardar en disco:** Se chequea el resultado final del pipeline respecto a lo definido inicialmente.


###  Tutoriales y ejemplos

- **Limpieza de datos**
    - **Outliers filtering**
        - https://towardsdatascience.com/ways-to-detect-and-remove-the-outliers-404d16608dba
        - http://colingorrie.github.io/outlier-detection.html
        - https://medium.com/datadriveninvestor/finding-outliers-in-dataset-using-python-efc3fce6ce32
        - http://www.ttable.org/z-score-table.html
        - https://mathbitsnotebook.com/Algebra2/Statistics/STzScores.html
- **Transformación de datos**
    - **Funciones en Pandas**
        - https://github.com/nvmoyar/datascience_notebooks/blob/master/Manipulating_DataFrames_with_Pandas.ipynb
        - https://chrisalbon.com/python/data_wrangling/pandas_apply_operations_to_dataframes/
        - http://queirozf.com/entries/pandas-dataframe-by-example
        - https://chrisalbon.com/python/data_wrangling/pandas_join_merge_dataframe/
    
    - **Escalado**
        - http://www.datasciencemadesimple.com/scaling-normalizing-column-pandas-dataframe-python/
        - https://www.kaggle.com/parasjindal96/how-to-normalize-dataframe-pandas
        - https://scikit-learn.org/stable/modules/preprocessing.html
        - https://scikit-learn.org/stable/auto_examples/preprocessing/plot_all_scaling.html
         
    - **One-Hot Encoding**
        - https://machinelearningmastery.com/how-to-one-hot-encode-sequence-data-in-python/
        - https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html
    
    