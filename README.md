# BIMU Backend

Backend REST para BIMU, una aplicación cliente-servidor orientada a la gestión de rutas ciclistas y salidas grupales.

## Descripción

BIMU es un proyecto desarrollado como Trabajo de Fin de Grado (TFG) enfocado en la creación de una plataforma social para rutas ciclistas.

El backend proporciona una API REST encargada de gestionar usuarios, rutas, salidas grupales y funcionalidades sociales, utilizando una arquitectura cliente-servidor conectada con una aplicación Android.

## Tecnologías utilizadas

* Node.js
* Express.js
* MongoDB Atlas
* REST APIs
* Railway
* Java / Kotlin (cliente Android)

## Funcionalidades principales

* Registro y gestión de usuarios
* Creación y edición de rutas
* Sistema de salidas grupales
* Filtrado y búsqueda de rutas
* Persistencia de datos NoSQL
* Arquitectura cliente-servidor
* Gestión de perfiles y funcionalidades sociales

## Arquitectura

Aplicación Android ↔ API REST ↔ MongoDB Atlas

## Endpoints principales

### Usuarios

```http
POST /registerUser
PUT /editUser/:id
```

### Rutas

```http
POST /addRoute
PUT /editRoute/:id
DELETE /deleteRoute/:id
GET /routes/:id
POST /searchRoutes
```

## Ejecución local

### Clonar repositorio

```bash
git clone https://github.com/angel-orden/bimu-backend.git
```

### Instalar dependencias

```bash
npm install
```

### Ejecutar servidor

```bash
npm start
```

## Variables de entorno

Crear un archivo `.env` con las variables necesarias para la conexión con MongoDB Atlas.

Ejemplo:

```env
MONGO_URI=your_mongodb_connection
PORT=3000
```

## Deploy

Backend desplegado mediante Railway.

## Objetivos del proyecto

* Aplicar arquitectura cliente-servidor en una aplicación real
* Diseñar APIs REST para aplicaciones móviles
* Gestionar persistencia de datos con MongoDB Atlas
* Implementar funcionalidades sociales y gestión de rutas
* Mejorar conocimientos en backend y desarrollo full-stack

## Autor

Ángel Orden Rodríguez

* GitHub: [https://github.com/angel-orden](https://github.com/angel-orden)
* LinkedIn: [https://linkedin.com/in/ángel-orden-rodriguez](https://linkedin.com/in/ángel-orden-rodriguez)
