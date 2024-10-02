# DFS
búsqueda en profundidad iterativa (IDDFS) para encontrar una solución en un grafo de vuelos entre ciudades. La estructura es correcta, pero algunos detalles podrían mejorarse para asegurar que funcione adecuadamente. Aquí te comparto algunas observaciones:

Alcance global de conexiones: En tu función imprimir(), la variable conexiones se define como global, pero luego no es accesible dentro de la función buscar_solucion_DFS_Rec porque no es global ahí. Para evitar este problema, puedes pasar conexiones como un argumento a las funciones recursivas.

Problema con el estado de visitados: La lista visitados se pasa por referencia, lo que puede provocar que se modifique en profundidad sin control. Deberías crear una copia de visitados al hacer la llamada recursiva para evitar este problema.

Método en_lista: Asegúrate de que la clase Nodo tenga el método en_lista, que no está definido aquí.

Control de límites: El código maneja adecuadamente el límite de profundidad para el algoritmo de búsqueda iterativa.
