# Simulaciones-coocurrencias

Estos programas simulan las ocurrencias de 12 presas y 3 depredadores.

Están programados en octave.

$${\color{blue}Entradas}$$
Sólo es necesario descargar los programas sim1.m y sim2.m y correr en octave por separado, ya que corresponden a abundancias distintas, el programa no solicitará ninguna información.

> [!NOTE]
> Cada corrida del programa proporciona una simulación distinta aunque similar

13,14,15 corresponden a los depredadores

1,2,3,4 son las presas para el depredador 13
- la especie 13 se mueve completamente al azar, al igual que sus presas

5,6,7,8 son las presas para el depredador 14
- la especie 14 pasa entre 10 y 12 días después de la especie 5 
- la especie 14 pasa entre 10 y 12 días antes de la especie 6 
- la especie 14 pasa entre 5 y 7 días antes de la especie 7 
- la especie 14 pasa el mismo día que la especie 8

9,10,11,12 son las presas para el depredador 15
- la especie 15 pasa entre 2 y 4 días después de la especie 9
- la especie 15 pasa entre 10 y 12 días antes de la especie 10
- la especie 15 pasa entre 3 y 5 días antes de la especie 11
- la especie 15 pasa el mismo día que la especie 12

Cada especie se observa con distinta frecuencia

En el código sim1.m las abundancias se comportan de la siguiente manera

|    Especie    |  Abundancia   |
| --------------| ------------- |
| 1,5,9,  | Baja |
| 2,6,10,15  | Regular |
| 3,7,11,14  | Media|
| 4,8,12,13  | Alta |

En el código sim2.m las abundancias se comportan de la siguiente manera

|    Especie    |  Abundancia   |
| --------------| ------------- |
| 1,5,9,  | Muy baja |
| 2,6,10,15  | Baja |
| 3,7,11,14  | Regular|
| 4,8,12,13  | Media |


$${\color{blue}Salidas}$$
Las salidas son los archivos de texto

- $${\color{purple}MI}$$ Matriz tridimensional, cada matriz de 2x2 corresponde a una especie y contiene en sus filas los días y en sus columnas las estaciones 
- $${\color{purple}fechas}$$ contiene día inicial de colocación de la cámara, día final y número de días instalada
- $${\color{purple}Frec}$$ contiene la frecuencia de ocurrencia por especie (fila) y por estación (columna)
- $${\color{purple}Lista}$$ Lista con tres columnas, la primera corresponde al día, la segunda a la estación y la tercera a la especie


Se muestran ejemplos de los archivos de salida
