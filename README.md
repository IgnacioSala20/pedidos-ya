# Pedidos Ya - Monorepo Project

Este es un proyecto de gestión integral desarrollado con una arquitectura de microservicios moderna, diseñado para demostrar habilidades en el desarrollo Full Stack y arquitectura de software. El sistema permite la gestión de usuarios, roles, permisos y datos maestros geográficos.

## 🚀 Arquitectura del Proyecto

El proyecto está organizado como un **monorepo** gestionado con **Turborepo**, lo que permite una gestión eficiente de dependencias y scripts de construcción entre los diferentes servicios y el frontend.

### Componentes Principales

1.  **Frontend**: Aplicación desarrollada en **Angular 20**, utilizando **Tailwind CSS** para un diseño moderno y responsivo. Se comunica con los microservicios mediante Axios.
2.  **Auth Service**: Microservicio en **Nest.js** encargado de la autenticación y autorización. Implementa seguridad con **JWT** (access y refresh tokens), control de acceso basado en roles (RBAC) y permisos.
3.  **Gateway Service**: Microservicio en **Nest.js** que actúa como punto central para la gestión de entidades de negocio (Persona, País, Provincia, Ciudad).

## 🛠️ Tecnologías Utilizadas

### Core
- **Node.js**: Entorno de ejecución de JavaScript.
- **Turborepo**: Orquestador de monorepo.
- **TypeScript**: Superset de JavaScript para tipado estático.

### Backend (Microservicios)
- **Nest.js**: Framework para aplicaciones de servidor eficientes y escalables.
- **TypeORM**: ORM para la interacción con la base de datos.
- **PostgreSQL**: Sistema de gestión de bases de datos relacionales.
- **JWT & Bcrypt**: Para autenticación segura y encriptación de contraseñas.

### Frontend
- **Angular 20**: Framework para aplicaciones web de una sola página (SPA).
- **Tailwind CSS**: Framework de CSS moderno para diseño rápido.
- **Axios**: Cliente HTTP para integración con APIs.

## 📋 Requisitos Previos

- [Node.js](https://nodejs.org/) (versión v18 o superior).
- [pnpm](https://pnpm.io/) o [npm](https://www.npmjs.com/).
- [PostgreSQL](https://www.postgresql.org/) corriendo localmente o en un contenedor.

## ⚙️ Instalación y Configuración

1.  Clonar el repositorio:
    ```bash
    git clone <url-del-repositorio>
    cd pedidos-ya
    ```

2.  Instalar dependencias globales del monorepo:
    ```bash
    npm install
    ```

3.  Configurar variables de entorno:
    Asegúrate de configurar las credenciales de base de datos en los archivos de configuración de `auth-service` y `gateway-service`.

## 🚀 Ejecución en Desarrollo

Para ejecutar todos los servicios simultáneamente en modo desarrollo utilizando Turborepo:

```bash
npm run dev
```

Esto iniciará:
- **Frontend**: [http://localhost:4200](http://localhost:4200)
- **Auth Service**: [http://localhost:3001](http://localhost:3001)
- **Gateway Service**: [http://localhost:3000](http://localhost:3000)

---

## 📂 Estructura del Repositorio

```text
pedidos-ya/
├── auth-service/     # Gestión de usuarios, roles y seguridad (Nest.js)
├── gateway-service/  # API de gestión de personas y geografía (Nest.js)
├── frontend/         # Interfaz de usuario (Angular 20)
└── package.json      # Configuración del monorepo y Turborepo
```
