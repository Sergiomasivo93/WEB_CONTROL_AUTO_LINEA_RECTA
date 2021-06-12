# Sistema de rectificación para conduccion en linea recta de vehiculos autonomos

La problematica que se aborda en este proyecto es el control de direccion sin desviaciones por oscilacion en el PWM del control del puente H para los motores de CC.
Se utilizo un protipo de auto y una SPA (single page application) diseñada para controlar sus direcciones. Ademas se midio la tension, corriente y RPM de los motores, en base a estos parametros se compenzó la diferencia de velocidades entre los motores modificando el ciclo de trabajo del PWM utilizado para controlar el movimiento de cada motor.

## Materiales
El proyeto fue implementado con Arduino UNO, modulo ESP8266, servoMotores y puente H ,
desarrollado en 5to año de la carrera ingenieria en computación en la catedra de Taller de proyectos II.

## Lbrerias y framework

Para el control y gestion de los datos producidos por el auto se implemento
un servido con flask y socket, para el almacenamiento de la informacion el dispositivo realiza un volcado sobre
una base de datos SQL con mariaDB engine.

Para el analisis y la logica de control de los motores de CC, la implementación se realizo mediante el IDE de arduino.

Como base de la solucion para la problematica si implemento la solucion mediante un sistema de control PID.
Es un mecanismo de control que a través de un lazo de retroalimentación permite regular la velocidad

El controlador PID calcula la diferencia entre nuestra variable real contra la variable deseada.
El algoritmo de control incluye tres parámetros fundamentales: Ganancia proporcional (P), Integral (I) y Derivativo (D).

Fuentes de investigación para la busqueda de la solución:

[Controladores PID, Virginia Mazzone](https://www.eng.newcastle.edu.au/~jhb519/teaching/caut1/Apuntes/PID.pdf)

[Sintonía de reguladores PID, Prof. Mª Jesús de la Fuente ](http://www.isa.cie.uva.es/~maria/pids.pdf)

[CONTROL PID UN ENFOQUE DESCRIPTIVO, Ing. Walter J. D. Cova](http://www.frlr.utn.edu.ar/archivos/alumnos/electronica/catedras/38-sistemas-de-control-aplicado/Publicaciones/Control_PID_Enfoque_Descriptivo.pdf)


## Desarrollado por:

| Linkedin | Repositorio |
| ------ | ------ |
| [Ailigo Oriana](https://www.linkedin.com/in/oriana-ailigo-80a2701a0/) | https://github.com/Oriailigo |
| [Aguilar Sergio](https://www.linkedin.com/in/sergioaguilarsoria/) | https://github.com/Sergiomasivo93 |
