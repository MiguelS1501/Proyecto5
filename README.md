# Proyecto 5. Sistema M/M/s. 

Nombre: Miguel Andrés Salazar Alvarado. 

Carné: B97118.

En el siguiente proyecto se hizo uso de la cadenas de Markov, las cuales se conocen como modelos de Markov o proceso de Markov, es un concepto desarrollado dentro de la teoría de la probabilidad y la estadística que establece una fuerte dependencia entre un evento y otro suceso anterior. Su principal utilidad es el análisis del comportamiento de procesos estocásticos.

![alt text](https://github.com/MiguelS1501/Proyecto4/blob/main/arenal.png)

Separando la funcionalidad de las secciones modificadas se tiene que: 

1- ) En la parte de modulación la señal le ingresa un vector unitario que luego se le cambia la forma por medio de la función de Numpy "reshape", dejandolo como matriz de Nx4. 
La misma igual que en la BPSK, presenta una función portadora s(t), la cual está compuesta por los componentes seno y coseno quienes son ortogonales. Los mismos se suman en una
sola variable. Estos presentan diversos valores para las amplitudes ([-3,-1,1,3]) dependiendo como indica el enunciado de los bits de la matriz los cuales están separados en b1, 
b2, b3 y b4. De esta manera y por medio de un for iterativo es posible encontrar los valores de ambos componentes. 

2- ) Ahora bien, en la parte de demodulación, se toma los valores de la parte anterior recostruyendo el seno y el coseno de la señal demodulada. Además se establece un criterio de
decisión por detección de energía en ambas portadoras, los cuales se encontraron através de variaciones con distintos números. En este caso se demodula la función para posteriormente
obtener la traducción de la misma por medio de una imagen. Los resultados indicaron que se hizo el proceso de manera correcta, debido a que tenía 0 errores y además se recuperaba 
la misma imagen. En las graficas se observaba la señal moduladora y el comportamiento acorde a la transmitida. 

Cabe destacar que las demás funciones se dejaron como estaban inicialmente y lo que se modificó, fueron estas dos para la primera parte. Lo anterior, debido a que cumplian con la 
misma funcionalidad. Depués, en la parte de ergodicidad y de estacionaridad, se hizo la comprobación mediante un porcentaje de error que el promedio de los datos corresponde 
al promedio en el tiempo, lo cual es el criterio de la ergodicidad. Como esta primera, es más restrictiva en su significado que la estacionaridad, una implica la otra. Sin embargo, 
se realizó la comprobación de que una de sus propiedades estadísticas (media) es igual a un valor constante para un intervalo de tiempo. Finalmente, mediante la densidad espectral de
potencia se visualizó un máximo de más de 140000 en su magnitud y se observa un comportamiento adecuado a los resultados obtenidos en las secciones anteriores. 

# Resultados obtenidos:

La siguiente muestra la imagen transmitida y recibida después del proceso de modulación:

![alt text](https://github.com/MiguelS1501/Proyecto4/blob/main/Recibida-Transmitida.JPG)

Además, se señalan las gráficas de las diferentes señales de especial relevancia que forman parte de las distintas secciones de transformación.

![alt text](https://github.com/MiguelS1501/Proyecto4/blob/main/grafica.png)

Seguidamente, se muestra un ejemplo de diferentes patrones de funciones en el tiempo. 

![alt text](https://github.com/MiguelS1501/Proyecto4/blob/main/ergodicidad.png)

Por último, es posible visualizar la gráfica que indica la magnitud espectral de potencia.

![alt text](https://github.com/MiguelS1501/Proyecto4/blob/main/potencia.png)
