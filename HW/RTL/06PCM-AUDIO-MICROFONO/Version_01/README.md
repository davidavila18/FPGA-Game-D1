# SISTEMA DE AUDIO

## Integrantes del equipo de trabajo:

### 1 Lisseth Tatiana Herrera Rosero ltherreraro@unal.edu.co

### 2 Nombre1 nombre2 apelido1 apellido2 correo@electronico

### 3 Nombre1 nombre2 apelido1 apellido2 correo@electronico


## Descripción general del sistema: (tomado del documento de clase)

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

## Descripción de la caja Funcional  (in/out)

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

## Descripción funcional (Modulo Fpga):
En este modulo se tienen inicialmente dos submodulos: divisor de frecuencia y registros. El divisor de frecuencia es necesario para obtener los clocks de sincranizacion de el modulo de microfono y de altavoz, para esto se necesita un clock de entrada CLK, un clock de salida CLKOUT y un RESET de entrada para reiniciar el ciclo, adicionalmente se tienen dos parametros fijos la Fi que es la frecuencia del reloj de la Nexys 2 50MHZ y el Fo que es la Frecuencia de salida que se quiere. 

El modulo de la FPGA ademas de los submodulos tiene 4 entradas: 
* **di** que son los datos provenientes del microfono (conformado por 18 bits) 
* **INT** para inicializar (conformado por 1 bit)
* **W/R** para indicar si va a repoducir o grabar (conformado por 1 bit)
* **done** para indicar que finalizo la accion (conformado por 1 bit)

Finalmente este modulo tiene 3 salidas:
* **clkout** El clock que necesita el microfono para modular la señal y enviarla (conformado por 1 bit)
* **select** necesario mas adelante para seleccionar derecho o izquierdo (conformado por 1 bit)
* **do** la informacion de salida hacia el altavos (conformado por 16 bits)

<a href="https://ibb.co/fsxH2Q"><img src="https://preview.ibb.co/gXGo95/fpga.jpg" alt="fpga" border="0"></a>

## Descripción Estructural:


## Diagrama de Estados:

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

## Arquitectura del periférico:

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

## Diagrama de bloques del periférico:

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

## referencias:

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

