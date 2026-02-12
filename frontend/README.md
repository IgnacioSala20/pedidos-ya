# Frontend - Pedidos Ya

Interfaz de usuario moderna y responsiva para el ecosistema de Pedidos Ya. Desarrollada con **Angular 20**, esta aplicación ofrece una experiencia de usuario fluida integrando seguridad y gestión de datos en tiempo real.

## ✨ Características Principales

- **Dashboard Dinámico**: Gestión de datos maestros con una interfaz intuitiva.
- **Autenticación Completa**: Vistas de Login, Registro y Recuperación de Contraseña integradas con el Auth Service.
- **Gestión de Sesión**: Implementación de interceptores para el manejo automático de tokens JWT y renovación de sesiones expiradas.
- **UI/UX Moderno**: Estilizado con **Tailwind CSS** y componentes interactivos.
- **Drag & Drop**: Integración de **Swapy** para componentes reposicionables.

## 🚀 Tecnologías

- **Angular 20**
- **Tailwind CSS**
- **Axios** (Cliente HTTP principal)
- **Swapy** (Interactividad visual)
- **Lucide Angular** (Iconografía)

## 🛠️ Instalación

```bash
npm install
```

## 🏃 Ejecución

```bash
# Servidor de desarrollo
npm run start
```

Navega a [http://localhost:4200](http://localhost:4200). La aplicación se recargará automáticamente ante cualquier cambio.

## 🧪 Pruebas

```bash
# Unit tests
npm run test
```

## 📂 Estructura del Proyecto

- `src/app/pages/`: Componentes de página (Login, Register, Home, etc.).
- `src/api/`: Configuración del cliente Axios e interceptores de seguridad.
- `src/app/services/`: Servicios globales como `api.service` y `global-status.service`.
- `src/app/config/`: Configuraciones de entorno y globales.

## 📡 Integración

La aplicación está configurada para conectarse por defecto a:
- **Auth Service**: `http://localhost:3001`
- **Gateway Service**: `http://localhost:3000`


```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
