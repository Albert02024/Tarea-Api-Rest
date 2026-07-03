# 🔐 API REST - Autenticación JWT, Roles y Permisos

<p align="center">

![Node.js](https://img.shields.io/badge/Node.js-22.x-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-Backend-000000?style=for-the-badge&logo=express)
![JWT](https://img.shields.io/badge/JWT-Autenticación-orange?style=for-the-badge&logo=jsonwebtokens)
![bcrypt](https://img.shields.io/badge/bcrypt-Seguridad-blue?style=for-the-badge)
![Swagger](https://img.shields.io/badge/Swagger-API%20Docs-85EA2D?style=for-the-badge&logo=swagger)
![Postman](https://img.shields.io/badge/Postman-Testing-FF6C37?style=for-the-badge&logo=postman)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

</p>

---

# 📚 Tabla de Contenidos

- [Descripción](#-descripción)
- [Objetivo](#-objetivo)
- [Características](#-características)
- [Tecnologías Utilizadas](#-tecnologías-utilizadas)
- [Arquitectura](#-arquitectura)
- [Instalación](#-instalación)
- [Variables de Entorno](#-variables-de-entorno)
- [Autenticación](#-autenticación)
- [Roles y Permisos](#-roles-y-permisos)
- [Endpoints](#-endpoints)
- [Documentación Swagger](#-documentación-swagger)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Autor](#-autor)

---

# 📖 Descripción

Esta aplicación consiste en una **API REST profesional** desarrollada con **Node.js** y **Express**, diseñada para gestionar el registro y autenticación de usuarios mediante **JSON Web Tokens (JWT)**.

La aplicación implementa mecanismos modernos de seguridad, control de acceso basado en roles, cifrado de contraseñas y documentación automática mediante Swagger.

---

# 🎯 Objetivo

Desarrollar una API REST segura que permita:

- Registrar nuevos usuarios.
- Iniciar sesión mediante autenticación JWT.
- Encriptar contraseñas utilizando bcrypt.
- Controlar el acceso mediante roles y permisos.
- Proteger rutas privadas utilizando middleware.
- Gestionar registros mediante operaciones CRUD.
- Documentar toda la API de forma interactiva mediante Swagger UI.

---

# 🚀 Características

✔ Registro de usuarios

✔ Inicio de sesión

✔ Autenticación mediante JWT

✔ Contraseñas encriptadas con bcrypt

✔ Middleware de autenticación

✔ Middleware de autorización por roles

✔ CRUD completo

✔ Validación de datos

✔ Manejo de errores

✔ Documentación Swagger

✔ Colección Postman

---

# 🛠 Tecnologías Utilizadas

| Tecnología | Uso |
|------------|-----|
| Node.js | Entorno de ejecución |
| Express.js | Framework Backend |
| JWT | Autenticación |
| bcrypt | Encriptación de contraseñas |
| Swagger UI | Documentación |
| Postman | Pruebas de la API |
| GitHub | Control de versiones |

---

# 🏗 Arquitectura

```
Cliente
    │
    ▼
Express Server
    │
    ├── Middleware JWT
    │
    ├── Middleware Roles
    │
    ├── Controladores
    │
    ├── Servicios
    │
    └── Base de Datos
```

---

# ⚙ Instalación

## Clonar el repositorio

```bash
git clone https://github.com/usuario/repositorio.git
```

Entrar al proyecto

```bash
cd repositorio
```

Instalar dependencias

```bash
npm install
```

Ejecutar el proyecto

```bash
npm run dev
```

---

# 🔑 Variables de Entorno

Crear un archivo `.env`

```env
PORT=3000

JWT_SECRET=tu_clave_super_secreta

DATABASE_URL=tu_base_de_datos
```

---

# 🔐 Autenticación

La autenticación se realiza mediante **JSON Web Token (JWT)**.

Una vez que el usuario inicia sesión correctamente, el servidor genera un Token que deberá enviarse en cada petición protegida.

Ejemplo:

```http
Authorization: Bearer eyJhbGciOiJIUzI1NiIsIn...
```

---

# 👥 Roles y Permisos

La API implementa autorización basada en roles.

Ejemplo:

| Rol | Permisos |
|------|-----------|
| Admin | Crear, Consultar, Actualizar y Eliminar |
| Usuario | Consultar información |

Los roles son validados mediante middleware antes de acceder a rutas protegidas.

---

# 📌 Endpoints

## Autenticación

| Método | Endpoint | Descripción |
|---------|----------|-------------|
| POST | /register | Registrar usuario |
| POST | /login | Iniciar sesión |

---

## Usuarios

| Método | Endpoint | Descripción |
|---------|----------|-------------|
| GET | /users | Obtener usuarios |
| GET | /users/:id | Obtener usuario |
| POST | /users | Crear usuario |
| PUT | /users/:id | Actualizar usuario |
| DELETE | /users/:id | Eliminar usuario |

---

# 📄 Documentación Swagger

La documentación interactiva está disponible en:

```
http://localhost:3000/api-docs
```

Desde Swagger es posible:

- Probar todos los endpoints.
- Autenticarse con JWT.
- Visualizar modelos de datos.
- Consultar respuestas del servidor.

---

# 📁 Estructura del Proyecto

```
src
│
├── controllers/
│
├── routes/
│
├── middlewares/
│
├── services/
│
├── models/
│
├── config/
│
├── docs/
│
├── utils/
│
└── app.js
```

---

# 🔒 Seguridad Implementada

- Contraseñas encriptadas con bcrypt.
- Tokens JWT.
- Middleware de autenticación.
- Middleware de autorización.
- Validación de entradas.
- Manejo centralizado de errores.

---

# 🧪 Pruebas

La API puede ser probada mediante:

- Swagger UI
- Postman

---

# 📌 Casos de Uso

✔ Registro de usuarios.

✔ Inicio de sesión.

✔ Validación del usuario.

✔ Consulta de registros.

✔ Creación de registros.

✔ Actualización de registros.

✔ Eliminación de registros.

✔ Acceso protegido mediante JWT.

✔ Validación de permisos según rol.

---

# 📖 Documentación

Toda la API se encuentra documentada mediante Swagger en:

```
/api-docs
```

La colección de pruebas también puede ser importada en **Postman**.

---

# 👨‍💻 Autor

**Desarrollado como proyecto académico de Backend**

API REST con autenticación JWT, bcrypt, middleware de seguridad, roles y permisos, siguiendo buenas prácticas de desarrollo y arquitectura REST.

---

<p align="center">
⭐ Si este proyecto te resultó útil, considera darle una estrella en GitHub.
</p>
