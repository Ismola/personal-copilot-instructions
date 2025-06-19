---
applyTo: "**"
---

# Instrucciones para generación de documentación de API (API_DOC.md) con Copilot

- El archivo debe llamarse `API_DOC.md` y estar en la raíz del proyecto o en la carpeta docs.
- Incluye una introducción breve sobre la API y su propósito.
- Documenta todos los endpoints disponibles, agrupados por recurso o funcionalidad.
- Para cada endpoint, especifica:
  - Método HTTP (GET, POST, PUT, DELETE, etc.)
  - Ruta del endpoint
  - Descripción de la funcionalidad
  - Parámetros de entrada (query, path, body), indicando si son obligatorios u opcionales
  - Ejemplo de request y response (en JSON u otro formato relevante)
  - Códigos de respuesta posibles y su significado
  - Notas de seguridad o autenticación si aplica
- Si hay versiones de API, documenta las diferencias principales.
- Si hay límites de uso, cuotas o restricciones, explícalos.
- Usa tablas o ejemplos claros para mejorar la legibilidad.
- Si la API requiere autenticación, explica el mecanismo (token, JWT, OAuth, etc.).
- Si la API tiene errores comunes, documenta los mensajes y cómo resolverlos.
- Usa el idioma predominante del proyecto.
