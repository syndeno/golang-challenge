# Syndeno golang-challenge
Golang CLI Challenge

El objetivo de este desafío es implementar un caso de una herramienta de CLI en Golang empleando la librería de Cobra. En este proyecto inicial, se encuentra un proyecto de Cobra inicializado.
## Desafío
Se requiere implementar dos casos de CLI que se describen a continuación.

### Caso 1 - synctl dig [FQDN]

Este comando toma como parámetro un FQDN e intenta resolverlo recursivamente buscando un registro de tipo A o CNAME. Si no encuentra registro A, buscará un CNAME.

Opcionalmente, podrá solicitarse un debug de la resolución con el switch --verbose.

### Caso 2 - synctl connect [FQDN] [PROTOCOL]

Este comando tomará un FQDN y un PROTOCOL e intentará realizar una conexión TCP. El FQDN deberá emplear la resolución codificada en el Caso 1. El PROTOCOL podrá ser un valor numérico o una cadena de caracteres, en este último caso, se deberá buscar el número de puerto empleando el archivo de sistema de Linux /etc/services.

Una vez establecida la conexión, deberá ser posible interactuar con el servidor hasta que el usuario introduzca CTRL-C o el servidor remoto cierre la conexión.

## Modalidad de entrega
Para entregar la resolución del desafío, será necesario enviar el código en un archivo comprimido a emiliano.spinella@sydeno.com.


