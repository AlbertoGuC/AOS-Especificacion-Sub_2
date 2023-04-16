# AOS-Especificacion-Sub_2

## Integrantes
- Alberto Guardiola Churiaque
- Álvaro Alonso Devesa 
- Omar Piñeiro Parada 
- Javier Rodríguez de Tujillo Landecho
- Alberto Rey Cristino

## Trabajo AOS 

# Guardado y gestión de los vehiculos de un cliente

Gestión de los vehículos que son propiedad de los clientes y que se reparan y/o revisan en el taller. Cada vehículo estará identificado de forma única por su VIN.<br> 

- VIN
- Marca
- Modelo
- Año
- Matrícula
- Fecha última intervención

# Despliegue 

Para desplegar un servidor mock y una UI con docker ejecutar el siguiente comando en la raíz del proyecto:

```
$ docker-compose up
```

Con los servicios desplegados, se puede acceder a una interfaz desde la que se puede revisar la especificación y realizar consultas al servidor mock. 
Se puede acceder desde el navegador en el siguiente URL: 'localhost:8000'.
