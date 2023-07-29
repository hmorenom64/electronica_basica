<div align="center">
<img src = "/.icons/image1.jpeg" >
</div>

<div align="center">
<b> Universidad Escuela Colombiana de Ingeniería Julio Garavito</b>
<br></div>

<div align="center">
Henry Moreno Mosquera
<br></div>

<div align="center">
Profesor del Centro de Estudios Electrónicos
<br></div>

<div align="center">
henry.moreno@escuelaing.edu.co
<br></div>



# **CURSO DE ELECTRONICA BASICA PARA INGENIEROS. MODULO 1. AMPLIFICADORES OPERACIONALES**

## Amplificador Operacional

Un amplificador operacional, comúnmente conocido como "op-amp" (abreviatura de operational amplifier en inglés), es un dispositivo electrónico con dos entradas y una sola salida, diseñado para amplificar señales eléctricas. Es uno de los componentes más importantes en la electrónica analógica y se utiliza ampliamente en circuitos para realizar diversas funciones, como amplificación, sumas, restas, integración, derivación, entre otras.

El símbolo esquemático del amplificador operacional es un triángulo con dos entradas marcadas (+ y -) y una salida:

<div align="center">
  <img src="imagenes/imagen_45.png" width="400px">
</div>



Las dos entradas del op-amp son:

La entrada no inversora (+): Es la terminal donde se aplica la señal de entrada que se quiere amplificar. La señal en esta entrada no se invierte.

La entrada inversora (-): Es la terminal donde se aplica la señal de retroalimentación o la señal de entrada si se desea amplificar con inversión. La señal en esta entrada se invierte y se compara con la señal en la entrada no inversora.

La salida del amplificador operacional se genera como una amplificación de la diferencia de voltaje entre las dos entradas, multiplicada por un factor de ganancia K):

<div align="center">
  <img src="imagenes/imagen_46.png" width="400px">
</div>

El valor de K es muy grande, típicamente 10^5


En teoría, el valor de ganancia (K) es infinito, pero en la práctica, los amplificadores operacionales tienen una ganancia muy alta. Por lo tanto, cualquier pequeña diferencia entre las dos entradas generará una salida amplificada significativamente.

Los amplificadores operacionales se alimentan con una fuente de voltaje dual (por ejemplo, +Vcc y -Vcc) para permitir la amplificación de señales tanto positivas como negativas.

Es importante destacar que el amplificador operacional ideal tiene características ideales, como alta impedancia de entrada, ganancia infinita, ancho de banda infinito y rechazo infinito del modo común. Sin embargo, en la práctica, los amplificadores operacionales reales tienen limitaciones debido a la tecnología y otros factores, y estas limitaciones se tienen en cuenta al diseñar y utilizar circuitos con op-amps.

### Amplificador Inversor

El amplificador inversor es un tipo de configuración de amplificador operacional (op-amp) muy común y ampliamente utilizado en circuitos electrónicos. La función principal del amplificador inversor es invertir la polaridad de la señal de entrada aplicada a su terminal de entrada, es decir, si la señal de entrada aumenta, la señal de salida disminuirá proporcionalmente, y viceversa.

La configuración básica del amplificador inversor consta de dos elementos principales: el amplificador operacional y dos resistencias. La señal de entrada se aplica al terminal de entrada no inversor (+) del amplificador operacional, mientras que el terminal de entrada inversor (-) está conectado a tierra o referencia de voltaje.

Aquí tienes el diagrama esquemático del amplificador inversor:

<div align="center">
  <img src="imagenes/imagen_47.png" width="400px">
</div>



Vin: Señal de entrada.
Vout: Señal de salida.
R1 y R2: Resistencias conectadas en la configuración de realimentación.
Vref: Referencia de voltaje (normalmente conectada a tierra).
La ganancia del amplificador inversor se calcula mediante la siguiente fórmula:

<div align="center">
  <img src="imagenes/imagen_48.png" width="400px">
</div>

Es importante notar que la ganancia será siempre positiva debido al valor absoluto en la fórmula. Sin embargo, como la señal se invierte, su polaridad será opuesta a la señal de entrada.

La configuración del amplificador inversor tiene varias aplicaciones en electrónica, como amplificación de señales, filtros activos, generadores de onda y más. Al elegir los valores de las resistencias R1 y R2, puedes ajustar la ganancia según tus necesidades específicas. Ten en cuenta que el valor de R2 generalmente es mayor que el valor de R1 para obtener una amplificación adecuada.







### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2023.07.31| Versión No. 1 | [Henry Moreno](https://github.com/hmorenom64)  |  6 |

_Curso Electronica Básica para Ingenieros es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [hmorenom64](https://github.com/hmorenom64?tab=repositories) en GitHub._

| [Anterior](diodos.md) | [:house: Inicio](../readme.md) | [:beginner: Ayuda / Colabora] | [Siguiente](tutorial_multisim.md) |
|----------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|-----------------------------------------|
                                                                                                                                      
                                                                                                                                
<div align="center"><a href="https://enlace-academico.escuelaing.edu.co/psc/FORMULARIO/EMPLOYEE/SA/c/EC_LOCALIZACION_RE.LC_FRM_ADMEDCO_FL.GBL" target="_blank"><img src="https://github.com/rcfdtools/R.TeachingResearchGuide/blob/main/CaseUse/.icons/IconCEHBotonCertificado.png" alt="R.LTWB" width="260" border="0" /></a></div>
                                                                                                                                      
##
