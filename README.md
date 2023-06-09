# AOS-Especificacion-Sub_2 Grupo 7

## Integrantes
- Alberto Guardiola Churiaque
- Álvaro Alonso Devesa 
- Omar Piñeiro Parada 
- Javier Rodríguez de Tujillo Landecho
- Alberto Rey Cristino

# Enlace a repo Práctica 2: https://github.com/Omarpparada/AOS_Sub2_Implementaci-n
## Imagen de la implementación: omarpp/aos_vehiculos
## Trabajo AOS 

# Guardado y gestión de los vehiculos de un cliente

Gestión de los vehículos que son propiedad de los clientes y que se reparan y/o revisan en el taller. Cada vehículo estará identificado de forma única por su VIN.<br> 

- VIN
- Marca
- Modelo
- Fecha
- Matrícula
- Estado
- DNI

# Despliegue 

Para desplegar un servidor mock y una UI con docker ejecutar el siguiente comando en la raíz del proyecto:

```
$ docker-compose up
```

Con los servicios desplegados, se puede acceder a una interfaz desde la que se puede revisar la especificación y realizar consultas al servidor mock. 
Se puede acceder desde el navegador a Swagger con el siguiente URL: `localhost:8001` o `127.0.0.1:80`.  
En esa visualización se puede ver la especificación resultante de separar el fichero ***openapi.yaml*** usando **redocly split**.  

Hemos observado que al generar automáticamente los múltiples ficheros resultantes de la partición, los **schemas** no se ven reflejados en la especificación aún estando dentro de la carpeta schemas. 
Por este motivo hemos agregado otro servicio para poder ver la especificación original.  
El ***openapi.yaml*** completo se puede ver desde el navegador con la siguiente URL: `localhost:8000`, cambiando el puerto 8001 de la versión split por el 8000.

Para detener los servicios, presionar `Ctrl+C` o bien ejecutar en la raz 
```
$ docker compose down
```
Para hacer mocks de peticiones hemos usado  `HTTP Client` de Intellij. Estas pruebas se pueden encontrar en el fichero `http-requests.http`.
