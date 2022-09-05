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
* Cuando ya portan 5 cajas o no hay más cajas en el suelo de la cuadricula, las llevan a la estantería 
* Cuando ya no hay cajas en la cuadricula, los robots se estacionan en la esquina inferior derecha

### Sobre las cajas
* Se inicializan en posiciones vacías aleatorias dentro de la cuadricula
* Pueden coexistir en el mismo espacio que otros agentes, aunque dada nuestra implementación este caso no se presenta.

### Sobre la estantería
* Se inicializa en la esquina superior izquierda
* Puede contener una cantidad ilimitada de cajas
