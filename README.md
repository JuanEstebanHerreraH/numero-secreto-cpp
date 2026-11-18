# Número secreto · C++

**Ejercicio de consola sobre números aleatorios, comparación de listas y conteo de aciertos.**

Proyecto académico para un parcial en la CUN. El archivo fuente visible en el repositorio es [ParcialC++.cpp](ParcialC%2B%2B.cpp); no se documenta como si hubiera una implementación Java separada disponible.

## Cómo funciona

1. Genera cinco números secretos distintos entre 100 y 130.
2. Solicita cinco números al usuario.
3. Compara ambas listas, cuenta coincidencias y muestra una nota.

## Compilar y ejecutar

Necesitas un compilador C++ como GCC/MinGW.

~~~sh
g++ "ParcialC++.cpp" -o numero-secreto
~~~

En Windows ejecuta `.\numero-secreto.exe`; en Linux o macOS, `./numero-secreto`.

## Comportamiento actual y pendiente de corregir

| Coincidencias contadas | Nota que imprime el código actual |
| --- | --- |
| Más de 2 | 4.80 |
| 2 o menos | 3.0 |

El mensaje inicial anuncia 4.80 con un mínimo de dos aciertos, pero la condición implementada es `contador > 2`. Tampoco aplica una nota distinta para cero aciertos. Esta diferencia se conserva como límite del ejercicio, no como una función corregida.

La entrada no valida el rango ni evita que el usuario repita números. El conteo puede aumentar por repeticiones en la entrada. Se utiliza `rand()` con una semilla temporal para practicar; no es un generador criptográfico.

## Qué se practica

Arreglos, bucles anidados, generación pseudoaleatoria, comparación de valores y condicionales. El archivo comprimido del repositorio se conserva como material adicional del trabajo.
