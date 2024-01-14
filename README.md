# ARS_CEB_Hito2
Detección de comunidades utilizando algoritmos evolutivos multiobjetivo.

El objetivo principal de esta práctica consiste en la definición de un método que permita la detección de comunidades en un grafo. Concretamente, se busca encontrar el método más adecuado que permita dividir en sus correspondientes comunidades una red de datos reales de Amazon, donde cada nodo es un artículo de Amazon y dos nodos están conectados entre sí cuando suficientes usuarios han comprado los dos artículos juntos. Esta red de Amazon se encuentra dividida en 8 comunidades correspondientes a las categorías de los productos.

Como primera aproximación para intentar encontrar la fragmentación real que este grafo de Amazon presenta, se intentará optimizar la modularidad de la solución generada empleando el algoritmo de Leiden. Como segunda aproximación, se optimizará de manera simultánea la community_score y el internal_density de la solución encontrada empleando algoritmos evolutivos multiobjetivo. Posteriormente, se analizará la calidad de las soluciones generadas por los frentes de Pareto que estos algoritmos generan y se comparará con la solución real buscada para determinar su similitud.

Para la ejecución de este notebook se puede emplear cualquier entorno que cuente con Python 3.10.12.
Recomendamos usar Google Colab ya que es el entorno con el que se ha programado pero no es estrictamente necesario. Alternativas como Anaconda o Jupiter Lab son completamente válidas.
Todas las dependencias necesarias están incluidas dentro del propio código y se instalan automáticamente ejecutando el mismo. Mientras se tenga acceso a internet, (al menos en la primera ejecución), no debería haber ningún problema relacionado con las mismas.  

Cabe destacar que las rutas de acceso a los datos (el grafo) pueden variar dependiendo de dónde se guarden los mismos. El código está configurado para utilizar Google Drive, por lo que, si no se guardan los datos en la misma ruta configurada o se usa otro estilo de almacenamiento, será necesario cambiar las rutas de carga de los datos.

En este repositorio se incluye, por comodidad, el grafo original con el que se trabaja en el código.
