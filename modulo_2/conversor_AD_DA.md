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



# **CURSO DE ELECTRONICA BASICA PARA INGENIEROS. MODULO 2. CONVERORES A/D Y D/A**

## Conversión Digital / Análoga

Consiste en convertir un dato original que está en formato digital, para que a la salida se tenga un valor analógico (variable desde un Valor min hasta un Valor max

Por ejemplo, si tuviéramos dos datos de entrada en formato digital (0,1), mientras que el Valor min =0  y el Valor max= 3, tendríamos:

<div align="center">
  <img src="imagenes/im_85.png" width="500px">
</div>

### Módelo típico de Procesamiento de señales


<div align="center">
  <img src="imagenes/im_86.png" width="500px">
</div>

Para un sistema que tenga 4 datos de entrada, mientras que el umbral de salida estará entre 0 y 5 voltios, tenemos:

<div align="center">
  <img src="imagenes/im_87.png" width="500px">
</div>

<div align="center">
  <img src="imagenes/im_88.png" width="500px">
</div>

### Implementación Electrónica

<div align="center">
  <img src="imagenes/im_89.png" width="500px">
</div>

## Conversión Análoga / Diggital

La conversión analógica-digital (ADC) es el proceso de convertir una señal analógica en una señal digital. Las señales analógicas son continuas en el tiempo y pueden tomar cualquier valor dentro de un rango específico, mientras que las señales digitales son discretas, tomando valores específicos en intervalos de tiempo regulares.

La conversión analógica-digital se lleva a cabo en muchos dispositivos electrónicos modernos, como computadoras, teléfonos inteligentes, cámaras digitales, sensores, etc. Estos dispositivos generalmente operan con señales digitales, pero la mayoría de las señales en el mundo real son analógicas (por ejemplo, sonido, temperatura, voltaje, etc.). Por lo tanto, es necesario convertir estas señales analógicas en digitales para que puedan ser procesadas, almacenadas o transmitidas electrónicamente.

El proceso de conversión analógica-digital se realiza en dos etapas principales:

Muestreo: En esta etapa, la señal analógica se muestrea en intervalos regulares de tiempo. Se toman muestras de la señal analógica a intervalos específicos, y el valor de la señal en cada punto de muestreo se mantiene para su posterior procesamiento.

Cuantización: Después del muestreo, los valores analógicos de las muestras se cuantifican para representarlos con valores digitales discretos. La cuantización implica asignar un valor digital específico a cada muestra, generalmente usando una escala discreta, como bits (por ejemplo, 8, 16 o 24 bits).

La calidad de la conversión analógica-digital depende de la tasa de muestreo y la resolución de cuantización utilizadas. Una tasa de muestreo más alta y una mayor resolución resultarán en una representación digital más precisa de la señal analógica original.

Es importante destacar que durante este proceso de conversión, siempre existe una pérdida de información, ya que la señal analógica original se representa con una cantidad finita de valores digitales discretos. Esto se conoce como ruido de cuantización, que es un error inherente en el proceso de conversión.

En resumen, la conversión analógica-digital es una parte esencial de la electrónica y la informática modernas, permitiendo la manipulación y el procesamiento eficiente de señales del mundo real mediante dispositivos digitales.

### Conversión ADC por Rampa

Se genera una rampa a través de un contador, el cual va seguido de un DAC. La salida del DAC será una rampa (realmente es una escalera, presentando el ruido granular conocido en telecomunicaciones). Dicha rampa se compara con la señal de entrada, y si llega a ser mayor, frena el proceso de conteo, siendo la salida del contador la señal de salida digital

<div align="center">
  <img src="imagenes/im_90.png" width="500px">
</div>

El circuito implementado en Mutisim se observa a continuación:

<div align="center">
  <img src="imagenes/im_91.png" width="700px">
</div>


### Conversión ADC por aproximaciones sucesivas

Quizás el método de conversión A/D más ampliamente utilizado es el de las aproximaciones sucesivas. Tiene un tiempo de conversión mucho menor que la conversión de pendiente doble, aunque es más lento que el método flash. Asimismo, el tiempo de conversión es fijo para cualquier valor de la entrada analógica.

<div align="center">
  <img src="imagenes/im_92.png" width="700px">
</div>

<div align="center">
  <img src="imagenes/im_93.png" width="700px">
</div>

### Conversión ADC Flash

El método flash utiliza comparadores que comparan una serie de tensiones de referencia con la tensión de entrada analógica. Cuando la tensión  analógica sobrepasa a la tensión de referencia de un comparador determinado, se genera un nivel ALTO. La Figura siguiente presenta un convertidor de 3 bits que utiliza siete circuitos comparadores; no se necesita comparador para el caso de que todas las comparaciones sean cero.

En general, se requieren 2^(𝑛−1) comparadores para la conversión a un código binario de n bits. El número de bits empleado en un ADC es su resolución. Una de las desventajas del ADC flash es el gran número de comparadores necesarios para un número binario de tamaño razonable. Su principal ventaja es que tiene un tiempo de conversión rápido, gracias a su alta tasa de transferencia, la cual se mide en muestras por segundo.

<div align="center">
  <img src="imagenes/im_94.png" width="700px">
</div>

## Taller de Evaluación

1. Revisar las aplicaciones típicas de Arduino, para identifcar como funciona el conversor análogo digital. Posteriormente se debe implementar con un potenciometro un sistema de visualización de display 7 segmentos para mostrar en forma digital la señal de voltaje de entrada.

   
### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2023.07.31| Versión No. 1 | [Henry Moreno](https://github.com/hmorenom64)  |  6 |

_Curso Electronica Básica para Ingenieros es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [hmorenom64](https://github.com/hmorenom64?tab=repositories) en GitHub._

| [Anterior](logica_secuencial.md)| [:house: Inicio](../readme.md) | [:beginner: Ayuda / Colabora] | [Siguiente](microcontrol.md) |
|----------------------------|-----------------------------------|--------------------------------------------------------------------------------------------------|-----------------------------------------|
                                                                                                                                      
                                                                                                                                
<div align="center"><a href="https://enlace-academico.escuelaing.edu.co/psc/FORMULARIO/EMPLOYEE/SA/c/EC_LOCALIZACION_RE.LC_FRM_ADMEDCO_FL.GBL" target="_blank"><img src="https://github.com/rcfdtools/R.TeachingResearchGuide/blob/main/CaseUse/.icons/IconCEHBotonCertificado.png" alt="R.LTWB" width="260" border="0" /></a></div>
                                                                                                                                      
##
