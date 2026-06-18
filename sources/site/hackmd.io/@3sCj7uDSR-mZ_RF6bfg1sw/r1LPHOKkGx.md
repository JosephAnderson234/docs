# Source: https://hackmd.io/@3sCj7uDSR-mZ_RF6bfg1sw/r1LPHOKkGx

Table of Contents

[Documentación de endpoints por módulo](https://hackmd.io/#Documentación-de-endpoints-por-módulo) [Leyenda de estado](https://hackmd.io/#Leyenda-de-estado) [Resumen general](https://hackmd.io/#Resumen-general) [Convención de lectura](https://hackmd.io/#Convención-de-lectura) [Módulo auth](https://hackmd.io/#Módulo-auth) [Formato de respuesta de error](https://hackmd.io/#Formato-de-respuesta-de-error) [POST /auth/login](https://hackmd.io/#POST-authlogin) [POST /auth/refresh](https://hackmd.io/#POST-authrefresh) [GET /auth/me](https://hackmd.io/#GET-authme) [Resumen de contrato del módulo](https://hackmd.io/#Resumen-de-contrato-del-módulo) [Módulo users](https://hackmd.io/#Módulo-users) [Seguridad](https://hackmd.io/#Seguridad) [Formato de respuesta de error](https://hackmd.io/#Formato-de-respuesta-de-error31) [Endpoints](https://hackmd.io/#Endpoints) [Mapeo de casos de uso](https://hackmd.io/#Mapeo-de-casos-de-uso) [Notas](https://hackmd.io/#Notas) [Endpoints pendientes](https://hackmd.io/#Endpoints-pendientes) [Módulo activities](https://hackmd.io/#Módulo-activities) [Seguridad](https://hackmd.io/#Seguridad56) [Reglas de negocio aplicadas](https://hackmd.io/#Reglas-de-negocio-aplicadas) [Integración con Microsoft (Outlook Calendar / Teams)](https://hackmd.io/#Integración-con-Microsoft-Outlook-Calendar--Teams) [Formato de respuesta de error](https://hackmd.io/#Formato-de-respuesta-de-error59) [POST /activities](https://hackmd.io/#POST-activities) [GET /activities](https://hackmd.io/#GET-activities) [GET /activities/:id](https://hackmd.io/#GET-activitiesid) [PATCH /activities/:id](https://hackmd.io/#PATCH-activitiesid) [PATCH /activities/:id/complete](https://hackmd.io/#PATCH-activitiesidcomplete) [PATCH /activities/:id/cancel](https://hackmd.io/#PATCH-activitiesidcancel) [DELETE /activities/:id](https://hackmd.io/#DELETE-activitiesid) [Campos del response](https://hackmd.io/#Campos-del-response92) [Mapeo de casos de uso](https://hackmd.io/#Mapeo-de-casos-de-uso93) [Observaciones](https://hackmd.io/#Observaciones94) [Módulo contacts](https://hackmd.io/#Módulo-contacts) [Seguridad](https://hackmd.io/#Seguridad96) [Formato de respuesta de error](https://hackmd.io/#Formato-de-respuesta-de-error97) [POST /contacts](https://hackmd.io/#POST-contacts) [GET /contacts](https://hackmd.io/#GET-contacts) [GET /contacts/organization/:idOrganizacion](https://hackmd.io/#GET-contactsorganizationidOrganizacion) [GET /contacts/:id](https://hackmd.io/#GET-contactsid) [PATCH /contacts/:id](https://hackmd.io/#PATCH-contactsid) [Campos del response](https://hackmd.io/#Campos-del-response119) [Observaciones](https://hackmd.io/#Observaciones120) [Módulo integrations](https://hackmd.io/#Módulo-integrations) [Endpoints del controlador](https://hackmd.io/#Endpoints-del-controlador) [GET /microsoft/connect](https://hackmd.io/#GET-microsoftconnect) [GET /microsoft/callback](https://hackmd.io/#GET-microsoftcallback) [GET /microsoft/status](https://hackmd.io/#GET-microsoftstatus) [DELETE /microsoft/disconnect](https://hackmd.io/#DELETE-microsoftdisconnect) [Configuración de entorno](https://hackmd.io/#Configuración-de-entorno) [Observaciones](https://hackmd.io/#Observaciones145) [Módulo invitations](https://hackmd.io/#Módulo-invitations) [Formato de respuesta de error](https://hackmd.io/#Formato-de-respuesta-de-error147) [POST /invitations](https://hackmd.io/#POST-invitations) [GET /invitations](https://hackmd.io/#GET-invitations) [GET /invitations/info/:token](https://hackmd.io/#GET-invitationsinfotoken) [POST /invitations/accept](https://hackmd.io/#POST-invitationsaccept) [DELETE /invitations/:id](https://hackmd.io/#DELETE-invitationsid) [Proceso interno de expiración automática](https://hackmd.io/#Proceso-interno-de-expiración-automática) [Mapeo de casos de uso](https://hackmd.io/#Mapeo-de-casos-de-uso183) [Observaciones](https://hackmd.io/#Observaciones184) [Módulo leads](https://hackmd.io/#Módulo-leads) [Seguridad](https://hackmd.io/#Seguridad186) [Reglas de negocio aplicadas](https://hackmd.io/#Reglas-de-negocio-aplicadas187) [Formato de respuesta de error](https://hackmd.io/#Formato-de-respuesta-de-error188) [POST /leads](https://hackmd.io/#POST-leads) [GET /leads](https://hackmd.io/#GET-leads) [GET /leads/:id](https://hackmd.io/#GET-leadsid) [PATCH /leads/:id](https://hackmd.io/#PATCH-leadsid) [PATCH /leads/:id/status](https://hackmd.io/#PATCH-leadsidstatus) [DELETE /leads/:id](https://hackmd.io/#DELETE-leadsid) [Campos del response](https://hackmd.io/#Campos-del-response221) [Mapeo de casos de uso](https://hackmd.io/#Mapeo-de-casos-de-uso222) [Observaciones](https://hackmd.io/#Observaciones223) [Módulo notifications](https://hackmd.io/#Módulo-notifications) [Estado actual](https://hackmd.io/#Estado-actual) [Endpoints pendientes](https://hackmd.io/#Endpoints-pendientes226) [Observaciones](https://hackmd.io/#Observaciones227) [Módulo organizations](https://hackmd.io/#Módulo-organizations) [Formato de respuesta de error](https://hackmd.io/#Formato-de-respuesta-de-error229) [POST /organizations](https://hackmd.io/#POST-organizations) [GET /organizations](https://hackmd.io/#GET-organizations) [GET /organizations/sunat/:query](https://hackmd.io/#GET-organizationssunatquery) [GET /organizations/:id](https://hackmd.io/#GET-organizationsid) [PATCH /organizations/:id](https://hackmd.io/#PATCH-organizationsid) [Observaciones](https://hackmd.io/#Observaciones258) [Módulo quotations](https://hackmd.io/#Módulo-quotations) [Seguridad](https://hackmd.io/#Seguridad260) [Reglas de negocio aplicadas](https://hackmd.io/#Reglas-de-negocio-aplicadas261) [Formato de respuesta de error](https://hackmd.io/#Formato-de-respuesta-de-error262) [POST /quotations](https://hackmd.io/#POST-quotations) [GET /quotations](https://hackmd.io/#GET-quotations) [GET /quotations/:id](https://hackmd.io/#GET-quotationsid) [PATCH /quotations/:id](https://hackmd.io/#PATCH-quotationsid) [PATCH /quotations/:id/send](https://hackmd.io/#PATCH-quotationsidsend) [PATCH /quotations/:id/accept](https://hackmd.io/#PATCH-quotationsidaccept) [PATCH /quotations/:id/reject](https://hackmd.io/#PATCH-quotationsidreject) [DELETE /quotations/:id](https://hackmd.io/#DELETE-quotationsid) [Campos del response](https://hackmd.io/#Campos-del-response299) [Mapeo de casos de uso](https://hackmd.io/#Mapeo-de-casos-de-uso300) [Observaciones](https://hackmd.io/#Observaciones301) [Módulo reset\_password](https://hackmd.io/#Módulo-reset_password) [Formato de respuesta de error](https://hackmd.io/#Formato-de-respuesta-de-error303) [POST /reset-password/request](https://hackmd.io/#POST-reset-passwordrequest) [POST /reset-password/reset](https://hackmd.io/#POST-reset-passwordreset) [POST /reset-password/validate](https://hackmd.io/#POST-reset-passwordvalidate) [Mapeo de casos de uso](https://hackmd.io/#Mapeo-de-casos-de-uso329) [Proceso interno de expiración automática](https://hackmd.io/#Proceso-interno-de-expiración-automática330) [Módulo tokens](https://hackmd.io/#Módulo-tokens) [Estado actual](https://hackmd.io/#Estado-actual334) [Endpoints pendientes](https://hackmd.io/#Endpoints-pendientes335) [Observaciones](https://hackmd.io/#Observaciones336) [Módulos sin contrato HTTP visible](https://hackmd.io/#Módulos-sin-contrato-HTTP-visible) [Reglas de documentación para nuevos módulos](https://hackmd.io/#Reglas-de-documentación-para-nuevos-módulos) [Referencias útiles](https://hackmd.io/#Referencias-útiles) [Estado del documento](https://hackmd.io/#Estado-del-documento)

Untitled

[Edit](https://hackmd.io/@3sCj7uDSR-mZ_RF6bfg1sw/r1LPHOKkGx/edit?both)

[Edit](https://hackmd.io/@3sCj7uDSR-mZ_RF6bfg1sw/r1LPHOKkGx/edit?both)

- [Yiuseppe24](https://hackmd.io/@3sCj7uDSR-mZ_RF6bfg1sw)
 
 Last edited by [Yiuseppe24](https://hackmd.io/@3sCj7uDSR-mZ_RF6bfg1sw) on Jun 2, 2026
 
 [Linked with GitHub]()
 

Log in to edit or delete your comments and be notified of replies.

[Sign up](https://hackmd.io/join?return=true) [Already have an account? Log in]()

Comments

![](https://hackmd.io/new-comment-placeholder-dark.svg)There is no commentSelect some text and then click Comment, or simply add a comment to this page from below to start a discussion.

DiscardSend

# Documentación de endpoints por módulo

Este documento cataloga los endpoints del backend por módulo, siguiendo la organización hexagonal del proyecto. El objetivo es documentar lo que ya existe y marcar explícitamente lo que todavía está pendiente de exponer por HTTP.

## Leyenda de estado

- `Implementado`: el endpoint existe en el código actual.
- `Pendiente`: el módulo existe en dominio o aplicación, pero aún no expone controladores HTTP visibles.
- `Parcial`: hay parte de la API o de la infraestructura, pero no un contrato HTTP completo.

## Resumen general

| Módulo | Estado | Endpoints HTTP visibles |
| --- | --- | --- |
| `auth` | Implementado | `POST /auth/login`, `POST /auth/refresh`, `GET /auth/me` |
| `users` | Implementado | `GET /users`, `PATCH /users/:id/disable`, `PATCH /users/:id/enable` |
| `activities` | Implementado | `POST /activities`, `GET /activities`, `GET /activities/:id`, `PATCH /activities/:id`, `PATCH /activities/:id/complete`, `PATCH /activities/:id/cancel`, `DELETE /activities/:id` |
| `contacts` | Implementado | `POST /contacts`, `GET /contacts`, `GET /contacts/organization/:idOrganizacion`, `GET /contacts/:id`, `PATCH /contacts/:id` |
| `integrations` | Implementado | `GET /microsoft/connect`, `GET /microsoft/callback`, `GET /microsoft/status`, `DELETE /microsoft/disconnect` |
| `invitations` | Implementado | `POST /invitations`, `GET /invitations`, `GET /invitations/info/:token`, `POST /invitations/accept`, `DELETE /invitations/:id` |
| `leads` | Implementado | `POST /leads`, `GET /leads`, `GET /leads/:id`, `PATCH /leads/:id`, `PATCH /leads/:id/status`, `DELETE /leads/:id` |
| `notifications` | Pendiente | No hay controlador HTTP visible |
| `organizations` | Implementado | `POST /organizations`, `GET /organizations`, `GET /organizations/sunat/:query`, `GET /organizations/:id`, `PATCH /organizations/:id` |
| `quotations` | Implementado | `POST /quotations`, `GET /quotations`, `GET /quotations/:id`, `PATCH /quotations/:id`, `PATCH /quotations/:id/send`, `PATCH /quotations/:id/accept`, `PATCH /quotations/:id/reject`, `DELETE /quotations/:id` |
| `reset_password` | Implementado | `POST /reset-password/request`, `POST /reset-password/reset`, `POST /reset-password/validate` |
| `tokens` | Pendiente | No hay controlador HTTP visible |

## Convención de lectura

Cada módulo se documenta con esta estructura:

- Propósito del módulo.
- Endpoints reales, si existen.
- Endpoints pendientes o esperados, cuando todavía no hay API HTTP.
- Notas de seguridad o integración, si aplican.

## Módulo `auth`

Base path: `/auth`

El módulo de autenticación es el único módulo que hoy expone endpoints HTTP reales. Su función es resolver login, refresh y lectura del usuario autenticado.

### Formato de respuesta de error

Las respuestas que no son `200 OK` siguen el formato estándar de NestJS para excepciones HTTP.

#### `400 Bad Request`

Se produce cuando el body no cumple el DTO o cuando se envían campos no permitidos por el `ValidationPipe` global.

```
{
  "statusCode": 400,
  "message": [
    "correo must be an email",
    "property extraField should not exist"
  ],
  "error": "Bad Request"
}
```

#### `401 Unauthorized`

Se produce cuando las credenciales son inválidas, el refresh token no existe o un guard rechaza la petición.

```
{
  "statusCode": 401,
  "message": "No autorizado",
  "error": "Unauthorized"
}
```

#### `403 Forbidden`

Puede aparecer en rutas futuras protegidas por roles cuando el usuario autenticado no cumple el permiso requerido.

```
{
  "statusCode": 403,
  "message": "Forbidden resource",
  "error": "Forbidden"
}
```

#### Nota de consistencia

- En `login` y `refresh`, los errores de dominio se traducen normalmente a `401 Unauthorized`.
- En `GET /auth/me`, los errores del guard también se exponen como `401 Unauthorized` o `403 Forbidden`, según el origen.
- El formato exacto del arreglo de `message` en `400` depende de las validaciones activas en el DTO.

### `POST /auth/login`

Inicia sesión con correo y contraseña.

#### Request

Content-Type: `application/json`

```
{
  "correo": "usuario@dominio.com",
  "password": "123456"
}
```

#### Validaciones

- `correo` es obligatorio y debe tener formato de email.
- `password` es obligatorio.

#### Respuesta exitosa

HTTP `200 OK`

```
{
  "accessToken": "eyJhbGciOi...",
  "accessTokenExpiresIn": 900
}
```

#### Cookies emitidas

El backend setea una cookie `refreshToken` con estas características:

- `httpOnly: true`
- `sameSite: lax`
- `path: /auth/refresh`
- `secure: true` cuando `NODE_ENV=production`
- `maxAge: 7 días`

#### Errores posibles

- `401 Unauthorized` si las credenciales son inválidas.
- `401 Unauthorized` si el usuario no puede autenticarse.
- `400 Bad Request` si el body no cumple el DTO.

#### Observaciones

- El access token se devuelve en el body.
- El refresh token no se devuelve en JSON; viaja en cookie.
- El controller transforma errores de dominio a `UnauthorizedException` cuando corresponde.

### `POST /auth/refresh`

Renueva la sesión utilizando la cookie `refreshToken`.

#### Request

No requiere body.

La cookie esperada es `refreshToken`.

#### Respuesta exitosa

HTTP `200 OK`

```
{
  "accessToken": "eyJhbGciOi...",
  "accessTokenExpiresIn": 900
}
```

#### Cookies emitidas

Si el refresh token es válido, el backend vuelve a setear la cookie `refreshToken` con un valor rotado.

#### Errores posibles

- `401 Unauthorized` si no existe la cookie.
- `401 Unauthorized` si el refresh token es inválido o expiró.
- `401 Unauthorized` si el usuario ya no está autorizado.

#### Observaciones

- El endpoint depende de cookies, no de body.
- La cookie está restringida al path `/auth/refresh`.
- El refresh se rota en cada uso exitoso.

### `GET /auth/me`

Devuelve el usuario autenticado.

#### Headers requeridos

```
Authorization: Bearer <access-token>
```

#### Respuesta exitosa

HTTP `200 OK`

La respuesta serializa la instancia de `User` obtenida por el guard y el decorador `CurrentUser`.

Campos visibles en el modelo actual:

```
{
  "id": 1,
  "nombres": "Juan",
  "apellidos": "Pérez",
  "correo": "usuario@dominio.com",
  "password": "$2a$10$...",
  "created_at": "2026-05-19T00:00:00.000Z",
  "role": 1,
  "estado": 1,
  "updated_at": "2026-05-19T00:00:00.000Z"
}
```

#### Errores posibles

- `401 Unauthorized` si no se envía token.
- `401 Unauthorized` si el JWT es inválido o expiró.
- `401 Unauthorized` si el guard rechaza el usuario.

#### Observaciones

- El endpoint está protegido con `JwtAuthGuard`.
- El usuario se obtiene con `CurrentUser`.
- Si no se agrega serialización adicional, el campo `password` puede viajar en la respuesta.

### Resumen de contrato del módulo

| Endpoint | Estado | Descripción |
| --- | --- | --- |
| `POST /auth/login` | Implementado | Inicio de sesión |
| `POST /auth/refresh` | Implementado | Renovación de sesión |
| `GET /auth/me` | Implementado | Usuario autenticado |

## Módulo `users`

Base path: `/users`

El módulo `users` administra los usuarios del sistema. Actualmente expone el listado paginado con filtros y acciones de habilitar/deshabilitar usuarios. Solo accesible por usuarios con rol `ADMINISTRADOR`.

### Seguridad

- Todas las rutas requieren `JwtAuthGuard` y `RolesGuard`.
- Solo usuarios con rol `ADMINISTRADOR` pueden acceder.

### Formato de respuesta de error

#### `400 Bad Request`

```
{
  "statusCode": 400,
  "message": [
    "search must be a string",
    "page must not be less than 1"
  ],
  "error": "Bad Request"
}
```

#### `401 Unauthorized`

```
{
  "statusCode": 401,
  "message": "No autorizado",
  "error": "Unauthorized"
}
```

#### `403 Forbidden`

```
{
  "statusCode": 403,
  "message": "Forbidden resource",
  "error": "Forbidden"
}
```

#### `409 Conflict`

Se produce cuando se intenta deshabilitar la propia cuenta o cuando el usuario ya está en el estado solicitado.

```
{
  "statusCode": 409,
  "message": "Un administrador no puede deshabilitar su propia cuenta",
  "error": "Conflict"
}
```

### Endpoints

#### `GET /users`

Listado paginado de usuarios con filtros opcionales de búsqueda, rol y estado.

##### Query params

| Parámetro | Tipo | Obligatorio | Default | Descripción |
| --- | --- | --- | --- | --- |
| `search` | `string` | No | — | Búsqueda insensible a mayúsculas por nombre o correo electrónico |
| `role` | `UserRole` | No | — | Filtrar por rol (`ADMINISTRADOR`, `TRABAJADOR`) |
| `estado` | `UserState` | No | — | Filtrar por estado (`PENDIENTE`, `ACTIVO`, `SUSPENDIDO`) |
| `page` | `number` | No | `1` | Número de página (mínimo 1) |
| `limit` | `number` | No | `10` | Elementos por página (mínimo 1) |

##### Response `200 OK`

```
{
  "data": [
    {
      "id": 1,
      "nombres": "Juan",
      "apellidos": "Pérez",
      "correo": "juan@example.com",
      "rol": "TRABAJADOR",
      "estado": "ACTIVO",
      "fechaRegistro": "2026-01-15T10:30:00.000Z"
    }
  ],
  "meta": {
    "page": 1,
    "limit": 10,
    "total": 1,
    "totalPages": 1
  }
}
```

##### Campos del response

| Campo | Tipo | Descripción |
| --- | --- | --- |
| `data[].id` | `number` | ID del usuario |
| `data[].nombres` | `string` | Nombres del usuario |
| `data[].apellidos` | `string` | Apellidos del usuario |
| `data[].correo` | `string` | Correo electrónico |
| `data[].rol` | `string` | Rol del usuario (`ADMINISTRADOR` o `TRABAJADOR`) |
| `data[].estado` | `string` | Estado de la cuenta (`PENDIENTE`, `ACTIVO` o `SUSPENDIDO`) |
| `data[].fechaRegistro` | `string` (ISO 8601) | Fecha de creación del usuario |
| `meta.page` | `number` | Página actual |
| `meta.limit` | `number` | Elementos por página |
| `meta.total` | `number` | Total de usuarios que cumplen los filtros |
| `meta.totalPages` | `number` | Total de páginas |

##### Ejemplo de llamada

```
GET /users?search=juan&role=TRABAJADOR&estado=ACTIVO&page=1&limit=10
Authorization: Bearer <token>
```

#### `PATCH /users/:id/disable`

Suspende el acceso de un usuario al sistema. El usuario queda con estado `SUSPENDIDO`.

##### Seguridad

- Requiere `JwtAuthGuard` y `RolesGuard`.
- Solo rol `ADMINISTRADOR`.
- Un administrador no puede deshabilitarse a sí mismo (devuelve `409 Conflict`).

##### Parámetros de ruta

| Parámetro | Tipo | Obligatorio | Descripción |
| --- | --- | --- | --- |
| `id` | `number` | Sí | ID numérico del usuario a deshabilitar (mín. 1) |

##### Respuesta exitosa

HTTP `204 No Content` — sin body.

##### Errores posibles

- `401 Unauthorized` si no hay sesión válida.
- `403 Forbidden` si el usuario no es administrador.
- `404 Not Found` si el usuario no existe.
- `409 Conflict` si el administrador intenta deshabilitarse a sí mismo o el usuario ya está deshabilitado.

#### `PATCH /users/:id/enable`

Reactiva el acceso de un usuario al sistema. El usuario pasa a estado `ACTIVO`.

##### Seguridad

- Requiere `JwtAuthGuard` y `RolesGuard`.
- Solo rol `ADMINISTRADOR`.

##### Parámetros de ruta

| Parámetro | Tipo | Obligatorio | Descripción |
| --- | --- | --- | --- |
| `id` | `number` | Sí | ID numérico del usuario a habilitar (mín. 1) |

##### Respuesta exitosa

HTTP `204 No Content` — sin body.

##### Errores posibles

- `401 Unauthorized` si no hay sesión válida.
- `403 Forbidden` si el usuario no es administrador.
- `404 Not Found` si el usuario no existe.
- `409 Conflict` si el usuario ya está habilitado.

### Mapeo de casos de uso

| Caso de uso | Endpoint HTTP | Estado |
| --- | --- | --- |
| `GetAllUsersUseCase` | `GET /users` | Implementado |
| `DisableUserUseCase` | `PATCH /users/:id/disable` | Implementado |
| `EnableUserUseCase` | `PATCH /users/:id/enable` | Implementado |

### Notas

- La contraseña NUNCA se incluye en la respuesta.
- `fechaRegistro` corresponde a la fecha de creación del usuario (`createdAt` en base de datos).
- Los enums se devuelven como strings legibles, no como valores numéricos.

### Endpoints pendientes

| Endpoint | Estado | Nota |
| --- | --- | --- |
| `GET /users/:id` | Pendiente | Detalle de usuario |
| `POST /users` | Pendiente | Creación de usuario |
| `PATCH /users/:id` | Pendiente | Actualización parcial |
| `PATCH /users/:id/password` | Pendiente | Cambio de contraseña |

## Módulo `activities`

Base path: `/activities`

El módulo de actividades administra las interacciones comerciales asociadas a un Lead (reuniones, llamadas, emails u otras). Cada actividad pertenece a un Lead y a un Responsable, sigue un ciclo de estados (`PENDIENTE → REALIZADA` / `CANCELADA`) y soporta eliminación lógica (soft delete). Las notas de la actividad (`notas`) representan sus comentarios; no existe entidad separada de comentarios. Todas las rutas requieren autenticación JWT.

### Seguridad

- Todas las rutas requieren `JwtAuthGuard` (`@ApiBearerAuth()`).

### Reglas de negocio aplicadas

- La actividad debe estar asociada a un Lead existente y no eliminado (RN-001).
- El responsable (`idResponsable`) debe existir (RN-002).
- `fechaInicio` debe ser menor que `fechaFin` (RN-003).
- No se permite crear una actividad si el Lead ya tiene otra en estado `PENDIENTE` (RN-004).
- Toda actividad nueva inicia en estado `PENDIENTE` (RN-005).
- Estados válidos: `PENDIENTE`, `REALIZADA`, `CANCELADA` (RN-006).
- Una actividad `REALIZADA` o `CANCELADA` no puede volver a `PENDIENTE` ni cambiar de estado (RN-007, RN-008).
- La eliminación es lógica: marca `deletedAt` y los registros eliminados quedan excluidos de las consultas.

### Integración con Microsoft (Outlook Calendar / Teams)

Sincronización **unidireccional** CRM → Microsoft (nunca Microsoft → CRM). La actividad es la fuente de verdad.

- La sincronización es **opcional y explícita**: solo ocurre si el request incluye `syncWithMicrosoft: true`. Evita llenar calendarios con actividades internas que no requieren evento real.
- Si el responsable (`idResponsable`) **no** tiene Microsoft conectado, la actividad se crea normalmente con `outlookEventId: null` y `teamsMeetingUrl: null` (RN-MS-001).
- Solo las actividades de tipo `REUNION` con `createTeamsMeeting: true` generan una reunión de Teams (RN-MS-004). La reunión se crea dentro del propio evento de Outlook (`isOnlineMeeting`), en una sola llamada.
- Crear la reunión de Teams requiere una cuenta **work/school (Azure AD)** con licencia de Teams. Con cuentas personales de Microsoft el evento se crea pero `teamsMeetingUrl` viene `null`.
- Los errores de Microsoft **nunca** revierten ni bloquean la operación del CRM: se capturan, se registran en el log y la operación se reporta como exitosa (RN-MS-003).
- `PATCH /activities/:id` propaga `nombreActividad`, `fechaInicio`, `fechaFin` y `notas` al evento de Outlook solo si la actividad ya tiene `outlookEventId`.
- `PATCH /activities/:id/cancel` elimina el evento de Outlook asociado (si existe) y limpia `outlookEventId`/`teamsMeetingUrl`; `PATCH /activities/:id/complete` **no** interactúa con Microsoft.
- El evento/reunión se crea en el calendario del **responsable** (`idResponsable`), que es quien debe tenerlo en su Outlook.
- Los scopes de Graph se leen de la variable de entorno `MICROSOFT_SCOPES`; su valor por defecto ya incluye `Calendars.ReadWrite` y `OnlineMeetings.ReadWrite`. Las cuentas conectadas antes de habilitar estos scopes deben reconectarse para volver a consentir.

### Formato de respuesta de error

Los errores se serializan con el `GlobalExceptionFilter`, que añade `kind`, `path` y `timestamp` al payload.

#### `400 Bad Request`

DTO inválido, o fechas inválidas (`fechaInicio >= fechaFin`).

```
{
  "statusCode": 400,
  "error": "InvalidActivityDateException",
  "kind": "Validation",
  "message": "La fecha de inicio debe ser menor que la fecha de fin",
  "path": "/activities",
  "timestamp": "2026-05-31T10:30:00.000Z"
}
```

#### `404 Not Found`

Actividad, Lead o responsable inexistentes.

```
{
  "statusCode": 404,
  "error": "ActivityNotFoundException",
  "kind": "NotFound",
  "message": "Actividad con id 99 no encontrada",
  "path": "/activities/99",
  "timestamp": "2026-05-31T10:30:00.000Z"
}
```

#### `409 Conflict`

El Lead ya tiene una actividad pendiente (RN-004).

```
{
  "statusCode": 409,
  "error": "PendingActivityExistsException",
  "kind": "Conflict",
  "message": "El lead 1 ya tiene una actividad pendiente",
  "path": "/activities",
  "timestamp": "2026-05-31T10:30:00.000Z"
}
```

#### `422 / 400` por transición inválida

Completar o cancelar una actividad que no está `PENDIENTE` devuelve `400` con `InvalidActivityTransitionException`.

```
{
  "statusCode": 400,
  "error": "InvalidActivityTransitionException",
  "kind": "Validation",
  "message": "No se puede completar una actividad en estado REALIZADA",
  "path": "/activities/1/complete",
  "timestamp": "2026-05-31T10:30:00.000Z"
}
```

### `POST /activities`

Crea una nueva actividad. El estado inicial siempre es `PENDIENTE`.

#### Request

Content-Type: `application/json`

```
{
  "idLead": 1,
  "nombreActividad": "Llamada de seguimiento",
  "fechaInicio": "2026-06-01T10:00:00.000Z",
  "fechaFin": "2026-06-01T11:00:00.000Z",
  "tipo": "REUNION",
  "notas": "Confirmar detalles del proyecto",
  "idResponsable": 1,
  "syncWithMicrosoft": true,
  "createTeamsMeeting": true
}
```

#### Validaciones

| Campo | Tipo | Obligatorio | Longitud máx. | Notas |
| --- | --- | --- | --- | --- |
| `idLead` | `number` | Sí | — | Mín. 1; el Lead debe existir y no estar eliminado |
| `nombreActividad` | `string` | Sí | 90 | |
| `fechaInicio` | `string` (ISO 8601) | Sí | — | Debe ser menor que `fechaFin` |
| `fechaFin` | `string` (ISO 8601) | Sí | — | Debe ser mayor que `fechaInicio` |
| `tipo` | `enum` | Sí | — | `REUNION`, `LLAMADA`, `EMAIL`, `OTRO` |
| `notas` | `string` | No | 1000 | `null` si no se envía |
| `idResponsable` | `number` | Sí | — | Mín. 1; el usuario debe existir |
| `syncWithMicrosoft` | `boolean` | No | — | Default `false`. Si `true` y el responsable tiene Microsoft conectado, crea el evento en Outlook |
| `createTeamsMeeting` | `boolean` | No | — | Default `false`. Solo aplica a `tipo: REUNION` con `syncWithMicrosoft: true`; crea la reunión de Teams |

#### Respuesta exitosa (`201 Created`)

```
{
  "id": 1,
  "nombreActividad": "Llamada de seguimiento",
  "tipo": "LLAMADA",
  "estado": "PENDIENTE",
  "fechaInicio": "2026-06-01T10:00:00.000Z",
  "fechaFin": "2026-06-01T11:00:00.000Z",
  "notas": "Confirmar detalles del proyecto",
  "idLead": 1,
  "leadServicioInteres": "Consultoría en transformación digital",
  "leadEstado": "EN_PROSPECTO",
  "idResponsable": 1,
  "responsableName": "Carlos López",
  "outlookEventId": "AAMkAGI2...",
  "teamsMeetingUrl": "https://teams.microsoft.com/l/meetup-join/...",
  "createdAt": "2026-05-31T10:30:00.000Z",
  "updatedAt": "2026-05-31T10:30:00.000Z"
}
```

> Si el responsable no tiene Microsoft conectado (o `syncWithMicrosoft: false`), `outlookEventId` y `teamsMeetingUrl` vienen en `null`.

#### Errores posibles

- `400 Bad Request` si el DTO no cumple validaciones o `fechaInicio >= fechaFin`.
- `404 Not Found` si el Lead o el responsable no existen.
- `409 Conflict` si el Lead ya tiene una actividad pendiente.
- Un fallo de Microsoft **no** produce error: la actividad se crea igual con `outlookEventId`/`teamsMeetingUrl` en `null`.

### `GET /activities`

Lista actividades con filtros opcionales y paginación. Excluye los registros eliminados.

#### Query params

| Parámetro | Tipo | Obligatorio | Default | Descripción |
| --- | --- | --- | --- | --- |
| `idLead` | `number` | No | — | Filtra por Lead (mín. 1) |
| `idResponsable` | `number` | No | — | Filtra por responsable (mín. 1) |
| `estado` | `EstadoActividad` | No | — | `PENDIENTE`, `REALIZADA`, `CANCELADA` |
| `tipo` | `TipoActividad` | No | — | `REUNION`, `LLAMADA`, `EMAIL`, `OTRO` |
| `fechaInicio` | `string` (ISO 8601) | No | — | `fechaInicio` de la actividad ≥ a este valor |
| `fechaFin` | `string` (ISO 8601) | No | — | `fechaInicio` de la actividad ≤ a este valor |
| `page` | `number` | No | `1` | Número de página (mín. 1) |
| `limit` | `number` | No | `10` | Elementos por página (mín. 1) |

#### Respuesta exitosa (`200 OK`)

```
{
  "data": [
    {
      "id": 1,
      "nombreActividad": "Llamada de seguimiento",
      "tipo": "LLAMADA",
      "estado": "PENDIENTE",
      "fechaInicio": "2026-06-01T10:00:00.000Z",
      "fechaFin": "2026-06-01T11:00:00.000Z",
      "notas": "Confirmar detalles del proyecto",
      "idLead": 1,
      "leadServicioInteres": "Consultoría en transformación digital",
      "leadEstado": "EN_PROSPECTO",
      "idResponsable": 1,
      "responsableName": "Carlos López",
      "outlookEventId": null,
      "teamsMeetingUrl": null,
      "createdAt": "2026-05-31T10:30:00.000Z",
      "updatedAt": "2026-05-31T10:30:00.000Z"
    }
  ],
  "meta": {
    "page": 1,
    "limit": 10,
    "total": 1,
    "totalPages": 1
  }
}
```

#### Ejemplo de llamada

```
GET /activities?idLead=1&estado=PENDIENTE&tipo=LLAMADA&page=1&limit=10
Authorization: Bearer <token>
```

### `GET /activities/:id`

Obtiene el detalle de una actividad por su ID, incluyendo datos del Lead y del responsable. No retorna registros eliminados.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID numérico de la actividad |

#### Respuesta exitosa (`200 OK`)

Devuelve una actividad (misma estructura que un elemento de `data` en `GET /activities`).

#### Errores posibles

- `404 Not Found` si la actividad no existe o está eliminada.

### `PATCH /activities/:id`

Actualiza los campos de negocio de una actividad. Todos los campos son opcionales; solo se actualizan los enviados. No permite modificar `estado`, `lead`, `createdAt` ni `deletedAt`.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID numérico de la actividad |

#### Request

Content-Type: `application/json`

```
{
  "nombreActividad": "Reunión de cierre",
  "fechaFin": "2026-06-01T12:00:00.000Z"
}
```

#### Validaciones

Campos permitidos: `nombreActividad`, `fechaInicio`, `fechaFin`, `notas`, `idResponsable` (todos opcionales). Si se envía alguna fecha, la combinación resultante con la actual debe cumplir `fechaInicio < fechaFin`.

#### Respuesta exitosa (`200 OK`)

Devuelve la actividad actualizada (misma estructura que `GET /activities/:id`).

#### Errores posibles

- `400 Bad Request` si el DTO no cumple validaciones o las fechas resultantes son inválidas.
- `404 Not Found` si la actividad o el nuevo responsable no existen.

> Si la actividad tiene `outlookEventId`, los cambios de `nombreActividad`, `fechaInicio`, `fechaFin` y `notas` se propagan al evento de Outlook (fallo de Microsoft no bloquea la actualización).

### `PATCH /activities/:id/complete`

Marca la actividad como `REALIZADA`. Solo permitido desde `PENDIENTE` (RN-007). **No** interactúa con Microsoft.

#### Respuesta exitosa (`200 OK`)

Devuelve la actividad actualizada (misma estructura que `GET /activities/:id`).

#### Errores posibles

- `400 Bad Request` si la actividad ya está `REALIZADA` o `CANCELADA`.
- `404 Not Found` si la actividad no existe.

### `PATCH /activities/:id/cancel`

Marca la actividad como `CANCELADA`. Solo permitido desde `PENDIENTE` (RN-008).

#### Respuesta exitosa (`200 OK`)

Devuelve la actividad actualizada (misma estructura que `GET /activities/:id`).

#### Errores posibles

- `400 Bad Request` si la actividad ya está `CANCELADA` o `REALIZADA`.
- `404 Not Found` si la actividad no existe.

> Si la actividad tiene `outlookEventId`, se elimina el evento de Outlook y se limpian `outlookEventId`/`teamsMeetingUrl`. Un fallo de Microsoft no impide que la actividad quede `CANCELADA`.

### `DELETE /activities/:id`

Elimina lógicamente una actividad (soft delete): marca `deletedAt` sin borrar físicamente el registro.

#### Respuesta exitosa (`200 OK`)

```
{
  "ok": true
}
```

#### Errores posibles

- `404 Not Found` si la actividad no existe o ya estaba eliminada.

### Campos del response

| Campo | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID de la actividad |
| `nombreActividad` | `string` | Nombre de la actividad |
| `tipo` | `string` | Tipo (`REUNION`, `LLAMADA`, `EMAIL`, `OTRO`) |
| `estado` | `string` | Estado actual (`PENDIENTE`, `REALIZADA`, `CANCELADA`) |
| `fechaInicio` | `string` (ISO 8601) | Fecha y hora de inicio |
| `fechaFin` | `string` (ISO 8601) | Fecha y hora de fin |
| `notas` | `string | null` | Notas / comentarios de la actividad |
| `idLead` | `number` | ID del Lead asociado |
| `leadServicioInteres` | `string` | Servicio de interés del Lead (JOIN) |
| `leadEstado` | `string` | Estado del Lead (JOIN) |
| `idResponsable` | `number` | ID del usuario responsable |
| `responsableName` | `string` | Nombre completo del responsable (JOIN) |
| `outlookEventId` | `string | null` | ID del evento en Outlook si está sincronizada |
| `teamsMeetingUrl` | `string | null` | URL de la reunión de Teams si se generó |
| `createdAt` | `string` (ISO 8601) | Fecha de creación |
| `updatedAt` | `string` (ISO 8601) | Fecha de última actualización |

### Mapeo de casos de uso

| Caso de uso | Endpoint HTTP | Estado |
| --- | --- | --- |
| `CreateActivityUseCase` | `POST /activities` | Implementado |
| `ListActivitiesUseCase` | `GET /activities` | Implementado |
| `GetActivityByIdUseCase` | `GET /activities/:id` | Implementado |
| `UpdateActivityUseCase` | `PATCH /activities/:id` | Implementado |
| `CompleteActivityUseCase` | `PATCH /activities/:id/complete` | Implementado |
| `CancelActivityUseCase` | `PATCH /activities/:id/cancel` | Implementado |
| `DeleteActivityUseCase` | `DELETE /activities/:id` | Implementado |

### Observaciones

- Las `notas` de la actividad cumplen el rol de comentarios; no hay entidad separada.
- `leadServicioInteres`, `leadEstado` y `responsableName` se resuelven por JOIN; el frontend no necesita llamadas adicionales.
- El filtro por fechas (`fechaInicio`, `fechaFin`) acota la `fechaInicio` de las actividades a ese rango.
- Los registros con `deletedAt` distinto de `null` quedan excluidos de todas las consultas.
- La sincronización con Outlook/Teams se consume vía el puerto `CALENDAR_SYNC` que exporta el módulo `integrations`; la capa Activity nunca conoce Microsoft Graph directamente (arquitectura hexagonal).
- Secuencias de seguimiento, recordatorios, plantillas de correo y notificaciones siguen siendo módulos aún no expuestos por HTTP.

## Módulo `contacts`

Base path: `/contacts`

El módulo de contactos administra personas asociadas a organizaciones. Permite registrar, listar, consultar y actualizar contactos, con soporte para vocativos, correos múltiples y estado de correo. Todas las rutas requieren autenticación JWT.

### Seguridad

- Todas las rutas requieren `JwtAuthGuard`.
- El `idAuthor` se obtiene automáticamente del usuario autenticado (`@CurrentUser()`), no del body de la petición.

### Formato de respuesta de error

#### `400 Bad Request`

```
{
  "statusCode": 400,
  "message": [
    "correo must be an email",
    "nombres must be a string"
  ],
  "error": "Bad Request"
}
```

#### `401 Unauthorized`

```
{
  "statusCode": 401,
  "message": "No autorizado",
  "error": "Unauthorized"
}
```

#### `404 Not Found`

```
{
  "statusCode": 404,
  "message": "Contacto no encontrado",
  "error": "Not Found"
}
```

#### `409 Conflict`

```
{
  "statusCode": 409,
  "message": "El correo electrónico ya existe",
  "error": "Conflict"
}
```

### `POST /contacts`

Registra un nuevo contacto.

#### Request

Content-Type: `application/json`

```
{
  "nombres": "Juan",
  "apellidos": "Pérez",
  "vocativo": "SR",
  "cargo": "Gerente Comercial",
  "correo": "juan.perez@empresa.com",
  "telefono": "+51 987654321",
  "correo2": "jperez.personal@gmail.com",
  "comentarios": "Interesado en servicios de I+D",
  "idOrganizacion": "123e4567-e89b-12d3-a456-426614174000"
}
```

#### Validaciones

| Campo | Tipo | Obligatorio | Longitud máx. | Notas |
| --- | --- | --- | --- | --- |
| `nombres` | `string` | Sí | 90 | |
| `apellidos` | `string` | No | 90 | `null` si no se envía |
| `vocativo` | `enum` | No | — | Valores: `SR`, `SRA`, `SRTA` |
| `cargo` | `string` | No | 120 | `null` si no se envía |
| `correo` | `email` | Sí | 254 | Único en el sistema |
| `telefono` | `string` | No | 20 | `null` si no se envía |
| `correo2` | `email` | No | 254 | Único en el sistema |
| `comentarios` | `string` | No | 500 | `null` si no se envía |
| `idOrganizacion` | `string` (UUID) | Sí | — | Organización a la que pertenece |

#### Respuesta exitosa (`201 Created`)

```
{
  "id": 1,
  "nombres": "Juan",
  "apellidos": "Pérez",
  "vocativo": "SR",
  "cargo": "Gerente Comercial",
  "correo": "juan.perez@empresa.com",
  "telefono": "+51 987654321",
  "correo2": "jperez.personal@gmail.com",
  "comentarios": "Interesado en servicios de I+D",
  "idOrganizacion": "123e4567-e89b-12d3-a456-426614174000",
  "organizacionNombre": "Bioactiva SAC",
  "idAuthor": 3,
  "estado_correo": "VIGENTE",
  "createdAt": "2025-05-27T12:00:00.000Z"
}
```

### `GET /contacts`

Lista todos los contactos registrados.

#### Respuesta exitosa (`200 OK`)

```
[
  {
    "id": 1,
    "nombres": "Juan",
    "apellidos": "Pérez",
    "vocativo": "SR",
    "cargo": "Gerente Comercial",
    "correo": "juan.perez@empresa.com",
    "telefono": "+51 987654321",
    "correo2": "jperez.personal@gmail.com",
    "comentarios": "Interesado en servicios de I+D",
    "estado_correo": "VIGENTE",
    "idOrganizacion": "123e4567-e89b-12d3-a456-426614174000",
    "organizacionNombre": "Bioactiva SAC",
    "idAuthor": 3,
    "createdAt": "2025-05-27T12:00:00.000Z"
  }
]
```

### `GET /contacts/organization/:idOrganizacion`

Consulta los contactos filtrados por organización.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `idOrganizacion` | `string` (UUID) | UUID de la organización |

#### Respuesta exitosa (`200 OK`)

Devuelve un array de contactos pertenecientes a la organización (misma estructura que `GET /contacts`).

### `GET /contacts/:id`

Obtiene el detalle de un contacto específico por su ID.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID numérico del contacto |

#### Respuesta exitosa (`200 OK`)

```
{
  "id": 1,
  "nombres": "Juan",
  "apellidos": "Pérez",
  "vocativo": "SR",
  "cargo": "Gerente Comercial",
  "correo": "juan.perez@empresa.com",
  "telefono": "+51 987654321",
  "correo2": "jperez.personal@gmail.com",
  "comentarios": "Interesado en servicios de I+D",
  "estado_correo": "VIGENTE",
  "idOrganizacion": "123e4567-e89b-12d3-a456-426614174000",
  "organizacionNombre": "Bioactiva SAC",
  "idAuthor": 3,
  "createdAt": "2025-05-27T12:00:00.000Z"
}
```

### `PATCH /contacts/:id`

Actualiza los datos de un contacto existente. Todos los campos son opcionales; solo se actualizan los campos enviados.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID numérico del contacto |

#### Request

Content-Type: `application/json`

```
{
  "nombres": "Juan Carlos",
  "cargo": "Director Comercial"
}
```

#### Validaciones

Mismas validaciones que `POST /contacts`, pero todos los campos son opcionales. El campo `idOrganizacion` también es opcional en actualización.

#### Respuesta exitosa (`200 OK`)

Devuelve el contacto actualizado (misma estructura que `GET /contacts/:id`).

### Campos del response

| Campo | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID del contacto |
| `nombres` | `string` | Nombres del contacto |
| `apellidos` | `string | null` | Apellidos del contacto |
| `vocativo` | `string | null` | Tratamiento (`SR`, `SRA`, `SRTA`) |
| `cargo` | `string | null` | Cargo en la organización |
| `correo` | `string` | Correo electrónico principal |
| `telefono` | `string | null` | Teléfono de contacto |
| `correo2` | `string | null` | Correo electrónico secundario |
| `comentarios` | `string | null` | Comentarios adicionales |
| `estado_correo` | `string` | Estado del correo (`VIGENTE`, `VENCIDO`) |
| `idOrganizacion` | `string` (UUID) | ID de la organización asociada |
| `organizacionNombre` | `string` | Nombre de la organización asociada |
| `idAuthor` | `number` | ID del usuario que creó el contacto |
| `createdAt` | `string` (ISO 8601) | Fecha de creación del contacto |

### Observaciones

- El estado de correo (`estado_correo`) se inicializa como `VIGENTE` al crear el contacto. Valores posibles: `VIGENTE`, `VENCIDO`.
- El `vocativo` puede ser `SR`, `SRA` o `SRTA`.
- Los campos `correo` y `correo2` son únicos a nivel de base de datos.
- La autoría (`idAuthor`) se obtiene del token JWT, no del body.
- `organizacionNombre` se obtiene mediante un JOIN con la tabla `Organizacion` (no requiere llamada adicional del frontend).
- El campo `updatedAt` no se incluye en la respuesta.

## Módulo `integrations`

El módulo de integraciones actualmente solo expone el sub-módulo **Microsoft Integration**, que implementa OAuth2 Authorization Code Flow para conectar cuentas Microsoft (Outlook, Azure AD).

### Endpoints del controlador

Base path: `/microsoft`

| Método | Ruta | Auth | Descripción |
| --- | --- | --- | --- |
| `GET` | `/microsoft/connect` | JWT | Retorna la URL de autorización de Microsoft para iniciar el flujo OAuth |
| `GET` | `/microsoft/callback` | Público | Callback OAuth de Microsoft; redirige al frontend con resultado |
| `GET` | `/microsoft/status` | JWT | Retorna el estado de conexión del usuario autenticado |
| `DELETE` | `/microsoft/disconnect` | JWT | Desconecta la cuenta Microsoft del usuario autenticado |

---

### `GET /microsoft/connect`

Genera la URL de autorización de Microsoft para iniciar el flujo OAuth.

#### Seguridad

- Requiere JWT.
- No requiere rol específico.

#### Respuesta exitosa

HTTP `200 OK`

```
{
  "url": "https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=..."
}
```

#### Errores posibles

- `401 Unauthorized` si no hay JWT.

#### Observaciones

- La URL contiene el `state` con el `userId` para identificar al usuario al regresar del callback.
- Los scopes solicitados se configuran vía `MICROSOFT_SCOPES` (por defecto: `User.Read, Mail.Read, Mail.Send`).

---

### `GET /microsoft/callback`

Endpoint público que recibe el código de autorización de Microsoft y lo canjea por tokens.

#### Seguridad

- No requiere JWT.
- Es público por diseño (Microsoft redirige aquí sin autenticación previa).

#### Query parameters

| Parámetro | Tipo | Obligatorio | Descripción |
| --- | --- | --- | --- |
| `code` | `string` | Sí | Código de autorización de Microsoft |
| `state` | `string` | Sí | `{userId}:{uuid}` — contiene el ID del usuario que inició el flujo |
| `client_info` | `string` | No | Enviado por Microsoft, ignorado por el backend |
| `clientdata` | `string` | No | Enviado por Microsoft, ignorado por el backend |

#### Comportamiento

1. Recibe `code` y `state` de Microsoft.
2. Extrae `userId` del `state` (formato `{userId}:{uuid}`).
3. Canjea el código por tokens con MSAL.
4. Almacena `refreshToken` y `tokenExpiresAt` en la base de datos.

#### Redirección exitosa

```
HTTP 302 → FRONTEND_URL/ajustes?microsoft=connected
```

#### Redirección en error

```
HTTP 302 → FRONTEND_URL/ajustes?microsoft=error
```

#### Posibles causas de error

- `code` o `state` faltantes.
- `state` no contiene `userId` válido.
- El código de autorización expiró o ya fue canjeado.
- Error de red con Microsoft.

#### Observaciones

- El `state` se divide por `:` y la primera parte se parsea como `userId` numérico.
- No hay response JSON; siempre redirige al frontend.

---

### `GET /microsoft/status`

Retorna si el usuario autenticado tiene una cuenta Microsoft conectada.

#### Seguridad

- Requiere JWT.

#### Respuesta exitosa (`200 OK`)

```
{
  "connected": true
}
```

```
{
  "connected": false
}
```

#### Errores posibles

- `401 Unauthorized` si no hay JWT.

---

### `DELETE /microsoft/disconnect`

Elimina la conexión Microsoft del usuario autenticado.

#### Seguridad

- Requiere JWT.

#### Respuesta exitosa

HTTP `200 OK`

```
{
  "ok": true
}
```

#### Errores posibles

- `401 Unauthorized` si no hay JWT.
- `404 Not Found` si el usuario no tiene una conexión activa (lanza `MicrosoftIntegrationNotFoundException`).

---

### Configuración de entorno

| Variable | Descripción | Obligatorio |
| --- | --- | --- |
| `AZURE_CLIENT_ID` | Client ID de la app en Azure AD | Sí |
| `AZURE_TENANT_ID` | Tenant ID (`common` para multi-tenant) | Sí |
| `AZURE_CLIENT_SECRET` | Client Secret de la app en Azure AD | Sí |
| `MICROSOFT_REDIRECT_URI` | URL de callback registrada en Azure AD | Sí |
| `MICROSOFT_SCOPES` | Scopes separados por espacio. Default: `openid profile email offline_access User.Read Calendars.ReadWrite OnlineMeetings.ReadWrite` (incluye los necesarios para sincronizar actividades con Outlook/Teams) | No |
| `FRONTEND_URL` | URL base del frontend (para redirección post-callback) | No (default: `http://localhost:3120`) |

### Observaciones

- Este módulo implementa OAuth2 Authorization Code Flow con MSAL v3.
- Los tokens de acceso no se almacenan; se obtienen bajo demanda mediante refresh token.
- El refresh token y su expiración se guardan en la tabla `IntegracionMicrosoft`.
- Expone el puerto `CALENDAR_SYNC` (sincronización CRM → Outlook Calendar / Teams) que consume el módulo `activities`. El adaptador resuelve el token del usuario y delega en Microsoft Graph. La reunión de Teams se crea como parte del evento (`POST /me/events` con `isOnlineMeeting`), no vía `/me/onlineMeetings`. Ningún otro módulo conoce Graph directamente.
- Crear reuniones de Teams requiere una cuenta **work/school (Azure AD)** con licencia de Teams; con cuentas personales el evento de Outlook se crea pero sin link de Teams.
- Si `AZURE_TENANT_ID` se configura como UUID de un tenant específico, los usuarios con cuentas Microsoft personales ([outlook.com](http://outlook.com), [hotmail.com](http://hotmail.com)) no podrán autenticarse. Usar `common` para soportar cualquier cuenta Microsoft.

## Módulo `invitations`

Base path: `/invitations`

El módulo de invitaciones ya expone un contrato HTTP completo para crear, listar, consultar, aceptar y revocar invitaciones. El dominio está modelado con `InvitationToken` y el controller aplica seguridad por JWT y roles en las rutas administrativas.

### Formato de respuesta de error

Las rutas protegidas siguen el mismo estilo de NestJS que el resto del backend:

#### `400 Bad Request`

Se produce cuando el DTO no cumple las validaciones o cuando la confirmación de contraseña no coincide al aceptar una invitación.

```
{
  "statusCode": 400,
  "message": [
    "correo must be an email",
    "rol must be a valid enum value"
  ],
  "error": "Bad Request"
}
```

También puede aparecer con el mensaje:

```
{
  "statusCode": 400,
  "message": "Las contraseñas no coinciden",
  "error": "Bad Request"
}
```

#### `401 Unauthorized`

Se produce cuando una ruta administrativa no recibe JWT válido o el guard rechaza la sesión.

```
{
  "statusCode": 401,
  "message": "No autorizado",
  "error": "Unauthorized"
}
```

#### `403 Forbidden`

Puede aparecer cuando el usuario autenticado no tiene el rol `ADMINISTRADOR` requerido por la ruta.

```
{
  "statusCode": 403,
  "message": "Forbidden resource",
  "error": "Forbidden"
}
```

### `POST /invitations`

Genera una invitación nueva para un correo y rol determinados.

#### Seguridad

- Requiere `JwtAuthGuard`.
- Requiere `RolesGuard`.
- Rol permitido: `ADMINISTRADOR`.

#### Request

Content-Type: `application/json`

```
{
  "correo": "nuevo.usuario@dominio.com",
  "rol": 1
}
```

#### Validaciones

- `correo` es obligatorio y debe ser email.
- `rol` es obligatorio y debe pertenecer al enum `UserRole`.

#### Respuesta exitosa

HTTP `201 Created`

La respuesta devuelve el resultado del caso de uso de creación. Según el modelo actual, incluye la invitación persistida y el token generado para envío.

#### Errores posibles

- `401 Unauthorized` si no hay sesión válida.
- `403 Forbidden` si el usuario no es administrador.
- `400 Bad Request` si el body no cumple el DTO.
- `400 Bad Request` si el email ya tiene una invitación pendiente.
- `400 Bad Request` si el dominio del correo no está permitido.

### `GET /invitations`

Lista invitaciones con filtros de búsqueda y estado.

#### Seguridad

- Requiere `JwtAuthGuard`.
- Requiere `RolesGuard`.
- Rol permitido: `ADMINISTRADOR`.

#### Query params

```
/invitations?page=1&limit=10&term=bio&estado=0
```

- `page` opcional, paginación base 1.
- `limit` opcional, cantidad de resultados.
- `term` opcional, filtro de texto por correo.
- `estado` opcional, valor del enum `TokenStatus`.

#### Respuesta exitosa

HTTP `200 OK`

Devuelve una lista de invitaciones persistidas con su metadata de estado.

#### Errores posibles

- `401 Unauthorized` si no hay sesión válida.
- `403 Forbidden` si el usuario no es administrador.

### `GET /invitations/info/:token`

Consulta información pública de una invitación usando el token.

#### Seguridad

- No requiere JWT.
- No requiere rol.

#### Path params

- `token`: token de invitación presentado por el cliente.

#### Respuesta exitosa

HTTP `200 OK`

```
{
  "correo": "n***o@dominio.com",
  "expired": false,
  "accepted": false
}
```

#### Observaciones

- El correo se devuelve enmascarado.
- El endpoint no expone el token persistido ni el hash interno.

### `POST /invitations/accept`

Acepta una invitación, completa la creación del usuario asociado y lo deja 
autenticado de inmediato (emite los tokens de sesión, igual que `POST /auth/login`).

#### Seguridad

- No requiere JWT.
- Está protegido por validación de DTO.

#### Request

Content-Type: `application/json`

```
{
  "token": "uuid-o-token-emitido",
  "password": "12345678",
  "confirmPassword": "12345678",
  "nombres": "Juan",
  "apellidos": "Pérez"
}
```

#### Validaciones

- `token` es obligatorio.
- `password` es obligatorio.
- `confirmPassword` es obligatorio.
- `nombres` es obligatorio.
- `apellidos` es obligatorio.
- `password` y `confirmPassword` deben coincidir.

#### Respuesta exitosa

HTTP `200 OK`

El endpoint completa la aceptación, activa el usuario asociado a la invitación 
y devuelve el access token de sesión (mismo formato que el login):

```
{
  "accessToken": "eyJhbGciOi...",
  "accessTokenExpiresIn": 900
}
```

#### Cookies emitidas

Al igual que el login, el backend setea una cookie `refreshToken`:

- `httpOnly: true`
- `sameSite: lax`
- `path: /auth/refresh`
- `secure: true` cuando `NODE_ENV=production`
- `maxAge: 7 días`

#### Errores posibles

- `400 Bad Request` si las contraseñas no coinciden.
- `400 Bad Request` si el DTO no cumple validaciones.
- `400 Bad Request` si el token es inválido.
- `400 Bad Request` si la invitación ya expiró.
- `400 Bad Request` si la invitación ya fue consumida.

#### Observaciones

- El usuario queda autenticado inmediatamente tras aceptar; no necesita un 
 `POST /auth/login` adicional.
- El access token se devuelve en el body; el refresh token viaja en cookie 
 `httpOnly` (no en JSON).
- `400 Bad Request` si el dominio del correo no está permitido.

### `DELETE /invitations/:id`

Revoca una invitación por su identificador numérico.

#### Seguridad

- Requiere `JwtAuthGuard`.
- Requiere `RolesGuard`.
- Rol permitido: `ADMINISTRADOR`.

#### Path params

- `id`: identificador numérico de la invitación.

#### Respuesta exitosa

HTTP `200 OK`

Devuelve la invitación actualizada luego de revocarla.

#### Errores posibles

- `401 Unauthorized` si no hay sesión válida.
- `403 Forbidden` si el usuario no es administrador.
- `400 Bad Request` si `id` no es numérico.
- `400 Bad Request` si la invitación no existe.

### Proceso interno de expiración automática

La expiración de invitaciones no se expone como endpoint HTTP. Se programa de forma interna al crear la invitación y se ejecuta cuando vence `expiresAt`.

#### Flujo interno

1. `CreateInvitationUseCase` persiste la invitación con `expiresAt` calculado.
2. La infraestructura de cola agenda un job diferido para la fecha exacta de vencimiento.
3. Cuando el job se ejecuta, invoca `ExpireInvitationUseCase` con el `id` de la invitación.
4. El caso de uso marca la invitación como `EXPIRADO` si todavía está pendiente.

#### Observaciones

- La expiración automática es idempotente: si el token ya fue aceptado o revocado, no vuelve a cambiar de estado.
- Existe un único mecanismo interno para el vencimiento; no hay endpoint HTTP asociado.
- El job diferido mejora la precisión frente a un barrido periódico y respeta la separación entre aplicación e infraestructura.

### Mapeo de casos de uso

| Caso de uso | Endpoint HTTP | Estado |
| --- | --- | --- |
| `CreateInvitationUseCase` | `POST /invitations` | Implementado |
| `ListInvitationsUseCase` | `GET /invitations` | Implementado |
| `ObtainInfoUseCase` | `GET /invitations/info/:token` | Implementado |
| `AcceptInvitationUseCase` | `POST /invitations/accept` | Implementado |
| `RevokeInvitationUseCase` | `DELETE /invitations/:id` | Implementado |
| `ExpireInvitationUseCase` | Proceso interno diferido | Interno |

### Observaciones

- La invitación se consume una sola vez al aceptarse.
- Al aceptar la invitación el usuario queda autenticado de inmediato: el endpoint emite el access token y la cookie de refresh igual que `POST /auth/login`, evitando un login extra.
- El controller actual usa guards de JWT y roles en las rutas administrativas.
- `ExpireInvitationUseCase` existe en aplicación, pero todavía no está expuesto por HTTP.
- El acceso público queda limitado a la consulta del token y la aceptación.

## Módulo `leads`

Base path: `/leads`

El módulo de leads administra las oportunidades del CRM. Cada lead pertenece obligatoriamente a una organización, opcionalmente a un contacto, y siempre tiene un encargado. Soporta creación, consulta, listado paginado con filtros, actualización, cambio de estado y eliminación lógica (soft delete). Todas las rutas requieren autenticación JWT.

### Seguridad

- Todas las rutas requieren `JwtAuthGuard` (`@ApiBearerAuth()`).
- El `idAuthor` se obtiene automáticamente del usuario autenticado (`@CurrentUser()`), no del body.

### Reglas de negocio aplicadas

- La organización (`idOrg`) debe existir al crear o actualizar.
- El contacto es opcional; si se envía, debe existir, pertenecer a la organización del lead y estar vigente (`estado_correo = VIGENTE`).
- El encargado (`idEncargado`) debe existir.
- El estado inicial al crear es `EN_PROSPECTO`.
- Los estados válidos son los del esquema: `EN_PROSPECTO`, `OFERTADO`, `CIERRE_CON_VENTA`, `CIERRE_SIN_VENTA`.
- La eliminación es lógica: marca `deletedAt` y los registros eliminados quedan excluidos de las consultas.

### Formato de respuesta de error

Los errores se serializan con el `GlobalExceptionFilter`, que añade `kind`, `path` y `timestamp` al payload estándar.

#### `400 Bad Request`

DTO inválido, o contacto no válido (inexistente, de otra organización o no vigente).

```
{
  "statusCode": 400,
  "error": "LeadContactInvalidException",
  "kind": "Validation",
  "message": "El contacto no se encuentra vigente",
  "path": "/leads",
  "timestamp": "2026-05-31T10:30:00.000Z"
}
```

#### `401 Unauthorized`

```
{
  "statusCode": 401,
  "message": "No autorizado",
  "error": "Unauthorized"
}
```

#### `404 Not Found`

Lead, organización o encargado inexistentes.

```
{
  "statusCode": 404,
  "error": "LeadNotFoundException",
  "kind": "NotFound",
  "message": "Lead con id 99 no encontrado",
  "path": "/leads/99",
  "timestamp": "2026-05-31T10:30:00.000Z"
}
```

### `POST /leads`

Crea un nuevo lead. El estado inicial siempre es `EN_PROSPECTO`.

#### Request

Content-Type: `application/json`

```
{
  "idOrg": "123e4567-e89b-12d3-a456-426614174000",
  "idContacto": 1,
  "servicioInteres": "Consultoría en transformación digital",
  "comentarios": "Cliente interesado en paquete completo",
  "desafioOportunidad": "Necesita optimizar procesos internos",
  "notasContacto": "Llamada inicial realizada, cliente muy interesado",
  "canalCaptacion": "LinkedIn",
  "idEncargado": 1
}
```

#### Validaciones

| Campo | Tipo | Obligatorio | Longitud máx. | Notas |
| --- | --- | --- | --- | --- |
| `idOrg` | `string` (UUID) | Sí | — | La organización debe existir |
| `idContacto` | `number` | No | — | Si se envía, mín. 1; debe existir, pertenecer a `idOrg` y estar vigente |
| `servicioInteres` | `string` | Sí | 120 | |
| `comentarios` | `string` | No | 500 | `null` si no se envía |
| `desafioOportunidad` | `string` | No | 500 | `null` si no se envía |
| `notasContacto` | `string` | No | 1000 | `null` si no se envía |
| `canalCaptacion` | `string` | No | 60 | `null` si no se envía |
| `idEncargado` | `number` | Sí | — | Mín. 1; el usuario debe existir |

#### Respuesta exitosa (`201 Created`)

```
{
  "id": 1,
  "estado": "EN_PROSPECTO",
  "servicioInteres": "Consultoría en transformación digital",
  "comentarios": "Cliente interesado en paquete completo",
  "desafioOportunidad": "Necesita optimizar procesos internos",
  "notasContacto": "Llamada inicial realizada, cliente muy interesado",
  "canalCaptacion": "LinkedIn",
  "idOrg": "123e4567-e89b-12d3-a456-426614174000",
  "organizationName": "Bioactiva SAC",
  "idContacto": 1,
  "contactName": "Juan Pérez",
  "idEncargado": 1,
  "encargadoName": "Carlos López",
  "idAuthor": 3,
  "createdAt": "2026-01-15T10:30:00.000Z",
  "updatedAt": "2026-01-15T10:30:00.000Z",
  "ultimoCambioEstado": "2026-01-15T10:30:00.000Z"
}
```

#### Errores posibles

- `400 Bad Request` si el DTO no cumple validaciones.
- `400 Bad Request` si el contacto no existe, es de otra organización o no está vigente.
- `404 Not Found` si la organización no existe.
- `404 Not Found` si el encargado no existe.

### `GET /leads`

Lista leads con filtros opcionales y paginación. Excluye los registros eliminados.

#### Query params

| Parámetro | Tipo | Obligatorio | Default | Descripción |
| --- | --- | --- | --- | --- |
| `estado` | `LeadState` | No | — | Filtra por estado |
| `idOrg` | `string` | No | — | Filtra por organización |
| `idEncargado` | `number` | No | — | Filtra por encargado (mín. 1) |
| `search` | `string` | No | — | Búsqueda insensible a mayúsculas sobre `servicioInteres` (máx. 100) |
| `page` | `number` | No | `1` | Número de página (mín. 1) |
| `limit` | `number` | No | `10` | Elementos por página (mín. 1) |

#### Respuesta exitosa (`200 OK`)

```
{
  "data": [
    {
      "id": 1,
      "estado": "EN_PROSPECTO",
      "servicioInteres": "Consultoría en transformación digital",
      "comentarios": "Cliente interesado",
      "desafioOportunidad": "Necesita optimizar procesos",
      "notasContacto": "Llamada inicial realizada",
      "canalCaptacion": "LinkedIn",
      "idOrg": "123e4567-e89b-12d3-a456-426614174000",
      "organizationName": "Bioactiva SAC",
      "idContacto": 1,
      "contactName": "Juan Pérez",
      "idEncargado": 1,
      "encargadoName": "Carlos López",
      "idAuthor": 3,
      "createdAt": "2026-01-15T10:30:00.000Z",
      "updatedAt": "2026-01-15T10:30:00.000Z",
      "ultimoCambioEstado": "2026-01-15T10:30:00.000Z"
    }
  ],
  "meta": {
    "page": 1,
    "limit": 10,
    "total": 1,
    "totalPages": 1
  }
}
```

#### Ejemplo de llamada

```
GET /leads?estado=EN_PROSPECTO&idOrg=123e4567-...&search=consultoría&page=1&limit=10
Authorization: Bearer <token>
```

### `GET /leads/:id`

Obtiene el detalle de un lead por su ID, incluyendo nombre de organización, contacto y encargado. No retorna registros eliminados.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID numérico del lead |

#### Respuesta exitosa (`200 OK`)

Devuelve un lead (misma estructura que un elemento de `data` en `GET /leads`).

#### Errores posibles

- `404 Not Found` si el lead no existe o está eliminado.

### `PATCH /leads/:id`

Actualiza los campos de negocio de un lead. Todos los campos son opcionales; solo se actualizan los enviados. Mantiene las validaciones de organización, contacto y encargado cuando esos campos se envían.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID numérico del lead |

#### Request

Content-Type: `application/json`

```
{
  "servicioInteres": "Nuevo servicio",
  "idContacto": null
}
```

#### Validaciones

Mismos campos que `POST /leads`, todos opcionales (excepto `idAuthor`, que nunca se envía). Enviar `idContacto: null` desvincula el contacto del lead. El estado no se modifica por este endpoint.

#### Respuesta exitosa (`200 OK`)

Devuelve el lead actualizado (misma estructura que `GET /leads/:id`).

#### Errores posibles

- `400 Bad Request` si el DTO no cumple validaciones.
- `400 Bad Request` si el contacto no existe, es de otra organización o no está vigente.
- `404 Not Found` si el lead, la nueva organización o el nuevo encargado no existen.

### `PATCH /leads/:id/status`

Cambia el estado del lead y actualiza `ultimoCambioEstado`.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID numérico del lead |

#### Request

Content-Type: `application/json`

```
{
  "estado": "OFERTADO"
}
```

#### Validaciones

- `estado` es obligatorio y debe pertenecer al enum `LeadState` (`EN_PROSPECTO`, `OFERTADO`, `CIERRE_CON_VENTA`, `CIERRE_SIN_VENTA`).

#### Respuesta exitosa (`200 OK`)

Devuelve el lead actualizado (misma estructura que `GET /leads/:id`).

#### Errores posibles

- `400 Bad Request` si `estado` no es un valor válido del enum.
- `404 Not Found` si el lead no existe.

### `DELETE /leads/:id`

Elimina lógicamente un lead (soft delete): marca `deletedAt` sin borrar físicamente el registro.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID numérico del lead |

#### Respuesta exitosa (`200 OK`)

```
{
  "ok": true
}
```

#### Errores posibles

- `404 Not Found` si el lead no existe o ya estaba eliminado.

### Campos del response

| Campo | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID del lead |
| `estado` | `string` | Estado actual (`EN_PROSPECTO`, `OFERTADO`, `CIERRE_CON_VENTA`, `CIERRE_SIN_VENTA`) |
| `servicioInteres` | `string` | Servicio de interés |
| `comentarios` | `string | null` | Comentarios adicionales |
| `desafioOportunidad` | `string | null` | Desafío u oportunidad identificada |
| `notasContacto` | `string | null` | Notas de contacto |
| `canalCaptacion` | `string | null` | Canal de captación |
| `idOrg` | `string` (UUID) | ID de la organización asociada |
| `organizationName` | `string` | Nombre de la organización (JOIN) |
| `idContacto` | `number | null` | ID del contacto asociado |
| `contactName` | `string | null` | Nombre del contacto (JOIN), `null` si no hay contacto |
| `idEncargado` | `number` | ID del usuario encargado |
| `encargadoName` | `string` | Nombre completo del encargado (JOIN) |
| `idAuthor` | `number` | ID del usuario que creó el lead |
| `createdAt` | `string` (ISO 8601) | Fecha de creación |
| `updatedAt` | `string` (ISO 8601) | Fecha de última actualización |
| `ultimoCambioEstado` | `string` (ISO 8601) | Fecha del último cambio de estado |

### Mapeo de casos de uso

| Caso de uso | Endpoint HTTP | Estado |
| --- | --- | --- |
| `CreateLeadUseCase` | `POST /leads` | Implementado |
| `ListLeadsUseCase` | `GET /leads` | Implementado |
| `GetLeadByIdUseCase` | `GET /leads/:id` | Implementado |
| `UpdateLeadUseCase` | `PATCH /leads/:id` | Implementado |
| `ChangeLeadStatusUseCase` | `PATCH /leads/:id/status` | Implementado |
| `DeleteLeadUseCase` | `DELETE /leads/:id` | Implementado |

### Observaciones

- Es uno de los módulos centrales del CRM.
- La autoría (`idAuthor`) se obtiene del token JWT, no del body.
- `organizationName`, `contactName` y `encargadoName` se resuelven por JOIN; el frontend no necesita llamadas adicionales.
- La búsqueda textual (`search`) es insensible a mayúsculas y aplica solo sobre `servicioInteres`.
- Los registros con `deletedAt` distinto de `null` quedan excluidos de todas las consultas.
- Las actividades y cotizaciones asociadas a un lead se exponen en sus propios módulos (`activities`, `quotations`).

## Módulo `notifications`

### Estado actual

- Dominio de notificaciones implementado.
- No hay controlador HTTP visible.

### Endpoints pendientes

| Endpoint sugerido | Estado | Nota |
| --- | --- | --- |
| `GET /notifications` | Pendiente | Listado de notificaciones |
| `PATCH /notifications/:id/read` | Pendiente | Marcar como leída |
| `PATCH /notifications/:id/unread` | Pendiente | Marcar como no leída |

### Observaciones

- Puede ser módulo interno o expuesto parcialmente para UI.

## Módulo `organizations`

Base path: `/organizations`

El módulo de organizaciones expone endpoints para gestionar empresas y entidades registradas en el sistema. Incluye consultas al scraper de SUNAT para obtener datos de contribuyentes peruanos.

### Formato de respuesta de error

Sigue el formato estándar de NestJS.

#### `400 Bad Request`

DTO inválido o error de validación de dominio.

```
{
  "statusCode": 400,
  "message": "El RUC '12345678901' no es válido o no existe en SUNAT.",
  "error": "Bad Request"
}
```

#### `404 Not Found`

Cuando no se encuentra la organización o no hay resultados en SUNAT.

```
{
  "statusCode": 404,
  "message": "No se encontraron resultados en SUNAT para la organización consultada.",
  "error": "Not Found"
}
```

### `POST /organizations`

Crea una nueva organización.

#### Seguridad

- No requiere JWT ni roles por el momento.

#### Request

Content-Type: `application/json`

```
{
  "codigoCliente": "CLI-001",
  "nombre": "Mi Empresa S.A.C.",
  "nombreComercial": "Mi Empresa",
  "subArea": null,
  "ruc": "10730315550",
  "tipo": "EMPRESA_NACIONAL",
  "linkedin": null,
  "ubicacion": "Lima",
  "sector": "TECNOLOGIA",
  "tamano": "PEQUENO",
  "actividadEconomica": "Desarrollo de Software",
  "alianzasEstrategicas": null,
  "idContactoActivo": null,
  "idAuthor": 1
}
```

#### Validaciones

- `codigoCliente`: obligatorio, máximo 20 caracteres.
- `nombre`: obligatorio, máximo 120 caracteres.
- `nombreComercial`: obligatorio, máximo 100 caracteres.
- `subArea`: opcional, máximo 60 caracteres.
- `ruc`: opcional, exactamente 11 caracteres. Si se provee, se valida contra SUNAT.
- `tipo`: obligatorio, enum `EnterpriseType`.
- `linkedin`: opcional, máximo 255 caracteres.
- `ubicacion`: opcional, máximo 100 caracteres.
- `sector`: opcional, enum `Sector`.
- `tamano`: obligatorio, enum `Size`.
- `actividadEconomica`: opcional, máximo 120 caracteres.
- `alianzasEstrategicas`: opcional, máximo 300 caracteres.
- `idContactoActivo`: opcional, número.
- `idAuthor`: obligatorio, número.

#### Respuesta exitosa

HTTP `201 Created`

Devuelve la organización creada.

#### Errores posibles

- `400 Bad Request` si el DTO no cumple validaciones.
- `400 Bad Request` si el RUC no tiene 11 dígitos.
- `400 Bad Request` si el RUC ya está registrado.
- `400 Bad Request` si el RUC no existe en SUNAT.

### `GET /organizations`

Lista todas las organizaciones registradas.

#### Seguridad

- No requiere JWT ni roles.

#### Respuesta exitosa

HTTP `200 OK`

Devuelve un arreglo de organizaciones.

### `GET /organizations/sunat/:query`

Consulta información de empresas en SUNAT.

#### Path params

- `query`: puede ser un RUC de 11 dígitos (búsqueda exacta) o un nombre/razón social (búsqueda por coincidencia).

#### Comportamiento

- Si el parámetro tiene 11 dígitos, se busca por RUC.
- Si no, se busca por razón social.
- La consulta delega en el microservicio Python `sunat-app`.

#### Respuesta exitosa

HTTP `200 OK`

Para búsqueda por RUC:

```
{
  "ruc": "10730315550",
  "razonSocial": "ESCOBAR PEREZ YURI ABEL",
  "nombreComercial": "ESCOBAR PEREZ YURI ABEL",
  "tipo": "INDEPENDIENTE",
  "ubicacion": "AREQUIPA",
  "actividadEconomica": "OTRAS ACTIVIDADES DE SERVICIOS PERSONALES N.C.P.",
  "tamano": "MICRO",
  "sector": "OTROS"
}
```

Para búsqueda por razón social, devuelve un arreglo de resultados.

#### Errores posibles

- `404 Not Found` si no hay resultados en SUNAT.

#### Observaciones

- Este endpoint requiere que el microservicio `sunat-app` esté corriendo y accesible en `PYTHON_SCRAPER_URL`.

### `GET /organizations/:id`

Obtiene una organización por su ID.

#### Path params

- `id`: UUID de la organización.

#### Respuesta exitosa

HTTP `200 OK`

Devuelve la organización encontrada.

#### Errores posibles

- `404 Not Found` si el ID no existe.

### `PATCH /organizations/:id`

Actualiza parcialmente una organización.

#### Seguridad

- No requiere JWT ni roles.

#### Path params

- `id`: UUID de la organización.

#### Request

Content-Type: `application/json`

```
{
  "nombre": "Nuevo Nombre",
  "tamano": "GRANDE"
}
```

#### Validaciones

Mismos campos que `POST /organizations`, pero todos opcionales.

#### Respuesta exitosa

HTTP `200 OK`

Devuelve la organización actualizada.

#### Errores posibles

- `400 Bad Request` si el DTO no cumple validaciones.
- `404 Not Found` si el ID no existe.
- `400 Bad Request` si el nuevo RUC ya está registrado.
- `400 Bad Request` si el nuevo RUC no existe en SUNAT.

### Observaciones

- El dominio modela sector (`Sector`), tamaño (`Size`) y tipo de empresa (`EnterpriseType`).
- La integración con SUNAT usa el microservicio Python (`sunat-app`).
- La autoría (`idAuthor`) se recibe del body; no se deriva del usuario autenticado.
- La ruta `GET /organizations/sunat/:query` debe definirse antes que `GET /organizations/:id` para evitar conflictos de ruteo.

## Módulo `quotations`

Base path: `/quotations`

El módulo de cotizaciones administra las propuestas comerciales asociadas a un Lead. Cada cotización pertenece a un Lead y a un Remitente (usuario emisor), registra quién la creó (`idAuthor`, tomado del token JWT), y sigue un ciclo de estados (`PENDIENTE → ENVIADA → ACEPTADA` / `RECHAZADA`) con soft delete. Aceptar o rechazar una cotización cierra el Lead asociado (`CIERRE_CON_VENTA` / `CIERRE_SIN_VENTA`) de forma atómica. Todas las rutas requieren autenticación JWT.

### Seguridad

- Todas las rutas requieren `JwtAuthGuard` (`@ApiBearerAuth()`).
- El creador (`idAuthor`) se obtiene del token JWT, no del body.
- No hay restricción por propietario: cualquier usuario autenticado puede modificar, enviar, aceptar, rechazar o eliminar cualquier cotización.

### Reglas de negocio aplicadas

- La cotización debe estar asociada a un Lead existente y a un Remitente existente (RN-001, RN-002).
- Toda cotización nueva inicia en estado `PENDIENTE` (RN-003).
- Estados válidos: `PENDIENTE`, `ENVIADA`, `ACEPTADA`, `RECHAZADA` (RN-004).
- `send()` solo es válido desde `PENDIENTE` (RN-005).
- `accept()` y `reject()` solo son válidos desde `PENDIENTE` o `ENVIADA` (RN-006).
- Una cotización `ACEPTADA` o `RECHAZADA` no puede modificarse ni cambiar de estado (RN-007).
- Aceptar pasa el Lead a `CIERRE_CON_VENTA`; rechazar lo pasa a `CIERRE_SIN_VENTA`, en una sola transacción (RN-008).
- La transición de estado usa concurrencia optimista: si entre la lectura y la escritura otra operación ya cambió el estado, la operación se rechaza con `409 Conflict` (RN-009).
- La eliminación es lógica: marca `deletedAt` y los registros eliminados quedan excluidos de las consultas.

### Formato de respuesta de error

Los errores se serializan con el `GlobalExceptionFilter`, que añade `kind`, `path` y `timestamp` al payload.

#### `400 Bad Request`

DTO inválido (p. ej. `monto` no numérico) o rango de fechas invertido (`fechaHasta < fechaDesde`) en el listado.

```
{
  "statusCode": 400,
  "error": "BadRequestException",
  "kind": "Validation",
  "message": ["fechaHasta debe ser posterior o igual a fechaDesde"],
  "path": "/quotations",
  "timestamp": "2026-06-01T10:30:00.000Z"
}
```

#### `404 Not Found`

Cotización, Lead o Remitente inexistentes.

```
{
  "statusCode": 404,
  "error": "CotizacionNotFoundException",
  "kind": "NotFound",
  "message": "Cotización con id 99 no encontrada",
  "path": "/quotations/99",
  "timestamp": "2026-06-01T10:30:00.000Z"
}
```

#### `409 Conflict`

La cotización fue procesada concurrentemente por otra operación (su estado cambió entre la lectura y la escritura).

```
{
  "statusCode": 409,
  "error": "CotizacionConflictException",
  "kind": "Conflict",
  "message": "La cotización con id 1 ya fue procesada por otra operación",
  "path": "/quotations/1/accept",
  "timestamp": "2026-06-01T10:30:00.000Z"
}
```

#### Transición inválida

Enviar/aceptar/rechazar/modificar una cotización en un estado no permitido devuelve `400` con `InvalidCotizacionTransitionException`.

```
{
  "statusCode": 400,
  "error": "InvalidCotizacionTransitionException",
  "kind": "Validation",
  "message": "Solo se puede enviar una cotización en estado PENDIENTE",
  "path": "/quotations/1/send",
  "timestamp": "2026-06-01T10:30:00.000Z"
}
```

### `POST /quotations`

Crea una nueva cotización. El estado inicial siempre es `PENDIENTE`. El creador (`idAuthor`) se toma del token JWT.

#### Request

Content-Type: `application/json`

```
{
  "fechaCot": "2026-06-01T10:00:00.000Z",
  "dirigido": "Dr. Martinez",
  "cliente": "TechCorp SA",
  "producto": "Licencia Software Pro",
  "nombreServicio": "Desarrollo Customizado",
  "monto": "5000.00",
  "tipo": "USD",
  "observacion": "Incluye 3 meses de soporte",
  "linkPropuesta": "https://proposal.techcorp.com/cot-001",
  "idLead": 1,
  "idRemitente": 1
}
```

#### Validaciones

| Campo | Tipo | Obligatorio | Longitud máx. | Notas |
| --- | --- | --- | --- | --- |
| `fechaCot` | `string` (ISO 8601) | Sí | — | |
| `dirigido` | `string` | Sí | 90 | |
| `cliente` | `string` | No | 120 | `null` si no se envía |
| `producto` | `string` | No | 120 | `null` si no se envía |
| `nombreServicio` | `string` | Sí | 150 | |
| `monto` | `string` (numérico) | Sí | — | Cadena numérica; se almacena como `Decimal(12,2)` |
| `tipo` | `enum` | Sí | — | `PEN`, `USD` |
| `observacion` | `string` | No | 1000 | `null` si no se envía |
| `linkPropuesta` | `string` | No | 500 | `null` si no se envía |
| `idLead` | `number` | Sí | — | Mín. 1; el Lead debe existir |
| `idRemitente` | `number` | Sí | — | Mín. 1; el usuario debe existir |

> `nombreRemitente` se deriva automáticamente del usuario `idRemitente` (no se envía en el body).

#### Respuesta exitosa (`201 Created`)

```
{
  "id": 1,
  "fechaCot": "2026-06-01T10:00:00.000Z",
  "dirigido": "Dr. Martinez",
  "cliente": "TechCorp SA",
  "producto": "Licencia Software Pro",
  "nombreRemitente": "Juan Perez",
  "nombreServicio": "Desarrollo Customizado",
  "monto": "5000.00",
  "tipo": "USD",
  "estado": "PENDIENTE",
  "observacion": "Incluye 3 meses de soporte",
  "linkPropuesta": "https://proposal.techcorp.com/cot-001",
  "idLead": 1,
  "leadServicioInteres": "Consultoría en transformación digital",
  "leadEstado": "EN_PROSPECTO",
  "contactName": "María Gómez",
  "idRemitente": 1,
  "remitenteName": "Juan Perez",
  "idAuthor": 1,
  "createdAt": "2026-06-01T10:30:00.000Z",
  "updatedAt": "2026-06-01T10:30:00.000Z"
}
```

#### Errores posibles

- `400 Bad Request` si el DTO no cumple validaciones (p. ej. `monto` no numérico).
- `404 Not Found` si el Lead o el Remitente no existen.

### `GET /quotations`

Lista cotizaciones con filtros opcionales y paginación. Excluye los registros eliminados. Orden por `createdAt` descendente.

#### Query params

| Parámetro | Tipo | Obligatorio | Default | Descripción |
| --- | --- | --- | --- | --- |
| `idLead` | `number` | No | — | Filtra por Lead (mín. 1) |
| `estado` | `EstadoCot` | No | — | `PENDIENTE`, `ENVIADA`, `ACEPTADA`, `RECHAZADA` |
| `idRemitente` | `number` | No | — | Filtra por remitente (mín. 1) |
| `fechaDesde` | `string` (ISO 8601) | No | — | `fechaCot` ≥ a este valor |
| `fechaHasta` | `string` (ISO 8601) | No | — | `fechaCot` ≤ a este valor; debe ser ≥ `fechaDesde` |
| `page` | `number` | No | `1` | Número de página (mín. 1) |
| `limit` | `number` | No | `10` | Elementos por página (mín. 1) |

#### Respuesta exitosa (`200 OK`)

```
{
  "data": [
    {
      "id": 1,
      "fechaCot": "2026-06-01T10:00:00.000Z",
      "dirigido": "Dr. Martinez",
      "cliente": "TechCorp SA",
      "producto": "Licencia Software Pro",
      "nombreRemitente": "Juan Perez",
      "nombreServicio": "Desarrollo Customizado",
      "monto": "5000.00",
      "tipo": "USD",
      "estado": "PENDIENTE",
      "observacion": "Incluye 3 meses de soporte",
      "linkPropuesta": "https://proposal.techcorp.com/cot-001",
      "idLead": 1,
      "leadServicioInteres": "Consultoría en transformación digital",
      "leadEstado": "EN_PROSPECTO",
      "contactName": "María Gómez",
      "idRemitente": 1,
      "remitenteName": "Juan Perez",
      "idAuthor": 1,
      "createdAt": "2026-06-01T10:30:00.000Z",
      "updatedAt": "2026-06-01T10:30:00.000Z"
    }
  ],
  "meta": {
    "page": 1,
    "limit": 10,
    "total": 1,
    "totalPages": 1
  }
}
```

#### Ejemplo de llamada

```
GET /quotations?idLead=1&estado=PENDIENTE&fechaDesde=2026-01-01&fechaHasta=2026-12-31&page=1&limit=10
Authorization: Bearer <token>
```

#### Errores posibles

- `400 Bad Request` si `fechaHasta` es anterior a `fechaDesde`.

### `GET /quotations/:id`

Obtiene el detalle de una cotización por su ID, incluyendo datos del Lead y del remitente. No retorna registros eliminados.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID numérico de la cotización |

#### Respuesta exitosa (`200 OK`)

Devuelve una cotización (misma estructura que un elemento de `data` en `GET /quotations`).

#### Errores posibles

- `404 Not Found` si la cotización no existe o está eliminada.

### `PATCH /quotations/:id`

Actualiza los campos de negocio de una cotización. Todos los campos son opcionales; solo se actualizan los enviados. No permite modificar `estado`, `idLead`, `idRemitente`, `createdAt` ni `deletedAt`.

#### Parámetros de ruta

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID numérico de la cotización |

#### Request

Content-Type: `application/json`

```
{
  "monto": "6500.00",
  "observacion": "Se amplía el alcance del soporte"
}
```

#### Validaciones

Campos permitidos (todos opcionales): `fechaCot`, `dirigido`, `cliente`, `producto`, `nombreServicio`, `monto`, `tipo`, `observacion`, `linkPropuesta`. Mismas reglas de longitud y formato que en `POST /quotations`.

#### Respuesta exitosa (`200 OK`)

Devuelve la cotización actualizada (misma estructura que `GET /quotations/:id`).

#### Errores posibles

- `400 Bad Request` si el DTO no cumple validaciones, o `InvalidCotizacionTransitionException` si la cotización ya está `ACEPTADA` o `RECHAZADA`.
- `404 Not Found` si la cotización no existe.

### `PATCH /quotations/:id/send`

Marca la cotización como `ENVIADA`. Solo permitido desde `PENDIENTE`.

#### Respuesta exitosa (`200 OK`)

Devuelve la cotización actualizada (misma estructura que `GET /quotations/:id`).

#### Errores posibles

- `400 Bad Request` si la cotización no está en `PENDIENTE`.
- `404 Not Found` si la cotización no existe.

### `PATCH /quotations/:id/accept`

Marca la cotización como `ACEPTADA` y cierra el Lead asociado como `CIERRE_CON_VENTA`, en una sola transacción. Solo permitido desde `PENDIENTE` o `ENVIADA`.

#### Respuesta exitosa (`200 OK`)

Devuelve la cotización actualizada (misma estructura que `GET /quotations/:id`).

#### Errores posibles

- `400 Bad Request` si la cotización no está en `PENDIENTE` ni `ENVIADA`.
- `404 Not Found` si la cotización o el Lead no existen.
- `409 Conflict` si la cotización fue procesada concurrentemente por otra operación.

### `PATCH /quotations/:id/reject`

Marca la cotización como `RECHAZADA` y cierra el Lead asociado como `CIERRE_SIN_VENTA`, en una sola transacción. Solo permitido desde `PENDIENTE` o `ENVIADA`.

#### Respuesta exitosa (`200 OK`)

Devuelve la cotización actualizada (misma estructura que `GET /quotations/:id`).

#### Errores posibles

- `400 Bad Request` si la cotización no está en `PENDIENTE` ni `ENVIADA`.
- `404 Not Found` si la cotización o el Lead no existen.
- `409 Conflict` si la cotización fue procesada concurrentemente por otra operación.

### `DELETE /quotations/:id`

Elimina lógicamente una cotización (soft delete): marca `deletedAt` sin borrar físicamente el registro.

#### Respuesta exitosa (`200 OK`)

```
{
  "ok": true
}
```

#### Errores posibles

- `404 Not Found` si la cotización no existe o ya estaba eliminada.

### Campos del response

| Campo | Tipo | Descripción |
| --- | --- | --- |
| `id` | `number` | ID de la cotización |
| `fechaCot` | `string` (ISO 8601) | Fecha de la cotización |
| `dirigido` | `string` | Destinatario de la cotización |
| `cliente` | `string | null` | Cliente |
| `producto` | `string | null` | Producto |
| `nombreRemitente` | `string` | Nombre del remitente (snapshot al crear) |
| `nombreServicio` | `string` | Servicio cotizado |
| `monto` | `string` | Monto (`Decimal(12,2)` serializado como string) |
| `tipo` | `string` | Tipo de moneda (`PEN`, `USD`) |
| `estado` | `string` | Estado actual (`PENDIENTE`, `ENVIADA`, `ACEPTADA`, `RECHAZADA`) |
| `observacion` | `string | null` | Observaciones |
| `linkPropuesta` | `string | null` | Enlace a la propuesta |
| `idLead` | `number` | ID del Lead asociado |
| `leadServicioInteres` | `string` | Servicio de interés del Lead (JOIN) |
| `leadEstado` | `string` | Estado del Lead (JOIN) |
| `contactName` | `string` | Nombre completo del contacto del Lead (JOIN; `''` si el Lead no tiene contacto) |
| `idRemitente` | `number` | ID del usuario remitente |
| `remitenteName` | `string` | Nombre completo del remitente (JOIN) |
| `idAuthor` | `number` | ID del usuario creador (del token JWT) |
| `createdAt` | `string` (ISO 8601) | Fecha de creación |
| `updatedAt` | `string` (ISO 8601) | Fecha de última actualización |

### Mapeo de casos de uso

| Caso de uso | Endpoint HTTP | Estado |
| --- | --- | --- |
| `CreateCotizacionUseCase` | `POST /quotations` | Implementado |
| `ListCotizacionesUseCase` | `GET /quotations` | Implementado |
| `GetCotizacionByIdUseCase` | `GET /quotations/:id` | Implementado |
| `UpdateCotizacionUseCase` | `PATCH /quotations/:id` | Implementado |
| `SendCotizacionUseCase` | `PATCH /quotations/:id/send` | Implementado |
| `AcceptCotizacionUseCase` | `PATCH /quotations/:id/accept` | Implementado |
| `RejectCotizacionUseCase` | `PATCH /quotations/:id/reject` | Implementado |
| `DeleteCotizacionUseCase` | `DELETE /quotations/:id` | Implementado |

### Observaciones

- `nombreRemitente` se guarda como snapshot al crear (no cambia si el usuario edita su nombre después); `remitenteName` del response se resuelve por JOIN con el usuario actual.
- `leadServicioInteres`, `leadEstado`, `contactName` y `remitenteName` se resuelven por JOIN; el frontend no necesita llamadas adicionales.
- `contactName` se obtiene del contacto del Lead (`lead.contacto`); si el Lead no tiene contacto asociado, devuelve cadena vacía.
- Aceptar/rechazar es transaccional: la cotización y el Lead se actualizan juntos o no se actualiza ninguno.
- La concurrencia optimista garantiza que dos `accept`/`reject` simultáneos no cierren el Lead dos veces; el segundo recibe `409 Conflict`.
- Los registros con `deletedAt` distinto de `null` quedan excluidos de todas las consultas.

## Módulo `reset_password`

Base path: `/reset-password`

El módulo de restablecimiento de contraseña permite solicitar un cambio de contraseña mediante un token de un solo uso enviado por correo electrónico. La infraestructura usa una cola BullMQ para el envío asíncrono del correo.

### Formato de respuesta de error

Las respuestas que no son `200 OK` siguen el formato estándar de NestJS para excepciones HTTP.

#### `400 Bad Request`

Se produce cuando el body no cumple el DTO, cuando las contraseñas no coinciden o cuando el token es inválido o expiró.

```
{
  "statusCode": 400,
  "message": [
    "El correo electrónico no es válido",
    "La contraseña debe tener al menos 6 caracteres"
  ],
  "error": "Bad Request"
}
```

También puede aparecer con un mensaje único:

```
{
  "statusCode": 400,
  "message": "Las contraseñas no coinciden",
  "error": "Bad Request"
}
```

```
{
  "statusCode": 400,
  "message": "Token de restablecimiento de contraseña inválido o ya utilizado",
  "error": "Bad Request"
}
```

```
{
  "statusCode": 400,
  "message": "El token de restablecimiento de contraseña ha expirado",
  "error": "Bad Request"
}
```

### `POST /reset-password/request`

Solicita un restablecimiento de contraseña para un correo determinado. Si el correo existe, se envía un token de un solo uso al email registrado.

#### Seguridad

- No requiere JWT.
- No requiere rol.
- Es público por diseño (el usuario no está autenticado cuando olvida su contraseña).

#### Request

Content-Type: `application/json`

```
{
  "correo": "usuario@dominio.com"
}
```

#### Validaciones

- `correo` es obligatorio y debe tener formato de email.

#### Respuesta exitosa

HTTP `200 OK`

```
{
  "ok": true
}
```

#### Comportamiento silencioso

Si el correo no existe en el sistema, el endpoint retorna `{ ok: true }` igualmente para evitar la enumeración de usuarios.

#### Errores posibles

- `400 Bad Request` si el body no cumple el DTO.

#### Observaciones

- El token se genera con `randomUUID` y se almacena hasheado con SHA-256.
- El envío del correo ocurre de forma asíncrona a través de una cola BullMQ (`RESET_PASSWORD_EMAIL_QUEUE`).
- El token expira a las 2 horas.
- El correo contiene el token en texto plano para que el usuario lo use en el endpoint de confirmación.

### `POST /reset-password/reset`

Confirma el restablecimiento de contraseña usando el token recibido por correo, la nueva contraseña y su confirmación.

#### Seguridad

- No requiere JWT.
- No requiere rol.

#### Request

Content-Type: `application/json`

```
{
  "token": "uuid-recibido-por-correo",
  "password": "nueva123",
  "confirmPassword": "nueva123"
}
```

#### Validaciones

- `token` es obligatorio.
- `password` es obligatorio y debe tener al menos 6 caracteres.
- `confirmPassword` es obligatorio.
- `password` y `confirmPassword` deben coincidir (validación manual en el controller).

#### Respuesta exitosa

HTTP `200 OK`

```
{
  "ok": true
}
```

#### Flujo interno

1. Se calcula el hash SHA-256 del token recibido y se busca en la base de datos.
2. Si el token no existe o no está en estado `PENDIENTE`, se rechaza la solicitud.
3. Si el token está expirado, se marca como `EXPIRADO` y se notifica al usuario.
4. Se obtiene el usuario asociado, se encripta y actualiza la contraseña.
5. El token se marca como `CONSUMIDO` (de un solo uso).

#### Errores posibles

- `400 Bad Request` si las contraseñas no coinciden.
- `400 Bad Request` si el DTO no cumple validaciones.
- `400 Bad Request` si el token es inválido o ya fue utilizado.
- `400 Bad Request` si el token ha expirado.

#### Observaciones

- El token es de un solo uso: una vez consumido no puede reutilizarse.
- La contraseña se hashea con el mismo `PasswordHasherPort` que usa el módulo `auth`.

### `POST /reset-password/validate`

Valida que un token de restablecimiento sea válido (pendiente y no expirado) y retorna el correo electrónico ofuscado al que pertenece.

#### Seguridad

- No requiere JWT.
- No requiere rol.

#### Request

Content-Type: `application/json`

```
{
  "token": "uuid-recibido-por-correo"
}
```

#### Validaciones

- `token` es obligatorio.

#### Respuesta exitosa

HTTP `200 OK`

```
{
  "correo": "u***o@dominio.com"
}
```

#### Regla de ofuscación

- Si el local-part tiene 1 o 2 caracteres, se muestra el primero y el resto se reemplaza con asteriscos.
- Si tiene más de 2 caracteres, se muestra el primero, luego asteriscos y finalmente el último carácter.
- El dominio se muestra completo.

| Local-part original | Ofuscado |
| --- | --- |
| `a` | `a*` |
| `an` | `a*` |
| `ana` | `a*a` |
| `user` | `u**r` |

#### Errores posibles

- `400 Bad Request` si el DTO no cumple validaciones.
- `400 Bad Request` si el token es inválido o ya fue utilizado.
- `400 Bad Request` si el token ha expirado.

#### Observaciones

- El endpoint no consume el token; solo valida su estado actual.
- Si el token está expirado, se marca como `EXPIRADO` en base de datos antes de responder.

### Mapeo de casos de uso

| Caso de uso | Endpoint HTTP | Estado |
| --- | --- | --- |
| `RequestPasswordResetUseCase` | `POST /reset-password/request` | Implementado |
| `ResetPasswordUseCase` | `POST /reset-password/reset` | Implementado |
| `ValidateResetTokenUseCase` | `POST /reset-password/validate` | Implementado |
| `ExpirePasswordResetTokenUseCase` | Proceso interno diferido | Interno |

### Proceso interno de expiración automática

La expiración de tokens de restablecimiento se agenda de forma interna al crear el token y se ejecuta cuando vence `expired_at`, utilizando el mismo mecanismo de cola diferida que el módulo de invitaciones.

#### Flujo interno

1. `RequestPasswordResetUseCase` persiste el token con `expired_at` calculado a 2 horas.
2. La infraestructura de cola agenda un job diferido para la fecha exacta de vencimiento.
3. Cuando el job se ejecuta, invoca `ExpirePasswordResetTokenUseCase` con el `id` del token.
4. El caso de uso marca el token como `EXPIRADO` si todavía está pendiente.

#### Observaciones

- La expiración automática es idempotente: si el token ya fue consumido o expiró manualmente, no vuelve a cambiar de estado.
- El job diferido mejora la precisión frente a un barrido periódico.
- Adicionalmente, la expiración se verifica de forma síncrona al momento de usar el token en los endpoints `reset` y `validate`.

## Módulo `tokens`

### Estado actual

- El módulo existe como dominio compartido.
- No hay controlador HTTP visible.

### Endpoints pendientes

| Endpoint sugerido | Estado | Nota |
| --- | --- | --- |
| `GET /tokens` | Pendiente | Listado interno o de soporte |
| `POST /tokens` | Pendiente | Emitir token de negocio |
| `DELETE /tokens/:id` | Pendiente | Revocar token |

### Observaciones

- Conviene aclarar en el futuro si este módulo será público o interno.

## Módulos sin contrato HTTP visible

Los módulos anteriores tienen estructura de dominio, pero todavía no se ven controladores NestJS en el código actual. Por eso sus endpoints están marcados como pendientes y deben tomarse como una guía de documentación, no como una API ya disponible.

## Reglas de documentación para nuevos módulos

Cuando aparezca un nuevo controlador HTTP, la documentación debe actualizarse con estos criterios:

1. Registrar el path base del controlador.
2. Documentar método, ruta, headers y body.
3. Indicar si usa JWT, cookies o roles.
4. Documentar respuestas exitosas y errores.
5. Marcar como pendiente solo lo que todavía no exista en el código.

## Referencias útiles

- [src/app.module.ts]()
- [src/modules/auth/auth.module.ts]()
- [src/modules/auth/infrastructure/http/auth.controller.ts]()
- [src/modules/users/user.module.ts]()
- [src/modules/common/prisma/prisma.module.ts]()

## Estado del documento

Este archivo documenta los endpoints reales de `auth` y deja explícitamente marcados los endpoints pendientes del resto de módulos. Si se agrega un controlador nuevo, esta guía debe evolucionar para reflejar el contrato HTTP real.

Last changed by 

---

 

[Yiuseppe24](https://hackmd.io/@3sCj7uDSR-mZ_RF6bfg1sw)

0

96

Add a comment

---

Published on ** [![](https://hackmd.io/Logo.svg) HackMD](https://hackmd.io/)**

×

### Sign in

Email

Password

 [Forgot password](https://hackmd.io/settings/forgotPassword)

or

 [![](https://hackmd.io/social/google.svg) Sign in via Google](https://hackmd.io/auth/google) [![](https://hackmd.io/social/facebook.svg) Sign in via Facebook](https://hackmd.io/auth/facebook) [![](https://hackmd.io/social/x.svg) Sign in via X(Twitter)](https://hackmd.io/auth/twitter) [![](https://hackmd.io/social/github.svg) Sign in via GitHub](https://hackmd.io/auth/github) [![](https://hackmd.io/social/dropbox.svg) Sign in via Dropbox](https://hackmd.io/auth/dropbox) [![](https://hackmd.io/images/wallet.svg) Sign in with Wallet\\ \\ Wallet ( )](https://hackmd.io/#)Connect another wallet Continue with a different method

New to HackMD? [Sign up](https://hackmd.io/join)

By signing in, you agree to our [terms of service](https://hackmd.io/s/terms).

 

Comment