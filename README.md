# Diseño y Desarrollo de una API REST Empresarial con Spring Boot

El objetivo es desarrollar una API REST empresarial con Spring Boot 3 para la gestión de productos y pedidos en un e-commerce. El sistema debe incluir arquitectura en capas con controladores REST, servicios de negocio y repositorios JPA; modelado de datos con entidades Product, Order y Customer usando relaciones OneToMany y ManyToMany con Hibernate; autenticación y autorización basada en JWT con Spring Security, incluyendo roles de ADMIN y USER con acceso diferenciado por endpoint; documentación automática con OpenAPI 3.0 y Swagger UI accesible en /api-docs; manejo centralizado de errores con @ControllerAdvice y respuestas estandarizadas en formato JSON; validación de entradas con Bean Validation usando @Valid, @NotNull y @Size; paginación y ordenamiento de resultados en los endpoints de listado usando Pageable; pruebas unitarias con JUnit 5 y Mockito cubriendo la capa de servicio al menos al 80%; pruebas de integración con @SpringBootTest verificando los flujos principales; y containerización con Docker usando Dockerfile multi-stage optimizado para producción.

## Informacion General

| Campo | Valor |
|-------|-------|
| **Tema** | spring-boot-enterprise-architecture |
| **Nivel** | advanced-l2 |
| **Tipo** | practical |
| **Tiempo estimado** | 2 semanas |

## Fases del Reto

### Fase 0: Configuración del Proyecto

**Objetivo:** Obtener el proyecto base funcional enviando el Código Base a un asistente de IA, que lo analizará, corregirá errores y generará un ZIP listo para usar.

**Tiempo estimado:** 15-30 minutos

**Instrucciones:**

- Asegúrate de tener instalado para ejecutar el proyecto: Un IDE o editor de código.
- Copia todo el contenido del campo **Código Base** de este reto — incluyendo el texto de instrucciones que aparece al inicio.
- Abre un asistente de IA (Claude en claude.ai, ChatGPT o Gemini — se recomienda Claude), pega el contenido copiado en el chat y envíalo.
- El asistente analizará los archivos, corregirá errores y generará un archivo ZIP descargable. Descárgalo y extráelo en la carpeta donde quieras trabajar.
- Verifica que el proyecto arranca sin errores.

**Entregable:** El proyecto compila/arranca sin errores.

<details>
<summary>Pistas de conocimiento</summary>

- Copia el Código Base completo incluyendo el texto de instrucciones al inicio — esas instrucciones le indican al asistente exactamente qué hacer con los archivos.
- Si el asistente no genera el ZIP automáticamente al terminar el análisis, escríbele: "genera el ZIP ahora".
- Si el proyecto tiene errores al arrancar, comparte el mensaje de error con el mismo asistente para que lo corrija.

</details>

### Fase 1: Arquitectura y Modelado de Datos

**Objetivo:** Definir la arquitectura en capas y el modelado de datos para la API REST.

**Tiempo estimado:** 3 días

**Instrucciones:**

- Diseñar la arquitectura en capas de la API, incluyendo controladores REST, servicios de negocio y repositorios JPA.
- Modelar las entidades Product, Order y Customer con las relaciones OneToMany y ManyToMany adecuadas.
- Establecer la autenticación y autorización basada en JWT con Spring Security, incluyendo roles de ADMIN y USER con acceso diferenciado por endpoint.

**Entregable:** Diagrama de la arquitectura en capas y modelado de datos con relaciones definidas.

<details>
<summary>Pistas de conocimiento</summary>

- Principios de arquitectura en capas en sistemas empresariales.
- Modelado de relaciones OneToMany y ManyToMany en JPA.
- Implementación de autenticación y autorización con JWT y Spring Security.

</details>

### Fase 2: Implementación de Controladores y Servicios

**Objetivo:** Implementar los controladores REST y los servicios de negocio para la API.

**Tiempo estimado:** 4 días

**Instrucciones:**

- Implementar los controladores REST para los endpoints de productos y pedidos.
- Desarrollar los servicios de negocio que interactúen con los repositorios JPA.
- Asegurar que la documentación automática con OpenAPI 3.0 y Swagger UI esté accesible en /api-docs.

**Entregable:** Controladores REST y servicios de negocio implementados con documentación automática accesible.

<details>
<summary>Pistas de conocimiento</summary>

- Prácticas de desarrollo de controladores REST en Spring Boot.
- Implementación de servicios de negocio que interactúen con repositorios JPA.
- Configuración de OpenAPI 3.0 y Swagger UI para documentación automática.

</details>

### Fase 3: Manejo de Errores y Validación de Entradas

**Objetivo:** Implementar el manejo centralizado de errores y la validación de entradas para la API.

**Tiempo estimado:** 3 días

**Instrucciones:**

- Implementar el manejo centralizado de errores con @ControllerAdvice y respuestas estandarizadas en formato JSON.
- Aplicar validación de entradas con Bean Validation usando @Valid, @NotNull y @Size.
- Asegurar que la paginación y el ordenamiento de resultados en los endpoints de listado estén correctamente implementados usando Pageable.

**Entregable:** Manejo centralizado de errores y validación de entradas implementados con paginación y ordenamiento de resultados.

<details>
<summary>Pistas de conocimiento</summary>

- Prácticas de manejo de errores en Spring Boot con @ControllerAdvice.
- Uso de Bean Validation para validación de entradas en Spring.
- Implementación de paginación y ordenamiento de resultados con Pageable.

</details>

### Fase 4: Pruebas y Containerización

**Objetivo:** Implementar pruebas unitarias y de integración, y containerizar la aplicación con Docker.

**Tiempo estimado:** 4 días

**Instrucciones:**

- Desarrollar pruebas unitarias con JUnit 5 y Mockito cubriendo la capa de servicio al menos al 80%.
- Implementar pruebas de integración con @SpringBootTest verificando los flujos principales.
- Containerizar la aplicación con Docker usando Dockerfile multi-stage optimizado para producción.

**Entregable:** Pruebas unitarias y de integración implementadas, y aplicación containerizada con Docker.

<details>
<summary>Pistas de conocimiento</summary>

- Prácticas de pruebas unitarias y de integración en Spring Boot.
- Uso de JUnit 5 y Mockito para pruebas unitarias.
- Containerización de aplicaciones con Docker y Dockerfile multi-stage.

</details>

## Dimensiones Evaluadas

- **queEs**: ¿Qué es la autenticación y autorización basada en JWT y cómo se implementa en Spring Security?
- **paraQueSirve**: ¿Para qué sirve el manejo centralizado de errores con @ControllerAdvice y cómo se implementa en Spring Boot?
- **comoSeUsa**: ¿Cómo se usa Bean Validation para validar entradas en Spring y cuáles son las anotaciones más comunes?
- **erroresComunes**: ¿Cuáles son los errores comunes al implementar paginación y ordenamiento de resultados con Pageable en Spring Boot?
- **queDecisionesImplica**: ¿Qué decisiones implica la containerización de una aplicación con Docker y cómo se optimiza un Dockerfile para producción?

## Criterios de Evaluacion

- Implementación correcta de la arquitectura en capas y el modelado de datos.
- Desarrollo de controladores REST y servicios de negocio funcionales.
- Manejo centralizado de errores y validación de entradas correctamente implementados.
- Pruebas unitarias y de integración que cubren adecuadamente la capa de servicio.
- Aplicación containerizada con Docker y Dockerfile optimizado para producción.

## Como trabajar con un asistente de IA

- **AGENTS.md** — instrucciones nativas del repo (Cursor, Codex, Copilot, Gemini, Claude Code). Abrí el proyecto y el agente las carga solo.
- **PROMPT_MEJORA.md** — el mismo prompt, para copiar y pegar en un chat (claude.ai, ChatGPT, etc.).

---

*Reto generado automaticamente por Challenge Generator - Pragma*
