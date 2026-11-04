<p align="center">
  <img src="./assets/di-banner.svg" alt="DI · Darío Idrovo · Desarrollo web, sistemas y redes" width="100%" />
</p>

# Hola, soy Darío Idrovo

**Ingeniero en Tecnologías de la Información · Desarrollador Full Stack y Analista de Datos**

Transformo necesidades de negocio en aplicaciones e información útil para tomar decisiones. Mi portafolio combina desarrollo web, APIs, bases de datos y análisis descriptivo, junto con experiencia en soporte técnico, configuración de equipos y redes. Busco construir soluciones claras, mantenibles y con un alcance bien documentado.

## Proyectos destacados

### NexusCore · Gestión operativa

Plataforma para registrar operaciones de logística, comercio y servicios, gestionar sus estados y generar eventos para análisis externo. Puede utilizarse sin NexusInsight.

**Tecnologías:** React, TypeScript, Node.js, NestJS y PostgreSQL.

[Código fuente](https://github.com/idrovodario16/nexuscore-platform) · [Demo web](https://nexuscore-idrovodario16-demo.brownlyric131.chatgpt.site/)

### NexusInsight · Análisis de operaciones

Plataforma para importar datos operativos, consultar indicadores, aplicar filtros y exportar resultados a CSV. Controla eventos duplicados y revisiones antiguas para mantener consistente el modelo analítico. Puede trabajar con la muestra incluida o con otra fuente compatible, sin depender de NexusCore.

**Tecnologías:** React, TypeScript, Python, FastAPI, PostgreSQL y SQL analítico.

[Código fuente](https://github.com/idrovodario16/nexusinsight-analytics) · [Demo web](https://nexusinsight-idrovodario16-demo.brownlyric131.chatgpt.site/)

### Independientes e integrables

Cada producto tiene su propio repositorio, API y base de datos. **NexusCore gestiona las operaciones; NexusInsight las convierte en indicadores.** Se integran mediante un contrato de eventos versionado: intercambio manual de JSON entre las demos o un relay HTTP entre las APIs, con reintentos y deduplicación.

[Arquitectura, contratos y guía de integración](https://github.com/idrovodario16/nexus-architecture)

**Estado actual:** ambos son MVP de portafolio con código público. Las demos usan datos ficticios y almacenamiento en el navegador; las APIs y la integración HTTP se ejecutan por separado en un entorno local. Las interfaces todavía no están conectadas a esas APIs. La conexión UI/API, la identidad OIDC/RBAC y la analítica predictiva forman parte de la evolución pendiente.

## Otros proyectos

| Proyecto | Aporte principal | Alcance actual |
| --- | --- | --- |
| [CargoFlow](https://github.com/idrovodario16/cargoflow) | Flujos configurables, inspecciones y seguimiento de estados para distintos sectores. | [Demo pública](https://idrovodario16.github.io/cargoflow/); prototipo con datos ficticios y persistencia en el navegador. |
| [Mis finanzas](https://github.com/idrovodario16/mis-finanzas) | Registro de ingresos, gastos y metas de ahorro con dashboard mensual. | [Demo pública](https://idrovodario16.github.io/mis-finanzas/) con datos ficticios y localStorage; aplicación original con autenticación y D1. Los ahorros se separan del saldo disponible. |
| [Cookies Privacy Analyzer](https://github.com/idrovodario16/cookies-dashboard) | Análisis descriptivo de metadatos de cookies, filtros y exportación de reportes. | [Demo pública](https://idrovodario16.github.io/cookies-dashboard/) con filtros y reportes ficticios; el análisis SQLite se ejecuta localmente con Python/Flask. |

## Resumen técnico por proyecto

| Proyecto | Lenguajes y frameworks | Base de datos o almacenamiento | Arquitectura |
| --- | --- | --- | --- |
| NexusCore | TypeScript/JavaScript, React, Node.js y NestJS | PostgreSQL en API; localStorage en demo | Monolito modular por capas y outbox transaccional; API independiente. |
| NexusInsight | Python/FastAPI, TypeScript/JavaScript y React | PostgreSQL en API; localStorage en demo | Ingesta modular, inbox de deduplicación y modelo analítico con SQL. |
| Nexus Architecture | JavaScript/Node.js, JSON Schema y OpenAPI | Sin base propia; cada producto conserva su PostgreSQL | Contratos y relay HTTP con checkpoint y reintentos; documentación C4. |
| CargoFlow | HTML, CSS y JavaScript | localStorage; sin base de servidor | Aplicación estática de navegador, sin backend. |
| Mis finanzas | TypeScript, React, Tailwind CSS y Vinext | Cloudflare D1 (SQLite) y Drizzle ORM | Aplicación full stack con rutas API, validación Zod y Cloudflare Workers. |
| Cookies Privacy Analyzer | Python/Flask, HTML/Jinja, CSS y JavaScript | Lectura de copias SQLite; resultados en memoria | Cliente-servidor local, análisis de metadatos y exportación CSV/JSON. |

## Tecnologías y conocimientos

| Área | Herramientas y enfoque |
| --- | --- |
| Frontend | JavaScript, TypeScript, HTML, CSS, React, Angular, Bootstrap y Tailwind CSS |
| Backend | Node.js, NestJS, Python, FastAPI, Flask y APIs REST |
| Datos y análisis | SQL, PostgreSQL, MySQL y SQLite; validación, agregaciones, indicadores y exportación CSV/JSON |
| Desarrollo y despliegue | Git, GitHub, VS Code, Docker y GitHub Actions; aprendizaje práctico de Linux |
| Soporte e infraestructura | Atención a usuarios, resolución de incidencias, configuración de equipos, routers y switches, y segmentación de redes |

## En qué me enfoco

- Desarrollar aplicaciones desde la interfaz hasta la API y la persistencia.
- Convertir datos operativos en indicadores comprensibles, con reglas y límites explícitos.
- Documentar contratos, decisiones de arquitectura y pruebas para facilitar el mantenimiento.
- Continuar mi formación en redes, ciberseguridad y servicios cloud.

## Colaboración

Me interesan oportunidades de **desarrollo Full Stack junior y análisis de datos**, así como roles de **soporte TI y sistemas** donde pueda aportar mi experiencia y seguir creciendo.

Puedes explorar mis proyectos y su documentación en [mis repositorios](https://github.com/idrovodario16?tab=repositories).
