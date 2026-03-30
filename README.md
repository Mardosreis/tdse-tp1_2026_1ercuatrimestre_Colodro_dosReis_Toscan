# tdse-tp1_2026_1ercuatrimestre_Colodro_dosReis_Toscan
 FIUBA - Electrónica - Taller de Sistemas  Embebidos - Trabajo Práctico N°: 1 – Diagramas de  Estado - Modelado 
# FIUBA - Electrónica - Taller de Sistemas Embebidos 
## Trabajo Práctico N°: 1 - Diagramas de Estado - Modelado 
### 2026 - 1er Cuatrimestre - Grupo: Colodro, dos Reis y Toscan
### Responsable de la entrega: 
| Padrón | Apellidos, Nombres      | Fecha    | Deadline  | 
| 106433 | Colodro, Felipe         | :------: | :-------: | 
| 111545 | dos Reis, Mariana       |          | Semana 04 | 
| 111106 | Toscan, Uma             |          | Semana 04 |


Eventos y Acciones del módulo Sensor

EV_BTN_PRESSED: se genera cuando el botón pasa de estado no presionado a presionado (flanco ascendente).
EV_BTN_RELEASED: se genera cuando el botón pasa de estado presionado a no presionado (flanco descendente).

Estados del modelo
ST_BTN_RELEASED: botón en estado no presionado
ST_BTN_PRESSED: botón presionado

Timer
Se define un contador de tiempo asociado al sistema:

tick: contador incrementado cada 1 ms (período del sistema)

Acciones
Lectura del estado actual del botón mediante una entrada digital
Comparación con el estado anterior para detectar cambios de estado
Actualización del estado interno del sistema
Generación de eventos (EV_BTN_PRESSED / EV_BTN_RELEASED) en función de las transiciones detectadas
