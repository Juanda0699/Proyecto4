
# Proyecto 4

Se desea modular y demoludar una imagen usando una transmisión 
16-QAM

Parte 1: Modulación y Demoludación 

Para transmitir una imagen en 16 QAM, hay que modular y demoludar usando 4 bits (b1, b2, b3, b4), que están asociados a la posición en una matriz (-1, 4).
Por lo tanto se separa la señal en una forma de onda seno (b3, b4) y otra coseno (b1, b2) y se va llenado la matriz llamada señal Tx, la cual se le asignan el valor de la forma de onda por una amplitud que de depende del valor del bit en cierta posición (-3, -1, 1, 3).
Luego de pasar esta señal Tx por un canal ruidoso, se tiene que demoludar, es decir reconstruir la imagen transmitida por la moduladora, para ello se asocian energías a cada valor de bit, y se asigna este valor de nivel de energía a un bit respectivamente de acuerdo a la forma en que se modulo (b1, b2, b3, b4), según el criterio de selección.
El criterio de selección va por rangos, en este caso se usaron valores de 40, ya que la energía tomaba valores cercanos a estos y sirvieron ya que la imagen se reconstruyo como debía.
Se llega a la conclusión de que la imagen se reconstruyo correctamente para un SNR de 5, ya que la cantidad de errores es 0, para un BER de 0.

Parte 2: Estacionaridad y Ergodicidad

Para esta parte se compara el promedio de la señal Tx de manera temporal y estadística, una es por definición usando la integral y la otra el valor promedio para la señal Tx, respectivamente.
Al comparar se obtuvo que la diferencia entre los promedios es de 0.00465897%, por lo tanto se considera un proceso estacionario, al ser casi idénticos ambos valores (temporal y estadístico).

Parte 3: Densidad Espectral de Potencia

Al graficar la densidad espectral de potencia para la señal Tx, se observa que la mayor concentración es en el rango de 2000 a 4000 Hz, después es casi nula la magnitud por lo que se puede considerar despeciable.

  
