# Tarea1_estructura_de_datos
Tarea 1 - Sistema de Gestion Hospitalaria

1. Compilacion y ejecucion
Ingresar al link de replit enviado (en caso de no tener cuenta, crear una)

Para compilar, ejecutar el siguiente comando en la terminal (SHELL):
gcc tarea1.c tdas/extra.c tdas/heap.c tdas/list.c tdas/map.c -I tdas -o tarea1

Para ejecutar el programa ya compilado:
./tarea1



2. Opciones del menu

Al ejecutar el programa se muestra un menu con las siguientes opciones:

1) Registrar paciente
2) Asignar prioridad a paciente
3) Mostrar lista de espera
4) Atender al siguiente paciente
5) Mostrar pacientes por prioridad
6) Salir

Todas las opciones funcionan correctamente.

Opcion 1 permite registrar un paciente nuevo, ingresando su nombre. El id se asigna automaticamente de forma correlativa y se guarda la hora de ingreso.

Opcion 2 permite asignar una prioridad (1 alta, 2 media, 3 baja) a un paciente ya registrado, buscandolo por su id.

Opcion 3 muestra la lista completa de pacientes en espera, con su id, nombre, prioridad y hora de ingreso.

Opcion 4 atiende al paciente con mayor prioridad (el numero mas bajo es mas urgente). Si ningun paciente tiene prioridad asignada, se atiende al que lleva mas tiempo esperando.

Opcion 5 muestra los pacientes agrupados segun su nivel de prioridad.

Opcion 6 termina la ejecucion del programa y libera la memoria reservada.

No se detectaron opciones con errores ni comportamiento inesperado.

3. Ejemplo de interaccion

A continuacion se muestra un ejemplo de uso del programa.

Ingrese su opcion: 1
Registrar nuevo paciente
Ingrese nombre del paciente: Juan Perez
Paciente registrado con id 1 (ingreso: Mon Sep 7 10:32:00 2026)

Ingrese su opcion: 2
Ingrese el id del paciente: 1
Ingrese la nueva prioridad (1=alta, 2=media, 3=baja): 1
Prioridad actualizada para el paciente Juan Perez (id 1)

Ingrese su opcion: 3
Pacientes en espera:
ID: 1 | Nombre: Juan Perez | Prioridad: 1 | Ingreso: Mon Sep 7 10:32:00 2026

Ingrese su opcion: 4
Atendiendo a: Juan Perez (id 1, prioridad 1)

Ingrese su opcion: 3
Pacientes en espera:
(No hay pacientes registrados)

Ingrese su opcion: 6
Saliendo del sistema de gestion hospitalaria...
