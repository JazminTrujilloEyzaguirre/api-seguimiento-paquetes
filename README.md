# api-seguimiento-paquetes

Gestiona paquetes, estados y eventos de cambio de estado. Utiliza autenticación JWT y optimización de consultas

## Tabla de Contenidos
- [Descripción](#descripción)
- [Requisitos Técnicos](#requisitos-técnicos)
- [Instalación](#instalación)
- [Uso](#uso)
- [Contribución](#contribución)
- [Licencia](#licencia)

## Descripción
La aplicación XYZ es una API backend desarrollada en Node.js con Express.js y utiliza una base de datos MySQL para gestionar el seguimiento de paquetes de una empresa de envíos. Proporciona un conjunto de endpoints que permiten a los clientes y empleados consultar y actualizar el estado de los paquetes en tiempo real.

Características principales:

    Gestión de paquetes: Los clientes pueden crear y realizar seguimiento de sus paquetes mediante un número de seguimiento único.
    Estados de los paquetes: Cada paquete puede tener un estado asociado, como "En tránsito", "Entregado" o "Retenido en aduana".
    Registro de cambios: Se registra un historial de los cambios de estado de cada paquete, incluyendo la fecha y hora de cada cambio.
    Conexión cliente-paquete: Los paquetes están vinculados a clientes específicos, lo que permite a los clientes rastrear y gestionar sus propios paquetes.
    Autenticación y autorización: Se implementa un sistema de autenticación para permitir el acceso a ciertos endpoints y garantizar la seguridad de la información.

## Requisitos Técnicos
- Node.js
- Express.js
- MySQL

## Instalación
1. Clona este repositorio en tu máquina local.
2. Ejecuta el comando `npm install` para instalar las dependencias.
3. Configura las credenciales de la base de datos en el archivo `config/db.js`.
4. Ejecuta el comando `npm run start` para iniciar el servidor.

## Uso
- La API estará disponible en `http://localhost:3000`.
- Puedes utilizar herramientas como Postman o cURL para realizar las siguientes operaciones:

RUTAS:
- Crear un nuevo paquete: `POST http://localhost:3000/paquete`
- Actualizar un paquete: `PUT http://localhost:3000/paquete/:id`
- Eliminar un paquete: `DELETE http://localhost:3000/paquete/:id`
- Obtener todos los paquetes: `GET http://localhost:3000/paquete`
- Obtener un paquete por numero de seguimiento: `GET http://localhost:3000/paquete/:n_seguimiento`
- Crear un nuevo cliente: `POST http://localhost:3000/cliente`
- Actualizar un cliente: `PUT http://localhost:3000/cliente/:id`
- Eliminar un cliente: `DELETE http://localhost:3000/cliente/:id`
- Obtener todos los clientes: `GET http://localhost:3000/cliente`
- Obtener un cliente especifico: `GET http://localhost:3000/cliente/:id`

## Contribución

¡Contribuciones bienvenidas! Si deseas mejorar este proyecto o complementarlo con un frontend interactivo, siéntete libre de enviar un pull request. Antes de realizar cambios significativos, por favor, abre un issue para discutir los detalles y asegurarnos de estar en la misma página.

## Licencia
Este proyecto está licenciado bajo la Licencia MIT. Puedes ver informacion de la licencia [aquí](https://es.wikipedia.org/wiki/Licencia_MIT).
---
