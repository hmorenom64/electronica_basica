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

En este caso queremos que practiques la función for

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

### Control de versiones

| Versión    | Descripción   | Autor                                      | Horas |
|------------|:--------------|--------------------------------------------|:-----:|
| 2023.07.31| Versión No. 1 | [Henry Moreno](https://github.com/hmorenom64)  |  6 |

_Curso Electronica Básica para Ingenieros es de uso libre para fines académicos.

_¡Encontraste útil este repositorio!, apoya su difusión marcando este repositorio con una ⭐ o síguenos dando clic en el botón Follow de [hmorenom64](https://github.com/hmorenom64?tab=repositories) en GitHub._

| [Anterior](../readme.md)| [:house: Inicio](../readme.md) | [:beginner: Ayuda / Colabora] | [Siguiente](control_step.md) |
