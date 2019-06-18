Semana 18 - Natural Language Processing (NLP)
=============================================

### Descripción

En esta semana se retoma la etapa de preparación de datos en un proyecto de DS, pero en este caso enfocándose en texto como tipo de fuente de datos. Se explican métodos para pre-procesar texto y extracción de características en formato numérico para poder modelar a partir de una fuente transformada. 
  
### Etapas

(Orden sugerido, pero no estricto)

- **Normalización:** Para que las siguientes etapas de pre-procesamiento se puedan aplicar sobre una base normal de texto, se debe transformar el mismo en base a ciertas reglas, tales como:
    - Case (por lo general, lowercase)
    - Reemplazar:
        - Sinónimos
        - Abreviaciones
        - Typos (e.g. codroba -> cordoba)
        - etc
    - Remover puntuación y caracteres no deseados.
    - Stemmer and Lemmatizer (para conjugaciones, si se desea)
    - Traducción a un único lenguaje

- **Limpieza:** Se debe limpiar lo más posible el texto, para que se acote a un universo conocido de palabras que luego se puedan convertir en features numéricas de forma adecuada y predecible. 
    - Remover stop-words (e.g. a, hacia, el, de)
    - Blacklist and Whitelist (i.e. elegir palabras soportadas)
    - Regular expressions, para facilitar tarea de extracción de palabras de interés.

- **Tokenización:** Una vez que se tiene texto limpio y normalizado, es conveniente convertirlo en arreglos de palabras/letras que luego sean candidatas a ser convertidas en números.
    - Split en base a caracteres (espacios blancos, puntos)
    - Regular expressions, para extraer palabras de interés.
    - N-gramas

- **Feature extraction:** Para poder utilizar esta información en un modelo, se debe convertir en formato numérico de forma conveniente para la tarea pretendida. Esto quiere decir que no solo se deben asignar números por cada palabra, sino también que el número caracterice correctamente en base al contexto del documento.
    - Basados en frecuencias:
        - Bag of Words (BoW)
        - TF-IDF
        - BM25
    - Basados en Similaridad mediante Redes Neuronales:
        - Word2Vec
        - GloVe
    - Aplicando técnicas de NLP
        - Part of Speech tagging (PoS)
        - Named-entity recognition (NER)
        - WordNet synsets  

- **Métricas de similitud:** Para poder comparar documentos en forma numérica, se pueden utilizar diversas funciones dependiendo del formato dado de la información:
    - Basadas en texto:
        - Levenshtein, Hamming, Fuzzy
    - Basadas en conjuntos (letras, n-gramas, palabras):
        - Jaccard, Sorensen Dice
    - Basadas en vectores numéricos:
        - Cosine, Correlation
    - Basadas en histogramas de palabras:
        - Hellinger, Jensen-Shannon
    
- **Visualización:**
    - Histograma de palabras
    - Boxplot
    - WordCloud
    - t-SNE
    - Scattertext
    - N-gram frequency distribution plot

  
  
###  Tutoriales y ejemplos

- Text cleaning:
    - https://medium.com/@dobko_m/nlp-text-data-cleaning-and-preprocessing-ea3ffe0406c1
    - https://medium.com/@datamonsters/text-preprocessing-in-python-steps-tools-and-examples-bf025f872908
    - https://machinelearningmastery.com/clean-text-machine-learning-python/
    - https://www.analyticsvidhya.com/blog/2018/02/the-different-methods-deal-text-data-predictive-python/
- Aplicaciones de NLP con Python: 
    - https://www.analyticsvidhya.com/blog/2017/01/ultimate-guide-to-understand-implement-natural-language-processing-codes-in-python/
    - https://levelup.gitconnected.com/machine-learning-with-python-nlp-and-text-recognition-94444d55b0ef
    - https://likegeeks.com/es/tutorial-de-nlp-con-python-nltk/
    - https://appliedmachinelearning.blog/2017/02/12/sentiment-analysis-using-tf-idf-weighting-pythonscikit-learn/
- NLP avanzado con Gensim:
    - https://www.machinelearningplus.com/nlp/gensim-tutorial/
    - http://kavita-ganesan.com/gensim-word2vec-tutorial-starter-code/#.XQhSiMszY3E
    - https://www.oreilly.com/learning/how-do-i-compare-document-similarity-using-python
    - http://lixinzhang.github.io/implementation-of-okapi-bm25-on-python.html
- Text similarity:
    - https://towardsdatascience.com/overview-of-text-similarity-metrics-3397c4601f50
    - https://medium.com/@adriensieg/text-similarities-da019229c894
    - http://sibiryakov.eu/2011/11/similarity-metrics/
    - https://www.oreilly.com/learning/how-do-i-compare-document-similarity-using-python
- Visualization:
    - https://itnext.io/basics-of-text-analysis-visualization-1978de48af47 
    - https://towardsdatascience.com/a-complete-exploratory-data-analysis-and-visualization-for-text-data-29fb1b96fb6a
    - https://kanoki.org/2019/03/17/text-data-visualization-in-python/
    - https://www.mien.in/2017/10/02/visual-text-analytics-with-python/
    - https://www.districtdatalabs.com/text-analytics-with-yellowbrick