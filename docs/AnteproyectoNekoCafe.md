# NekoCafé - Plataforma Web de Gestión para Cat Café

## Descripción

Aplicación web full-stack orientada a la gestión centralizada de un _cat café_ con espacio de acogida y adopción felina. Permite administrar de forma modular las reservas de clientes por turnos, el catálogo y estado básico de los gatos residentes, las solicitudes de adopción y la carta de productos de la cafetería desde una arquitectura desacoplada preparada para ampliar funcionalidades progresivamente.

## Objetivos y funcionalidades principales

- **Gestión de usuarios y roles:** Registro, inicio de sesión y control de acceso diferenciado entre clientes y administradores/personal.
- **Sistema de reservas por turnos:** Consulta de disponibilidad y creación/cancelación de reservas por fecha, franja horaria y número de personas.
- **Catálogo y fichas de gatos:** Listado de gatos residentes con información básica (descripción, edad, estado de adopción) y panel de administración para altas, bajas y modificaciones.
- **Solicitudes de adopción:** Formulario para que los usuarios registrados envíen solicitudes de adopción sobre un gato disponible y seguimiento básico de su estado.
- **Carta digital de cafetería:** Visualización de bebidas y productos disponibles con gestión de catálogo desde el panel de administración.

## Tecnologías, librerías y APIs previstas

- **Frontend:** Angular (TypeScript), Angular Router, Reactive Forms, Signals / RxJS y SCSS para una arquitectura basada en componentes reutilizables.
- **Backend:** Node.js, Express y TypeScript estructurado en capas (rutas, controladores, servicios y acceso a datos), utilizando un ORM tipado (Prisma o TypeORM) y validación de peticiones (Zod o express-validator).
- **Base de datos relacional:** PostgreSQL (o MySQL/MariaDB), garantizando integridad referencial mediante claves foráneas y una estructura de tablas normalizada y extensible.
- **Librerías y utilidades adicionales:** JWT y bcrypt para autenticación y cifrado de contraseñas; CORS y Helmet para seguridad HTTP; y posible integración futura de librerías de fechas (Day.js) o notificaciones por correo.

## Repositorio en GitHub y despliegue

- **Repositorio GitHub:** Organización modular del código (`frontend/` y `backend/`), control de versiones con ramas por funcionalidad y documentación básica de instalación (https://github.com/degarram/NekoCafe).
- **Despliegue (opcional):** Configuración mediante Docker y Docker Compose para levantar en local o en servidor los servicios de frontend, API REST y base de datos de forma aislada.
