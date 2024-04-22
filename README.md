# Aplicación de Gestión de Pacientes del Hospital

## Descripción

Esta aplicación en C permite a los usuarios gestionar la atención de pacientes en un hospital. Los usuarios pueden registrar nuevos pacientes, asignar prioridades, ver la lista de espera, atender al siguiente paciente y mostrar pacientes por prioridad. El objetivo es mejorar la eficiencia en la atención de los pacientes, asegurando que aquellos en situaciones críticas reciban atención lo más pronto posible.

## Cómo compilar y ejecutar

Dado que el sistema está diseñado para ser accesible y fácil de probar, se puede compilar y ejecutar en cualquier entorno de desarrollo de C compatible. Aquí tienes una guía rápida:

1. Clona este repositorio en tu máquina local.
2. Abre una terminal y navega hasta el directorio del repositorio clonado.
3. Compila el código utilizando un compilador de C compatible (por ejemplo, `gcc tdas/*.c main.c -Wno-unused-result -o main`).
4. Ejecuta el programa compilado (`./main`).


## Funcionalidades

### Funcionando correctamente:

**- Registrar Paciente**: Permite ingresar el nombre, edad y síntoma del paciente para registrarlo en la lista de espera.

**- Asignar Prioridad**: Permite asignar una nueva prioridad (Alto, Medio, Bajo) a un paciente registrado.

**- Mostrar Lista de Espera**: Muestra la lista de todos los pacientes registrados, junto con su información básica y hora de llegada.

**- Mostrar Paciente por prioridad** : Permite filtrar y mostrar los pacientes según su prioridad.

**- Atender Siguiente Paciente**: Atiende al siguiente paciente en la lista de espera, mostrando su información y hora de llegada.

### Problemas conocidos:

**- Asignar Prioridad**: Permite asignar una nueva prioridad (Alto, Medio, Bajo) a un paciente registrado. Cuando se asigna la prioridad, se modifica la prioridad del paciente, pero tambien se duplica el mismo paciente modificado. Creo que es un error en la aplicacion de funcion.

### A mejorar:

- Permitir ordenar por prioridad los pacientes mas que por orden de llegada.
- Permitir la edición de los datos de los pacientes.

## Ejemplo de uso

*Opcion 1 : Registre el paciente*
- 
Se mostrar un mensaje al momento de ingresar el dato requierido, en este caso:

```
Se le solicitaran los siguentes datos del paciente: Nombre, Edad y sintoma

Ingrese el nombre del paciente: Federico Rodriguez
Ingrese la edad del paciente: 20
Ingrese el síntoma del paciente: Vomitos con dolor de cabeza.
```


**El sistema registra a Federico Rodriguez con una prioridad inicial "Bajo" y guarda la hora actual de registro. La prioridad inicial puede ser ajustada más tarde basada en una evaluación médica más detallada.**


*Opcion 2 : Asignar Prioridad a un Paciente*
- 
Tras una evaluación inicial, el médico determina que el estado de Ana requiere atención prioritaria.
  
```
Lista de paciente:
Federico Rodriguez

Ingrese el nombre del paciente: Federico Rodriguez
Ingrese el nuevo nivel de prioridad (Alto, Medio, Bajo): Alto
```

*Opcion 3 : Lista de espera*
- 

El usuario revisa la lista de espera para ver todos los pacientes y sus prioridades.

```
Nombre: Federico Rodriguez
Edad: 20
Sintoma: Vomitos con dolor de cabeza.
Prioridad: Alto.
Hora de llegada : 21:56
```


*Opcion 4 : Atender Paciente*
-

```
Paciente atendido:
Nombre: Federico Rodriguez
Edad: 20
Sintoma: Lindo
Prioridad: Vomitos con dolor de cabeza.
Hora de llegada : 21:56

```



*Opcion 5 : Atender Paciente*
-

```
Ingrese el nivel de prioridad (Alto, Medio, Bajo):
Alto

Nombre: Federico Rodriguez
Edad: 20
Sintoma: Lindo
Prioridad: Vomitos con dolor de cabeza.
Hora de llegada : 21:56
```

## Contribuciones ##

**Vicente Martinez**:
- Desarrollo en solitario del codigo, juntos con las funciones.
