Semana 15 - Clasificación avanzada
==================================

### Descripción

En esta semana se continúa el desarrollo de Machine Learning con aprendizaje supervisado, enfocado en métodos más avanzados de clasificación. El objetivo es conocer una mayor gama de clasificadores para contar con diversas técnicas a comparar a la hora de modelar un clasificador sobre un conjunto de datos.
Los algoritmos a ser utilizados son:

- **Logistic Regression**
    - *Modelo:* Se modela la probabilidad de ocurrencia de un evento (clase positiva) a partir de una caracterización X (clasificación binaria)
    - *Optimización:* Varios (e.g. Gradiente Ascendente, L-BFGS)

- **Support Vector Machine**
    - *Modelo:* Hiperplano que maximiza el margen entre clases respecto a los puntos más cercanos
    - *Optimización:* Varios (e.g. Gradiente Ascendente, L-BFGS) 

- **Ensemble Learning**
    - **Boosting**: En cada iteración, modelos simples se van mejorando dando prioridad a ejemplos mal predichos. 
    - **Bagging:** Se entrenan diferentes modelos no correlacionados, y luego se agregan las predicciones de todos. 
    - **Stacking:** Similar a bagging, entrenando otro predictor para "aprender" la mejor agregación de predicciones.
       
- **One Class Classifier**
    - Utilizado en casos donde sólo se conoce el concepto de una clase a ser identificada
    - e.g. outlier detection, fraud prevention, etc
    - Incluso utilizado para multi-clases (e.g. one vs rest)
       
  
###  Tutoriales y ejemplos

- Logistic Regression
    - https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
    - https://medium.com/technology-nineleaps/logistic-regression-gradient-descent-optimization-part-1-ed320325a67e
    - https://towardsdatascience.com/building-a-logistic-regression-in-python-step-by-step-becd4d56c9c8
    - https://www.datacamp.com/community/tutorials/understanding-logistic-regression-python
    - https://www.dataschool.io/guide-to-logistic-regression/
- Support Vector Machine
    - https://jakevdp.github.io/PythonDataScienceHandbook/05.07-support-vector-machines.html
    - https://scikit-learn.org/stable/modules/svm.html
    - https://stackabuse.com/implementing-svm-and-kernel-svm-with-pythons-scikit-learn/
    - https://www.learnopencv.com/svm-using-scikit-learn-in-python/
    - http://web.mit.edu/6.034/wwwbob/svm-notes-long-08.pdf
- Ensemble Learning
    - https://en.wikipedia.org/wiki/Ensemble_learning
    - https://scikit-learn.org/stable/modules/ensemble.html 
    - https://towardsdatascience.com/ensemble-learning-using-scikit-learn-85c4531ff86a
    - https://www.analyticsvidhya.com/blog/2018/06/comprehensive-guide-for-ensemble-models/
    - https://www.datacamp.com/community/tutorials/ensemble-learning-python
- One Class Classifier
    - https://en.wikipedia.org/wiki/One-class_classification
    - https://dev.to/stevenbruno/an-introduction-to-one-class-classification-2m5c
    - https://ayush-iitkgp.github.io/posts/one-class-classification-algorithms/
 
   