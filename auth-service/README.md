# Auth Service - Pedidos Ya

Este microservicio se encarga de toda la lógica de seguridad, autenticación y gestión de usuarios del sistema. Construido con **Nest.js**, proporciona una base sólida y escalable para el control de acceso.

## 🔑 Funcionalidades

- **Autenticación JWT**: Implementación de tokens de acceso y tokens de refresco (Refresh Tokens) para una sesión segura y persistente.
- **Gestión de Usuarios**: Registro, login y perfil de usuario.
- **RBAC (Role-Based Access Control)**: Sistema de roles y permisos granulares para proteger los diferentes endpoints.
- **Seguridad**: Encriptación de contraseñas con **Bcrypt**.
- **Base de Datos**: Integración con PostgreSQL mediante **TypeORM**.

## 🚀 Tecnologías

- **Nest.js** (v11)
- **TypeORM**
- **Passport.js & JWT**
- **PostgreSQL**
- **Bcrypt**

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

# test coverage
npm run test:cov

# unit test con archivo específico
npm run test -- resource/roles/roles.controller.spec.ts 
```

## ⛁ Base de Datos y Migraciones

El servicio utiliza TypeORM para la gestión de la base de datos.

### Migraciones
```bash
# Generar migración
npm run migration:generate -- src/database/migrations/NombreMigracion

# Ejecutar migraciones
npm run migration:run
```

### Seeders (Población de datos)
Para inicializar la base de datos con datos por defecto (permisos, roles y usuarios administrador):
1. Rellenar los seeders en `src/database/seeders/sedeers/`.
2. Ejecutar:
```bash
npm run seed
```

## 🧬 Estructura del Código

- `src/database/core/`: Definición de entidades (User, Role, Permission).
- `src/jwt/`: Lógica de generación y validación de tokens.
- `src/middlewares/`: Decoradores y middlewares para control de permisos.
- `src/resource/`: Controladores y servicios para Usuarios, Roles y Permisos.

