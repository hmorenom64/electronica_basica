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



# **CURSO DE ELECTRONICA BASICA PARA INGENIEROS. MODULO 3. CONTROL DE MOTORES SERVOS**


## Montaje de un motor Servo paso a paso

Para controlar un motor servo grado por grado, necesitarás un microcontrolador o un dispositivo que pueda generar señales de control PWM (Modulación por Ancho de Pulso). Aquí hay una guía general sobre cómo hacerlo:

Materiales necesarios:

Motor servo: Asegúrate de tener un motor servo adecuado para tu proyecto, con el rango de grados de movimiento requerido.
Microcontrolador: Puedes utilizar un Arduino, Raspberry Pi u otro microcontrolador compatible con PWM.
Fuente de alimentación: Asegúrate de tener una fuente de alimentación adecuada para el motor servo.
Pasos para el control:

Conexión física: Conecta el motor servo al microcontrolador. Los servos tienen tres cables: uno para la alimentación (generalmente rojo), otro para el tierra (generalmente negro o marrón), y el tercero para el control de la señal (generalmente amarillo o blanco). Conecta el cable de señal a un pin de salida PWM en el microcontrolador.

Configuración del pin PWM: En el código de tu microcontrolador, asegúrate de configurar el pin de salida PWM que estás utilizando para controlar el motor servo.

Librerías: Si estás utilizando un Arduino u otra plataforma similar, es probable que existan librerías que simplifiquen el control del motor servo. Busca la librería correspondiente a tu modelo de microcontrolador y motor servo en particular.

Código de control: Escribe el código para controlar el motor servo. Utilizando la librería, normalmente deberás configurar el rango de grados que puede alcanzar el motor y luego enviar el valor deseado para mover el servo a un ángulo específico. Por ejemplo, si utilizas Arduino y la librería "Servo.h", podrías escribir algo como esto:


En este ejemplo, el servo se moverá de 0 a 90 grados y luego a 180 grados, con pausas de un segundo entre cada movimiento.

Ajuste fino: Dependiendo del modelo del servo y tus necesidades, es posible que debas ajustar los valores específicos de escritura para obtener la precisión deseada.

Espero que esta guía te haya sido útil. Recuerda siempre consultar la documentación de tu microcontrolador y del motor servo que estás utilizando para obtener información detallada sobre cómo controlarlos correctamente. ¡Buena suerte con tu proyecto!



```cpp
#include <Servo.h> 
 
Servo myservo;        // crea un objeto tipo servo para controlar el servo 
int pos ;          // variable para almacenar la posición del servo
 
void setup(){ 
  myservo.attach(7);  // En EduBasica el servo se conecta al pin 7 
}

void loop() 
{ 
 for (pos=10; pos<=180; pos+=10) { 
  myservo.write(pos); //orden con los grados en cada iteración
  delay(1000);
 }
}
```

## Taller de Evaluación

1. Implementar un esquema en el cual se entregue una rutina mediante una tabla, soobre diferentes posiciones y tiempos en los cuales debe
   permanecer en la posición. Es una simulación de un proceso de control por rutinas de movimiento
   
### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2023.07.31| Versión No. 1 | [Henry Moreno](https://github.com/hmorenom64)  |  6 |

_Curso Electronica Básica para Ingenieros es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [hmorenom64](https://github.com/hmorenom64?tab=repositories) en GitHub._

| [Anterior](../readme.md)| [:house: Inicio](../readme.md) | [:beginner: Ayuda / Colabora] | [Siguiente](control_step.md) |
