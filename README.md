# Evidencia 1. Actividad Integradora - Robots en un almacen

Este modelo representa un espacio de *N* por *M* casillas con una cantidad *K* de cajas repartidas de manera aleatoria por el espacio. En el espacio también existe una cantidad *X* de Robots cuya misión es llevar las cajas a la estantería ubicada en la esquina superior izquierda de la cuadricula. 

## Integrantes del equipo
* Luis Ángel Guzmán Iribe - A01741757
* Cesar Galvez - A01252177
* Antonio López Chávez - A01741741
* Sebastián Gálvez Trujillo - A01251884

## Profesores
* María Angélica Barreda Beltrán
* Jorge Mario Cruz Duarte

## Reglas

### Sobre los robots:
* Se inicializan en posiciones vacías aleatorias dentro de la cuadricula
* Únicamente pueden moverse hacia las casillas directamente adyacentes a su posicion actual (excluyendo diagonales)
* Únicamente pueden moverse hacia casillas vacías, y no pueden coexistir con otro agente en la misma casilla
* Pueden cargar un máximo de 5 cajas al mismo tiempo
* Cuando ya portan 4 cajas o no hay más cajas en el suelo de la cuadricula, la llevan a la estantería más cercana a la esquina superior izquierda que aún no tiene 5 cajas
* Cuando ya no hay cajas en la cuadricula, los robots se estacionan en la esquina inferior derecha

#### Sobre el Vuelo de Lévy:
La implementación del vuelo de Lévy para este programa funciona seleccionando una casilla aleatoria en la cuadrícula y moviendo al agente hasta esa dirección sin interrupciones. Esta implementación, reduce considerablemente el número de movimientos de los agentes y la cantidad de generaciones necesarias para recoger todas las cajas del piso. El movimiento browniano o aleatorio, en comparación, presenta un mayor número de movimientos y obtiene tiempos de finalización más largos.
En el pdf adjunto se incluye una comparación del desempeño de ambos modelos, con Vuelo de Levy y con Movimiento Browniano a lo largo de 10 ejecuciones del sistema.

### Sobre las cajas
* Se inicializan en posiciones vacías aleatorias dentro de la cuadricula
* Pueden coexistir en el mismo espacio que otros agentes, aunque dada nuestra implementación este caso no se presenta.

### Sobre la estanterías
* Se inicializan en la esquina superior izquierda
* Pueden contener un máximo de 5 cajas cada una