
n amplificador operacional, comúnmente conocido como "op-amp" (abreviatura de operational amplifier en inglés), es un dispositivo electrónico con dos entradas y una sola salida, diseñado para amplificar señales eléctricas. Es uno de los componentes más importantes en la electrónica analógica y se utiliza ampliamente en circuitos para realizar diversas funciones, como amplificación, sumas, restas, integración, derivación, entre otras.

El símbolo esquemático del amplificador operacional es un triángulo con dos entradas marcadas (+ y -) y una salida:

<div align="center">
  <img src="imagenes/imagen_45.png" width="400px">
</div>



Las dos entradas del op-amp son:

La entrada no inversora (+): Es la terminal donde se aplica la señal de entrada que se quiere amplificar. La señal en esta entrada no se invierte.

La entrada inversora (-): Es la terminal donde se aplica la señal de retroalimentación o la señal de entrada si se desea amplificar con inversión. La señal en esta entrada se invierte y se compara con la señal en la entrada no inversora.

La salida del amplificador operacional se genera como una amplificación de la diferencia de voltaje entre las dos entradas, multiplicada por un factor de ganancia (A):

<div align="center">
  <img src="imagenes/imagen_46.png" width="400px">
</div>

El valor de K es muy grande, típicamente 10^5


En teoría, el valor de ganancia (K) es infinito, pero en la práctica, los amplificadores operacionales tienen una ganancia muy alta. Por lo tanto, cualquier pequeña diferencia entre las dos entradas generará una salida amplificada significativamente.

Los amplificadores operacionales se alimentan con una fuente de voltaje dual (por ejemplo, +Vcc y -Vcc) para permitir la amplificación de señales tanto positivas como negativas.

Es importante destacar que el amplificador operacional ideal tiene características ideales, como alta impedancia de entrada, ganancia infinita, ancho de banda infinito y rechazo infinito del modo común. Sin embargo, en la práctica, los amplificadores operacionales reales tienen limitaciones debido a la tecnología y otros factores, y estas limitaciones se tienen en cuenta al diseñar y utilizar circuitos con op-amps.
