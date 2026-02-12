# Gateway Service - Pedidos Ya

Este microservicio actúa como el núcleo de gestión de datos maestros del sistema, manejando información sobre personas y su ubicación geográfica. Construido con **Nest.js**, proporciona una API robusta para la gestión de entidades de negocio.

## 📦 Funcionalidades

- **Gestión Geográfica**: Endpoints para administrar Países, Provincias y Ciudades.
- **Gestión de Personas**: CRUD completo para el registro y administración de personas.
- **Microservicios**: Diseñado para interactuar con otros servicios del ecosistema.
- **Base de Datos**: Integración con PostgreSQL mediante **TypeORM**.

## 🚀 Tecnologías

- **Nest.js** (v11)
- **TypeORM**
- **Axios** (para comunicación inter-service)
- **PostgreSQL**

## 🛠️ Instalación

```bash
npm install
```

## 🏃 Ejecución

```bash
# Desarrollo
npm run start:dev

# Producción
npm run start:prod
```

## 🧪 Pruebas

```bash
# unit tests
npm run test

# e2e tests
npm run test:e2e
```

## 🧬 Estructura del Código

- `src/entities/`: Definición de modelos de datos (Persona, Pais, Provincia, Ciudad).
- `src/persona/`: Lógica de negocio y controladores para la gestión de personas.
- `src/pais/`, `src/provincia/`, `src/ciudad/`: Módulos para la gestión geográfica.
- `src/base-service/`: Clases base para servicios y controladores, promoviendo la reutilización de código.

## 📡 Endpoints Principales

- `GET /persona`: Listado de personas registradas.
- `GET /pais`, `GET /provincia`, `GET /ciudad`: Endpoints de datos geográficos.

