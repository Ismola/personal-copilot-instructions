---
applyTo: "**"
---

# Instrucciones para generación de mensajes de commit

- Los mensajes de commit deben seguir estrictamente el estándar [Conventional Commits](https://www.conventionalcommits.org/).
- Incluye siempre un emoji relevante al tipo de commit al inicio del mensaje (por ejemplo: ✨, 🐛, ♻️, 🚀, 📝, 🔥, 🚑️, ⬆️, ⬇️, etc).
- El mensaje debe tener el siguiente formato:
  ```
  <emoji> <type>[optional scope]: <short summary>
  
  <detailed description explaining what, why and how>
  ```
- Usa los tipos estándar: feat, fix, docs, style, refactor, perf, test, build, ci, chore, revert.
- El resumen debe ser breve (máx. 72 caracteres), en minúsculas y sin punto final.
- La descripción debe ser detallada, explicando claramente qué se hizo, por qué y cómo.
- Si aplica, incluye referencias a issues o tareas relacionadas.
- Ejemplo:
  ```
  ✨ feat(auth): añade soporte para login con YubiKey

  Se implementa la autenticación usando YubiKey para mejorar la seguridad. 
  Se actualizan los controladores y se agregan pruebas unitarias. Relacionado con #42.
  ```

# Instrucciones adicionales para generación de mensajes de commit

- Siempre que sea posible, referencia issues, tareas o tickets relacionados usando el formato estándar (por ejemplo: `Relacionado con #123` o `Refs #123`).
- Si el proyecto lo requiere, escribe los mensajes de commit en inglés o español según el idioma predominante del repositorio.
- Evita mensajes genéricos como "update", "fix bug" o "minor changes". Sé específico sobre el cambio realizado.
- Si el commit introduce breaking changes, indícalo claramente en la descripción usando la sección `BREAKING CHANGE:` y explica el impacto.
- Para cambios que afectan la seguridad, usa el tipo `fix` y describe el riesgo mitigado.
- Si el commit es resultado de un merge o revert, usa los tipos `merge` o `revert` y explica el contexto.
- Para refactorizaciones sin cambio de funcionalidad, usa `refactor` y explica la motivación.
- Si el commit solo actualiza dependencias, usa `chore(deps)` y especifica los paquetes afectados.
- Ejemplos adicionales:
  ```
  🐛 fix(api): corrige error de validación en endpoint de usuarios

  Se soluciona un problema donde la validación de emails permitía valores inválidos.
  Relacionado con #56.
  ```

  ```
  ♻️ refactor(core): simplifica lógica de manejo de errores

  Se reorganiza el flujo de control para mejorar la legibilidad y facilitar futuras extensiones.
  No se modifica la funcionalidad existente.
  ```

  ```
  🚨 fix(security): actualiza dependencia vulnerable

  Se actualiza express de 4.17.1 a 4.18.2 para mitigar vulnerabilidad CVE-2022-12345.
  ```

  ```
  ⚠️ feat(config): añade soporte para múltiples entornos

  Se permite configurar variables de entorno para desarrollo, pruebas y producción.
  BREAKING CHANGE: la configuración previa en config.js ya no es compatible.
  ```

# Casos de uso adicionales y convenciones específicas

- Para cambios relacionados con la accesibilidad, usa el tipo `feat(a11y)` o `fix(a11y)` y describe el impacto en la experiencia de usuario.
- Para mejoras de internacionalización/localización, usa `feat(i18n)` o `fix(i18n)` y especifica los idiomas afectados.
- Para cambios en la documentación técnica, usa `docs` y especifica el área afectada (por ejemplo, `docs(readme)`).
- Para cambios en scripts de automatización, usa `chore(scripts)` y describe el propósito del script.
- Para cambios en configuraciones de herramientas de desarrollo (linters, formatters, etc.), usa `chore(config)` y detalla la herramienta.
- Para cambios en archivos de configuración de CI/CD, usa `ci` y especifica el proveedor o flujo afectado.
- Para mejoras de rendimiento, usa `perf` y explica la optimización realizada y su impacto.
- Para cambios en el diseño visual (CSS, temas, etc.), usa `style(ui)` y describe el ajuste visual.
- Para cambios en la estructura del proyecto (mover, renombrar carpetas/archivos), usa `chore(structure)` y explica la motivación.
- Para agregar o actualizar ejemplos de código, usa `docs(examples)` y describe el ejemplo añadido o modificado.
- Para cambios en archivos de licencia o avisos legales, usa `chore(legal)` y especifica el archivo.
- Para cambios temporales o experimentales, usa el tipo `feat(experimental)` y documenta claramente la naturaleza experimental.
- Para cambios en el sistema de logging, usa `feat(logging)` o `fix(logging)` y explica el ajuste.
- Para cambios en la gestión de errores, usa `fix(errors)` o `refactor(errors)` y detalla la mejora.
- Para cambios en la interfaz de línea de comandos (CLI), usa `feat(cli)` o `fix(cli)` y describe el cambio.
- Para cambios en la integración con APIs externas, usa `feat(api)` o `fix(api)` y especifica la API.
- Para cambios en la gestión de dependencias internas, usa `chore(deps-internal)` y detalla el paquete.
- Para cambios en la configuración de entornos de desarrollo, usa `chore(env)` y explica el ajuste.
- Para cambios en la gestión de versiones, usa `chore(release)` y describe el cambio.
- Para cambios en la configuración de Docker, usa `chore(docker)` y especifica el ajuste.
- Para cambios en la configuración de seguridad (headers, CORS, etc.), usa `fix(security)` y detalla la mitigación.
- Para cambios en la gestión de sesiones o autenticación, usa `feat(auth)` o `fix(auth)` y explica el cambio.
- Para cambios en la gestión de caché, usa `feat(cache)` o `fix(cache)` y describe el ajuste.
- Para cambios en la integración con servicios de terceros, usa `feat(integration)` o `fix(integration)` y especifica el servicio.
- Para cambios en la configuración de monitoreo o métricas, usa `feat(monitoring)` o `fix(monitoring)` y detalla el ajuste.
- Para cambios en la gestión de colas o tareas asíncronas, usa `feat(queue)` o `fix(queue)` y explica el cambio.
- Para cambios en la gestión de archivos o almacenamiento, usa `feat(storage)` o `fix(storage)` y describe el ajuste.
- Para cambios en la configuración de redes o proxies, usa `chore(network)` y detalla el cambio.
- Para cambios en la gestión de permisos o roles, usa `feat(permissions)` o `fix(permissions)` y explica el ajuste.
- Para cambios en la gestión de notificaciones, usa `feat(notifications)` o `fix(notifications)` y describe el cambio.
- Para cambios en la configuración de backups o restauraciones, usa `chore(backup)` y detalla el ajuste.
- Para cambios en la gestión de logs de auditoría, usa `feat(audit)` o `fix(audit)` y explica el cambio.
- Para cambios en la configuración de analítica, usa `feat(analytics)` o `fix(analytics)` y describe el ajuste.
- Para cambios en la gestión de pagos o facturación, usa `feat(billing)` o `fix(billing)` y detalla el cambio.
- Para cambios en la gestión de usuarios, usa `feat(users)` o `fix(users)` y explica el ajuste.
- Para cambios en la gestión de productos o catálogos, usa `feat(products)` o `fix(products)` y describe el cambio.
- Para cambios en la gestión de órdenes o transacciones, usa `feat(orders)` o `fix(orders)` y detalla el ajuste.
- Para cambios en la gestión de inventario, usa `feat(inventory)` o `fix(inventory)` y explica el cambio.
- Para cambios en la gestión de reportes, usa `feat(reports)` o `fix(reports)` y describe el ajuste.
- Para cambios en la gestión de comentarios o reseñas, usa `feat(comments)` o `fix(comments)` y detalla el cambio.
- Para cambios en la gestión de imágenes o multimedia, usa `feat(media)` o `fix(media)` y explica el ajuste.
- Para cambios en la gestión de búsqueda, usa `feat(search)` o `fix(search)` y describe el cambio.
- Para cambios en la gestión de etiquetas o categorías, usa `feat(tags)` o `fix(tags)` y detalla el ajuste.
- Para cambios en la gestión de preferencias o configuraciones de usuario, usa `feat(settings)` o `fix(settings)` y explica el cambio.
- Para cambios en la gestión de rutas o navegación, usa `feat(routing)` o `fix(routing)` y describe el ajuste.
- Para cambios en la gestión de formularios, usa `feat(forms)` o `fix(forms)` y detalla el cambio.
- Para cambios en la gestión de emails o comunicaciones, usa `feat(email)` o `fix(email)` y explica el ajuste.
- Para cambios en la gestión de archivos estáticos, usa `chore(static)` y detalla el cambio.
- Para cambios en la gestión de seeds o datos de prueba, usa `chore(seeds)` y describe el ajuste.
- Para cambios en la gestión de migraciones de base de datos, usa `chore(migrations)` y explica el cambio.
- Para cambios en la gestión de fixtures de pruebas, usa `test(fixtures)` y detalla el ajuste.
- Para cambios en la gestión de mocks o stubs, usa `test(mocks)` y describe el cambio.
- Para cambios en la gestión de snapshots de pruebas, usa `test(snapshots)` y explica el ajuste.
- Para cambios en la gestión de coverage de pruebas, usa `test(coverage)` y detalla el cambio.
- Para cambios en la gestión de integración continua, usa `ci` y especifica el flujo afectado.
- Para cambios en la gestión de despliegues, usa `ci(deploy)` y describe el ajuste.
- Para cambios en la gestión de rollback, usa `ci(rollback)` y explica el cambio.
- Para cambios en la gestión de pipelines, usa `ci(pipeline)` y detalla el ajuste.
- Para cambios en la gestión de artefactos, usa `ci(artifacts)` y describe el cambio.
- Para cambios en la gestión de versiones de API, usa `feat(api-versioning)` o `fix(api-versioning)` y explica el ajuste.
- Para cambios en la gestión de políticas de seguridad, usa `fix(security-policy)` y detalla el cambio.
- Para cambios en la gestión de recursos compartidos, usa `feat(shared)` o `fix(shared)` y describe el ajuste.
- Para cambios en la gestión de utilidades o helpers, usa `feat(utils)` o `fix(utils)` y explica el cambio.
- Para cambios en la gestión de hooks, usa `feat(hooks)` o `fix(hooks)` y detalla el ajuste.
- Para cambios en la gestión de middlewares, usa `feat(middleware)` o `fix(middleware)` y describe el cambio.
- Para cambios en la gestión de providers, usa `feat(provider)` o `fix(provider)` y explica el ajuste.
- Para cambios en la gestión de servicios, usa `feat(service)` o `fix(service)` y detalla el cambio.
- Para cambios en la gestión de controladores, usa `feat(controller)` o `fix(controller)` y describe el cambio.
- Para cambios en la gestión de modelos, usa `feat(model)` o `fix(model)` y explica el ajuste.
- Para cambios en la gestión de repositorios, usa `feat(repository)` o `fix(repository)` y detalla el cambio.
- Para cambios en la gestión de validaciones, usa `feat(validation)` o `fix(validation)` y describe el cambio.
- Para cambios en la gestión de serializadores, usa `feat(serializer)` o `fix(serializer)` y explica el ajuste.
- Para cambios en la gestión de adaptadores, usa `feat(adapter)` o `fix(adapter)` y detalla el cambio.
- Para cambios en la gestión de factories, usa `feat(factory)` o `fix(factory)` y describe el cambio.
- Para cambios en la gestión de decoradores, usa `feat(decorator)` o `fix(decorator)` y explica el ajuste.
- Para cambios en la gestión de directivas, usa `feat(directive)` o `fix(directive)` y detalla el cambio.
- Para cambios en la gestión de pipes, usa `feat(pipe)` o `fix(pipe)` y describe el cambio.
- Para cambios en la gestión de guards, usa `feat(guard)` o `fix(guard)` y explica el ajuste.
- Para cambios en la gestión de resolvers, usa `feat(resolver)` o `fix(resolver)` y detalla el cambio.
- Para cambios en la gestión de interceptors, usa `feat(interceptor)` o `fix(interceptor)` y describe el cambio.
- Para cambios en la gestión de esquemas, usa `feat(schema)` o `fix(schema)` y explica el ajuste.
- Para cambios en la gestión de DTOs, usa `feat(dto)` o `fix(dto)` y detalla el cambio.
- Para cambios en la gestión de entidades, usa `feat(entity)` o `fix(entity)` y describe el cambio.
- Para cambios en la gestión de migraciones, usa `chore(migration)` y explica el ajuste.
- Para cambios en la gestión de seeds, usa `chore(seed)` y detalla el cambio.
- Para cambios en la gestión de fixtures, usa `test(fixture)` y describe el ajuste.
- Para cambios en la gestión de mocks, usa `test(mock)` y explica el cambio.
- Para cambios en la gestión de snapshots, usa `test(snapshot)` y detalla el ajuste.
- Para cambios en la gestión de coverage, usa `test(coverage)` y describe el cambio.
- Para cambios en la gestión de integración continua, usa `ci` y especifica el flujo afectado.
- Para cambios en la gestión de despliegues, usa `ci(deploy)` y describe el ajuste.
- Para cambios en la gestión de rollback, usa `ci(rollback)` y explica el cambio.
- Para cambios en la gestión de pipelines, usa `ci(pipeline)` y detalla el ajuste.
- Para cambios en la gestión de artefactos, usa `ci(artifacts)` y describe el cambio.

# Consideraciones finales

- Si el commit abarca varios ámbitos, prioriza el más relevante o usa scopes múltiples separados por coma.
- Si el cambio es menor pero necesario, usa `chore` y explica la razón.
- Si el commit es experimental, indícalo claramente en el scope o en la descripción.
- Si el commit es temporal, añade una nota en la descripción para su posterior revisión.
- Si el commit revierte un cambio, usa `revert` y referencia el commit revertido.
- Si el commit es un merge, usa `merge` y explica el contexto.
- Si el commit es para pruebas internas, usa `test(internal)` y detalla el propósito.
- Si el commit es para pruebas de integración, usa `test(integration)` y describe el ajuste.
- Si el commit es para pruebas de aceptación, usa `test(acceptance)` y explica el cambio.
- Si el commit es para pruebas de regresión, usa `test(regression)` y detalla el ajuste.
- Si el commit es para pruebas de carga, usa `test(load)` y describe el cambio.
- Si el commit es para pruebas de seguridad, usa `test(security)` y explica el ajuste.
- Si el commit es para pruebas de usabilidad, usa `test(usability)` y detalla el cambio.
- Si el commit es para pruebas de accesibilidad, usa `test(a11y)` y describe el ajuste.
- Si el commit es para pruebas de rendimiento, usa `test(perf)` y explica el cambio.
- Si el commit es para pruebas de compatibilidad, usa `test(compat)` y detalla el ajuste.
- Si el commit es para pruebas de integración continua, usa `ci(test)` y describe el ajuste.
- Si el commit es para pruebas de despliegue, usa `ci(deploy-test)` y explica el cambio.
- Si el commit es para pruebas de rollback, usa `ci(rollback-test)` y detalla el ajuste.
- Si el commit es para pruebas de pipelines, usa `ci(pipeline-test)` y describe el cambio.
- Si el commit es para pruebas de artefactos, usa `ci(artifacts-test)` y explica el ajuste.
