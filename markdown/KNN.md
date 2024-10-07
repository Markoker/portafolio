# K-Nearest Neighbors Classifier

Es un método supervisado no parametrico de aprendizaje usado para clasificación.

Clasifica datos en base a los k (constante definida por el usuario) puntos más cercanos de los datos de entrenamiento.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/7/78/KNN_decision_surface_animation.gif/960px-KNN_decision_surface_animation.gif)

## Implementacion sklearn:

### Parametros:
- *n_neighbors*: Cantidad de vecinos más cercanos a tomar en cuenta a la hora de determinar la clase.
- *weights*: Determina si todos los puntos tendrán el mismo impacto en la 'votación' (*'uniform'*) o si el peso en la votación será inversamente proporcional a la distancia del punto (*'distance'*).
- *p*: Parámetro de la potencia para la distancia de Minkowski. La cual está definida como la raíz p-ésima de la suma de las diferencias elevadas a *p*
![img.png](src/minkowski.png) notar que con *p* = 2 es equivalente a la distancia euclideana 
- *metric*:
    - *'euclidean'*
    - *'manhattan'*
    - *'cosine'*