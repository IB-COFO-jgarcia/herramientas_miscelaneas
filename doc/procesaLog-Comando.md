# procesaLog-Comando.html

- Proceso que lee las trazas del emulador de SCORT
    - seleccionando un fichero y lo vuelva en un text-area
    - copiando y pengando un fragmento en en text-area
- Recupera de las líneas "- [Comando]" el tiempo y el comando
    - comprueba el tiempo que tarda entre que pinta la traza de comando y la siguiente traza de respuesta del comando (si es que existe)
- Hace un listado de los comandos y los tiempos que han tardado
    - Pone el tiempo en rojo para los comandos que tarden 25 o más segundos (equivale a un time-out)
    - Calcula el total de comandos en el fichero y hace la media de tiempo
    - Por cada comando que tarde más de la media marca el tiempo en morado
- Finalmente agrega un resumen para indicar lo sucedido y muestra los comandos que han superado la media

![Ejemplo de ejecucion](/doc/image/sample-run-001.png)