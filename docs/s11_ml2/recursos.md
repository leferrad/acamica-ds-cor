Semana 11 - Machine Learning (cont)
===================================

### Descripción

En esta semana se continúa el desarrollo de conceptos sobre Machine Learning, enfocado a tareas de aprendizaje supervisado. El objetivo es entender los pasos para obtener un modelo de forma supervisada a partir de un conjunto de datos, así como la validación adecuada del desempeño que dicho modelo tiene sobre un conjunto reservado para pruebas.

- **Carga de datos:** Lectura de fuente de datos (e.g. CSV, base de datos, streaming, etc) en un DataFrame.

- **Pre-procesamiento:** En caso de que el DataFrame no esté listo para modelar, procesarlo para convertirlo en un conjunto de "features" numéricas a ser procesadas por el modelo. 

- **Split:** Partir DF en train-valid-test usando algún criterio adecuado (e.g. 80/20, leave k-out, etc).

    - El conjunto de valid sirve para el ajuste de hiper-parámetros aunque es opcional. 
    
- **Configurar modelo a ajustar:** Definir los hiperpárametros y la arquitectura del modelo a ser ajustado, así como el método de optimización a utilizar.

- **Ajustar modelo:** Utilizar conjunto de train (y de valid, si existe) para ajustar el modelo definido.

- **Validar modelo:** Utilizar conjunto de test para validar el desempeño del modelo ajustado usando métricas adecuadas dependiendo del tipo de modelo.

- **Re-ajustar modelo:** En caso de que el desempeño actual no sea apropiado, volver a ajustar el modelo cambiando la configuración utilizada.
    - En caso de que estos cambios no sean suficientes, evaluar la posibilidad de cambiar alguna etapa del pre-procsamiento de datos (garbage in, garbage out).

- **Chequeo final y guardar en disco:** Se chequea el resultado final del modelo respecto a los criterios de aceptación manejados, y se guarda en disco tanto el modelo como la salida obtenida sobre el conjunto de test (si se requiere).

###  Tutoriales y ejemplos

- Regresión Lineal
    - https://www.geeksforgeeks.org/linear-regression-python-implementation/
    - https://www.datacamp.com/community/tutorials/essentials-linear-regression-python
    - https://datatofish.com/multiple-linear-regression-python/
    - https://scikit-learn.org/stable/auto_examples/linear_model/plot_ols.html
    - https://www.digitalvidya.com/blog/tutorial-on-python-linear-regression-with-example/