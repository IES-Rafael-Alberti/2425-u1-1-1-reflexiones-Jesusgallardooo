[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/Z6NE2ogx)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=16551485&assignment_repo_type=AssignmentRepo)
# Práctica 1: Introducción al desarrollo. Reflexiones.

Apoyate en los siguientes recursos para realizar la práctica:

[Descripción de la práctica](https://revilofe.github.io/section3/u01/practica/EDES-U1.-Practica010/)


---

# P 1.10: Reflexión y discusión sobre los resultados

## Identificación de la Actividad
- **ID de la Actividad:** 1.10
- **Módulo:** EDES
- **Unidad de Trabajo:** U1: Introducción al desarrollo de software 
- **Fecha de Creación:** 15/10/2024
- **Fecha de Entrega:** 20/10/2024
- **Alumno(s):** 
  - **Nombre y Apellidos:** Jesús  Gallardo Domínguez
  - **Correo electrónico:** jgaldom0701@g.educaand.es
  - **Iniciales del Alumno/Grupo:** JGD

## Descripción de la Actividad
Respuesta a una serie de preguntas, concretamente 40 preguntas, las cuales buscan reforzar y conseguir que adquiramos los conocimientos vistos en clases de la unidad 1: Introducción al desarrollo de software. Tocando detalladamente todos y cada uno de los puntos vistos en la unidad.  

# Preguntas

## 1. Relación de software y hardware


### 1.1 Primera parte


#### 1.1.1. ¿Cómo se ejecuta el código en el procesador? 

Primero, el procesador, en función del lenguaje en el que esté programado el código,  compilará o interpretará dicho código, para así convertirlo a 
lenguaje máquina. Tras traducirlo a lenguaje máquina, esta información se carga en la memoria RAM, desde la cual el procesador irá recibiendo instrucciones 
y ejecutándolas. Una vez estas instrucciones son ejecutadas, los resultados en caso de que los hubiese, los guardaríamos o veríamos en la salida.

#### 1.1.2. ¿Qué hace la memoria RAM con la información del botón o el LED? 

La RAM comprueba el estado tanto del botón como del LED, para saber si el botón se encuentra activo y si, por ende, el LED está encendido. almacena dicha información,y en caso de que dicha información cambiase, ordenará la instrucción de cambiar el estado del botón y del LED al procesador para así obtener el resultado que nos pedía nuestro programa. 

#### 1.1.3. ¿Cómo se comunican los periféricos (botón y LED) con el procesador? 

En nuestro caso, era una simulación con una placa arduino, por lo que existía una conexión física asignada a los pines correspondientes. Para comunicarse con el procesador, el cual comprueba el estado del botón y controla el estado del LED encendiéndolo o apagándolo según indique el botón.

### 1.2 Segunda parte



#### 1.2.1. ¿Cómo interactúan el procesador, la memoria y los periféricos en la ejecución del programa? 

La interacción consiste en la carga del programa/información en la memoria RAM, el procesador lee las instrucciones  que han sido recibidas de la RAM y las ejecuta realizando las funciones que estas indiquen, y cuando dicho programa ordene comunicarse con cualquier periférico, el procesador se encargará de comunicarse con él por los puertos de E/S, enviando o recibiendo datos según se necesite.

####  1.2.2. ¿Qué pasa con los datos en la memoria cuando el programa se ejecuta? 

Cuando ejecutamos un programa, primeramente se carga en la RAM, donde además se almacenarán los datos necesarios para ejecutarse. Una vez se cierra el programa, la memoria se vacía ya que así funciona la memoria RAM. 

####  1.2.3. ¿Qué roles juegan las instrucciones del software en esta interacción? 

Las instrucciones se encargan de que todo se ejecute correctamente, siguiendo lo que indican en su código. Controlan el funcionamiento del programa y la comunicación con los periféricos, coordinando así la ejecución y la interacción en el sistema.

####  1.2.4. ¿Cómo se relaciona esta simulación con lo que ocurre en un ordenador real? 

Pues al igual que ocurriría en un ordenador real, en esta simulación se ordenan ciertas instrucciones, se controlan ciertos procesos, y según el estado de los mismos se llevan a cabo o no las acciones necesarias para así realizar correctamente lo que se indica en las instrucciones del código. Esto mismo que ocurre en la práctica del botón y el LED, podría ocurrir en un ordenador real por ejemplo al pulsar una tecla de nuestro teclado y verla escrita en la pantalla.

## 2. Del código fuente al ejecutable¶


#### 2.1. ¿Cómo se diferencia el código fuente del código objeto y del ejecutable? 

El código fuente es el programa que escribe el programador utilizando un lenguaje de programación, normalmente fácilmente comprendido por los humanos, además no puede ser ejecutado directamente porque el ordenador no lo entendería.

El código objeto es una versión intermedia del código fuente. Este se obtiene tras compilar el programa, utilizando un compilador, el cual transforma el código fuente a un formato más cercano al lenguaje que la máquina esté más cerca de entender.

Y el código ejecutable es la versión final del programa y es aquel que sí que puede ser comprendido y leído por el ordenador para que pueda ejecutarlo directamente. En él se encuentra el mismo contenido que en el código fuente, solo que traducido a lenguaje máquina para que así el ordenador logre comprenderlo y ejecutarlo.


####  2.2. ¿Por qué el ordenador no puede entender el código fuente directamente? 

Porque este se encuentra escrito en un lenguaje de programación, el cual es familiar para el programador y no está en un formato adecuado para que el ordenador pueda entenderlo y ejecutarlo correctamente, para esto se necesita que el código que reciba el ordenador esté en lenguaje máquina, como es el caso del código ejecutable.


####  2.3. ¿Por qué es importante el paso de enlazado en la creación de programas? 

Es importante porque es el que se encarga de reunir todo lo necesario de nuestro programa en un solo archivo ejecutable, además de incluir a su vez las bibliotecas necesarias para que el programa funcione.

####  2.4. ¿Qué ocurre si falta alguna de las etapas (código objeto o ejecutable)? 

Si falta el código objeto, no podremos generar el código ejecutable y, por ende, no podríamos ejecutar nuestro programa de ninguna manera. En cambio si lo que falta es el código ejecutable, tampoco se podrá ejecutar el programa ya que es necesario que el archivo que lea nuestro ordenador esté en lenguaje máquina, y el único código que cumple este requisito es el ejecutable.

## 3. Generación de código intermedio

#### 3.1. ¿Cómo difiere el código intermedio del código ejecutable tradicional? 

Respuesta

####  3.2. ¿Por qué es útil tener una máquina virtual? 

Respuesta

####  3.3. ¿Qué ventajas ofrece el código intermedio? 

Respuesta

####  3.4. ¿Además de java, qué otros lenguajes usan máquinas virtuales? 

Respuesta

## 4. Lenguajes de programación


### 4.1 Primera parte


####  Compara el proceso de ejecución entre el lenguaje compilado y el interpretado. 


####   4.1.1. ¿Qué diferencias notaron en el proceso de compilación frente a la ejecución directa? 

Respuesta

####   4.1.2. ¿Qué pasa si hay un error de sintaxis en cada lenguaje? ¿Cuándo se detecta el error? 

Respuesta

### 4.2 Segunda parte


#### Compara un lenguaje de alto nivel con uno de bajo nivel.


#### 4.2.1. ¿Qué notaron sobre la abstracción entre los lenguajes de alto nivel y bajo nivel?

Respuesta

#### 4.2.2. ¿Qué ventajas y desventajas encontraron en cada uno?

Respuesta

### 4.3 Tercera parte



#### Compara un lenguaje orientado a objetos vs funcional.


#### 4.3.1. ¿Cómo funciona la organización de datos en Java usando objetos y métodos?

Respuesta

#### 4.3.2. ¿Cómo es diferente trabajar en un enfoque funcional en Python, usando solo funciones puras?      

Respuesta

### 4.4 Reflexión final

#### 4.4.1. ¿Qué lenguajes se sintieron más fáciles de usar? ¿Por qué?

Respuesta

#### 4.4.2. ¿En qué casos es preferible usar un lenguaje compilado frente a uno interpretado?

Respuesta

#### 4.4.3. ¿Cuándo es mejor usar un lenguaje de alto nivel en lugar de uno de bajo nivel?

Respuesta

#### 4.4.4. ¿Cómo se siente trabajar con el paradigma orientado a objetos en comparación con el imperativo o funcional?

Respuesta

## 5. Herramientas de desarrollo


### 5.1 Primera parte


#### Respecto a las proceso de creación de software identifica un conjunto de herramientas a usar.


#### 5.1.1. ¿Qué hace cada una de las herramientas?

Respuesta

#### 5.1.2. ¿Qué tipo de tareas facilita?

Respuesta

#### 5.1.3. ¿Qué características ofrece que la hacen única o diferente de otras herramientas similares?

Respuesta

#### 5.1.4. Elige una ¿Cómo es la experiencia de usuario al usarla? ¿Es fácil o compleja?

Respuesta

#### 5.1.5. Elige una ¿En qué situaciones sería ideal utilizar esta herramienta?

Respuesta

#### 5.1.6. Elige una ¿Qué limitaciones encontraste en la herramienta? 

Respuesta

### 5.2 Segunda parte


#### Céntrate en una herramienta dentro de la misma categoría y compárala con otras:


#### 5.2.1. ¿Qué herramienta se considera más útil y por qué?

Respuesta

#### 5.2.2. ¿Qué ventajas tiene una sobre la otra?ç

Respuesta

#### 5.2.3. ¿Cuál herramienta resultó ser la más intuitiva y por qué?

Respuesta

#### 5.2.4. ¿En qué casos se recomendaría usar un compilador en lugar de un intérprete?

Respuesta

#### 5.2.5. ¿Qué tipo de proyectos se beneficiarían más de un framework como Django?

Respuesta

### 5.3 Reflexión final


#### Con base en la experiencia de evaluación de las herramientas:


#### 5.3.1. ¿Cómo crees que impacta la elección de la herramienta en la calidad del software?

Respuesta

#### 5.3.2. ¿Qué características buscarías en una herramienta para facilitar tu flujo de trabajo?

Respuesta

#### 5.3.3. ¿Cómo cambió tu percepción de estas herramientas después de haberlas probado y evaluado? 

Respuesta

## Conclusiones
[Resumen de las conclusiones alcanzadas al desarrollar la actividad, las lecciones aprendidas, y posibles mejoras que se puedan implementar en futuras entregas.]

## Bibliografía


- https://revilofe.github.io/

- https://acortar.link/sfAjah

- https://acortar.link/nRaFB5


