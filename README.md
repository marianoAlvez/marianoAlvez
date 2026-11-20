# Mariano Alvez

**Senior Software Engineer | Arquitectura de software, Backend y Full Stack**

Diseño APIs e integraciones para productos SaaS, pagos y reservas. Trabajo desde el modelado del dominio hasta las pruebas y el soporte en producción. En este perfil comparto decisiones que se pueden poner a prueba.

## Posta · ¿Cuándo volverías a comprar una etiqueta de envío?

Una tienda pide una etiqueta. El transportista cobra y se pierde la respuesta. Si la tienda le compra a otro, puede terminar pagando dos veces el mismo despacho.

En **Posta** comparo las dos decisiones con el mismo pedido. En el segundo 3 podés alternar entre comprar en otro transportista y verificar la referencia original. Verificar evita el segundo cargo en ese ensayo, a costa de dejar el despacho pendiente mientras el proveedor no responda. Usé **Rust y PostgreSQL** para conservar la emisión y su evento en la misma transacción. Una prueba entrega el evento a dos consumidores al mismo tiempo y comprueba que queda un solo registro de auditoría.

**[Recorrer la demo](https://marianoalvez.github.io/carrier-failover-lab/)** · [Leer la decisión de arquitectura](https://github.com/marianoAlvez/carrier-failover-lab/blob/main/docs/adr/001-eventos-de-emision.md) · [Ver el código y las pruebas](https://github.com/marianoAlvez/carrier-failover-lab)

## Otros casos de arquitectura

Estas demos de portafolio utilizan datos ficticios y se desarrollaron con asistencia de IA. Los proyectos profesionales aparecen más abajo.

| Proyecto | Qué permite comprobar | Recorrido |
| --- | --- | --- |
| [**Inventario multirregión**](https://github.com/marianoAlvez/regional-inventory-tradeoffs) | Quórum y cupos regionales cuando dos sedes venden el mismo stock y pierden comunicación. | [Comparar qué pedidos se confirman](https://marianoalvez.github.io/regional-inventory-tradeoffs/). |
| [**Traspaso de autoridad contable**](https://github.com/marianoAlvez/ledger-authority-cutover) | Cambio del sistema que puede escribir sobre una cuenta mientras otras siguen operando. | [Seguir una escritura tardía durante la migración](https://marianoalvez.github.io/ledger-authority-cutover/). |
| [**Reliable Webhooks Lab**](https://github.com/marianoAlvez/reliable-webhooks-lab) | API NestJS/TypeScript, firma HMAC, idempotencia, inbox/outbox transaccional en SQLite, reintentos y recuperación de entregas. | Enviar un evento, repetirlo, provocar un fallo y observar su recuperación. Incluye contrato OpenAPI y pruebas. |
| [**AI Review Workbench**](https://github.com/marianoAlvez/ai-review-workbench) | API Python/FastAPI e interfaz React/TypeScript; proveedores intercambiables, validación de respuestas estructuradas y manejo de errores. | Analizar un requerimiento ficticio con el proveedor simulado; revisar riesgos, preguntas y criterios. Incluye pruebas y evaluación reproducible. |

Cada repositorio explica cómo ejecutarlo, las decisiones adoptadas y los límites de la demostración. Las pruebas del proveedor simulado no equivalen a una evaluación de precisión de un modelo real.

## Arquitectura y backend

- Diseño de arquitecturas modulares, microservicios y soluciones híbridas según el contexto del producto; modelado de dominios, responsabilidades, contratos API y datos.
- APIs REST y Backend for Frontend (BFF) con TypeScript/JavaScript, Node.js, NestJS y Express; APIs y servicios con Python/FastAPI y Go.
- Persistencia e integración de datos con PostgreSQL, TypeORM, MySQL y MongoDB; procesamiento asíncrono con Redis y BullMQ.
- CQRS, integración por eventos, idempotencia, reintentos y recuperación de errores. Webhooks, autenticación, autorización y trazabilidad de procesos.

## Frontend y mobile

Mis capacidades de desarrollo web incluyen **Angular, React y Vue**, junto con TypeScript, JavaScript, HTML y CSS/SASS. En mobile trabajo con **Flutter y Dart**. Integro interfaces, estados, validaciones, autenticación y servicios backend para construir funcionalidades completas de producto.

## IA aplicada, integraciones y entrega

Desarrollo herramientas e integraciones con **OpenAI y Gemini**, separación entre proveedores y lógica de negocio, validación de respuestas y automatización de contenidos. Trabajo con Docker, AWS, CI/CD, GitHub Actions, Jest y Playwright, documentación técnica y soporte de aplicaciones.

## Experiencia aplicada en proyectos

Estos casos describen contribuciones profesionales. Las demostraciones públicas del portafolio son implementaciones independientes.

| Proyecto | Contribución técnica |
| --- | --- |
| **AMB** | Backend con NestJS, TypeScript, PostgreSQL, TypeORM y CQRS; Redis y pruebas con Jest. |
| **CENTERBROK** | Portal de casos con Vue 3 y NestJS; máquina de estados, JWT, tareas BullMQ/Redis, notificaciones, almacenamiento S3 y trazabilidad. |
| **HazloPosible** | Generación de cursos con OpenAI/Gemini, abstracción de proveedores, validación de respuestas, procesamiento asíncrono y exportaciones IMS Common Cartridge/Moodle. |
| **Kangoo** | Stripe Connect, onboarding, pagos y facturación; validaciones backend, permisos y sincronización de estados mediante webhooks. |
| **HostAndBoat** | Angular/NestJS, integración y normalización de múltiples proveedores, disponibilidad y reservas; importaciones batch, cron y colas. |
| **Universidad Siglo 21** | BFFs Node.js, aplicación Flutter para estudiantes y APIs NestJS para ecommerce y cupones, trabajando desde Churrasco.cc junto a equipos de BitLogic y Vates. |
| **Delectatech** | Desarrollo full stack, integración frontend/backend, QA, documentación y soporte actual a Finder MVP2. |

## Trayectoria profesional

- **Lázzaro — Ingeniero de software:** abril de 2024-actualidad. Desarrollo para clientes de software factory.
- **Churrasco.cc — Desarrollador Web Ssr., Angular y Flutter:** marzo de 2022-abril de 2024. Proyectos para Universidad Siglo 21 con equipos de BitLogic (marzo de 2022-abril de 2023) y Vates (mayo de 2023-abril de 2024).
- **Freelance — Desarrollador de aplicaciones web:** abril de 2021-marzo de 2022. Trabajos pagos para clientes.
- **Coderhouse — Tutor de Programación Backend con Node.js:** febrero de 2022-junio de 2025. Tutor Angular: diciembre de 2021-abril de 2024.

Colaboraciones actuales con **SmartAoS e Innovaslab** y soporte a **Delectatech**.

## Competencias técnicas

| Área | Tecnologías y prácticas |
| --- | --- |
| Lenguajes | TypeScript, JavaScript, Python, Go, Dart y SQL. Rust aplicado en el laboratorio Posta. |
| Backend | Node.js, NestJS, Express, FastAPI, REST, BFF y Swagger/OpenAPI. |
| Frontend | Angular, React, Vue, Angular Material, RxJS, HTML, CSS/SASS. |
| Mobile | Flutter y Dart. |
| Datos y asincronía | PostgreSQL, MySQL, MongoDB, TypeORM, Redis y BullMQ. |
| Arquitectura e integración | Diseño modular, microservicios, CQRS, modelado de dominios, eventos, webhooks, idempotencia y reintentos. |
| Calidad y entrega | Docker, AWS, Git, GitHub Actions, CI/CD, Jest, Playwright, documentación y soporte. |

## Ubicación, idiomas y contacto

**Oberá, Misiones, Argentina.** Interés en oportunidades remotas de ingeniería de software, backend, full stack y arquitectura aplicada.

**Español:** nativo. **Inglés:** lectura de documentación técnica; sin comunicación oral en inglés.

[LinkedIn](https://www.linkedin.com/in/mariano-alvez/) · [GitHub](https://github.com/marianoAlvez)
