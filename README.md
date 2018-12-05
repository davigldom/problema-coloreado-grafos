# Resolución del problema de coloreado de grafos mediante un algoritmo híbrido
Este proyecto educativo está realizado en el contexto de la asignatura de Inteligencia Artificial, en el grado de Ingeniería Informática - Ingeniería del Software de la Universidad de Sevilla. En dicho proyecto, se intenta dar solución al problema de coloreado de grafos mediante un algoritmo híbrido, el cual consiste en utilizar un algoritmo genético y sustituir el proceso de mutaciones por un enfriamiento simulado.

## Estructura del código fuente
El código implementado en "Problema del Coloreado de Grafos", sigue una jerarquía donde se implementan los métodos, en orden de necesidad, de modo que todo el código puede ser ejecutado de forma continua y seguida para no obtener ningún fallo por faltas de declaración. Dicho código, a pesar de estar escrito en Python, está diseñado para ser utilizado en el entorno de ejecución interactivo "Jupyter". Se tiene pensado en un futuro pasar el código, junto con algunas mejoras, a una librería común de Python.

Es importante que el código se ejecute en orden sin saltarse ninguna celda, ya que esto puedo provocar excepciones.

Aunque todo este código esta explicado y detallado celda a celda, se puede resumir el contenido en dos partes diferenciadas:

1. Algoritmo genético clásico, esto incluye, las declaraciones de genotipo, fitness, grafos, y toda la casuística necesaria para aplicar el algoritmo.

2. Algoritmo genético híbrido con enfriamiento simulado, donde se modifican los elementos necesarios para aplicar el algoritmo híbrido.

## Interfaz gráfica

Para usar la interfaz gráfica, basta con ejecutar la única celda del notebook asociado con título "Interfaz Gráfica del Problema de Coloreado de Grafos" ( Previa instalación de los paquetes necesarios ).

A continuación, se abrirá una ventana con diferentes menús donde podremos seleccionar todos los apartados que queramos configurar para, posteriormente, aplicar el algoritmo genético por mutación genérica o mixto con enfriamiento simulado.

En esta ventana, una vez determinados los valores, podemos aplicar tanto un algoritmo como otro, esto es, una vez mostrada la solución por enfriamiento simulado, podemos hacer click en el otro botón para obtener la solución asociada al mismo grado, con los mismos valores, mediante mutación, del mismo modo, podemos seguir modificando los valores y obtener nuevas soluciones.

Nota: En algunos casos en donde se ejecute seguidamente el programa, puede ser necesario reiniciar la interfaz, cerrándola y volviéndola a ejecutar.

## Realización de pruebas

Basta con probar en la propia interfaz proporcionada, los valores para los que queramos probar el algoritmo.

En caso de numerosas pruebas continuas, puede darse la situación de que la solución no varíe, pese a insertar un nuevo grafo en los campos, para ello, basta con cerrar la interfaz y volver a ejecutar la celda.

## Reproducción de experimentos
Para reproducir los experimentos realizados por el grupo, es necesario fijar los siguientes valores:

PRUEBA 1 (GRAFO COMPLETO)
- COLORES: 8
- NODOS: 200
- POBLACIÓN: 10
- NUMERO DE GENERACIONES: 50
- PROBABILIDAD DE CRUZAMIENTO: 0.5
- PROBABILIDAD DE MUTACION : 0.3

--------------------------------------------------------	
	
PRUEBA 2 (GRAFO ALEATORIO)
- COLORES: 6
- NODOS: 80
- POBLACIÓN: 20
- DENSIDAD: 0.15
- NUMERO DE GENERACIONES: 50
- PROBABILIDAD DE CRUZAMIENTO: 0.5
- PROBABILIDAD DE MUTACION : 0.3

--------------------------------------------------------	

PRUEBA 3 (GRAFO ALEATORIO)
- COLORES: 3
- NODOS: 20
- POBLACION: 5
- DENSIDAD: 0.15
- NUMERO DE GENERACIONES: 50
- PROBABILIDAD DE CRUZAMIENTO: 0.5
- PROBABILIDAD DE MUTACION : 0.3
	
----------------------------------------------------------

PRUEBA 4 (GRAFO ALEATORIO)
- COLORES: 3
- NODOS: 20
- POBLACION: 50
- DENSIDAD: 0.15
- NUMERO DE GENERACIONES: 50
- PROBABILIDAD DE CRUZAMIENTO: 0.5
- PROBABILIDAD DE MUTACION : 0.3
	
------------------------------------------------
	
PRUEBA 5 (PETERSEN - 10 NODOS)
- COLORES: 3
- NODOS: 10
- POBLACION: 20
- NUMERO DE GENERACIONES: 50
- PROBABILIDAD DE CRUZAMIENTO: 0.5
- PROBABILIDAD DE MUTACION : 0.3
	
--------------------------------------------------

PRUEBA 6 (PETERSEN - 10 NODOS)
- COLORES: 3
- NODOS: 10
- POBLACION: 20
- PROBABILIDAD DE MUTACION: 0.3 -> 0.6
- NUMERO DE GENERACIONES: 50
- PROBABILIDAD DE CRUZAMIENTO: 0.5

---------------------------------------------------

PRUEBA 7 (PETERSEN - 10 NODOS)
- COLORES: 3
- NODOS: 10
- POBLACION: 20
- PROBABILIDAD DE MUTACION: 0.3 -> 0.2
- NUMERO DE GENERACIONES: 50
- PROBABILIDAD DE CRUZAMIENTO: 0.5
	
---------------------------------------------------

PRUEBA 8 (PETERSEN - 10 NODOS)
- COLORES: 3
- NODOS: 10
- POBLACION: 20
- PROBABILIDAD DE MUTACION: 0.3 -> 0.05
- NUMERO DE GENERACIONES: 50
- PROBABILIDAD DE CRUZAMIENTO: 0.5
	
## Diseñar nuevos experimentnos
Para diseñar nuevos experimentos, basta con fijar un grafo base ( Que se utilizará a lo largo de las diferentes pruebas ), e ir dando valores en los campos mas relevantes ( Cambiar la población, la probabilidad de mutación, los colores ), de modo que solo cambiemos un campo y reproduzcamos el ejemplo un mínimo de 3 veces ( Dado la aleatoriedad de los algoritmos y poblaciones ).

Una vez realizada las pruebas con el grafo, se puede mover a otro nuevo tipo de grafo, y volver a repetir la misma batería de pruebas.
