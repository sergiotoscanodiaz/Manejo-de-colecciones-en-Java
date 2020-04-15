# Manejo-de-colecciones-en-Java

***

1. Introducción 

Entendemos como colección un contenedor de un conjunto de elementos de un mismo tipo. Se usa para almacenar, recuperar y manipular datos. Por ejemplo: se pueden tratar problemas del mundo real como un carrito de la compra que podría ser un conjunto de items. 

Las colecciones están recogidas en el paquete java.util.  

En cada versión de java se ha ido incluyendo o modificando colecciones. En Java 5 se incluyó el uso de genéricos. 

El framework de colecciones en Java nos ofrece las interfaces (tipos de datos), implementaciones (concreciones de los tipos de datos) y algoritmos (métodos). 

Tres de las ventajas del uso del framework e colecciones son: 

-Reduce el esfuerzo de programación. 

-Más calidad y velocidad en el programa. 

-Reutilización de software. 

***

2. Tipos de colecciones 

Interfaz Iterable: permite recorrer y eliminar elementos. Nos permite usar el bucle forEach. 

Interfaz Collection: extiende a Iterable, es decir, hereda su funcionalidad. El resto de las interfaces heredan de él, salvo Map. Se puede manipular las colecciones de una forma más general. Algunas de las operaciones son: add, remove, size, contains, toArray... 

Set: se trata de un Collection que no permite duplicados. No se puede acceder por posición. Mejora algunos métodos como equals. Implementaciones de Set: 

-HashSet: Almacena sus valores en una tabla hash. No se puede predecir el orden de los elementos. Mejor rendimiento. Se puede insertar valores nulos. 

-LinkedHashSet: Almacena sus valores en una tabla hash en una lista doblemente enlazada por lo que mantiene el orden de inserción. 

-TreeSet: Almacena sus valores en un árbol red-back de búsqueda de elementos. Mantiene el orden según sus valores. Peor rendimiento que LinkedHashSet y HashSet. No permite insertar nulos. 

-List:  Se trata de un Collection que sí permite duplicados. Añade funcionalidades como el acceso posicional, la búsqueda, la iteración extendida y operaciones sobre un rango de elementos.
Implementaciones de List: 

ArrayList: más adecuada en la mayoría de las situaciones, acceso por índice O(1) y menos espacio que LinkedList. 

LinkedList: suele tener peor rendimiento, acceso por índice O(n) y más espacio en memoria. 

Otras interfaces relacionados con List: Queue y Deque. 

-Map: no hereda de Collection. Maneja pares clave,valor. Para cada clave hay un solo valor. Cada clave existe una sola vez en el map. Se le conoce como diccionario. Operaciones comunes: put( key, value), get(key)… Las implementaciones de Map son HashMap, LinkedHashMap y TreeMap. 

-Colecciones no modificables: Una vez creadas, no se pueden modificar. Se pueden utilizar como resultado de un método u operación. 

-Colecciones sincronizadas: aptas para el uso de diferentes hilos de ejecución. Varios procesos que compiten por el uso de la colección. 

***

3. Algunos algoritmos para colecciones 

Disponibles en la clase Collections para ordenar o desordenar, buscar y operar con max/min, frecuencia... 

Algoritmos de ordenación: Collections.sort. 

De desordenación: Collections.shuffle. 

De búsqueda: Búsqueda binaria. La lista debe estar ordenada previamente. Devuelve el índice del elemento si lo encuentra. 

*** 

4. Librerías de colecciones de terceros 

Las librerías más usuales son: la implementada por Google, Guava, que está disponible en Java/Android con constructores mejorados entre otros, Eclipse Collections que es un API más legible con gestión de memoria mejorada y Apache Commons Collections que ofrece colecciones tipo Bag, colecciones compuestas... 

Por último, para poder ver ejemplos de las colecciones puede visitar este repositorio: https://github.com/OpenWebinarsNet/java-collections 

 

 
