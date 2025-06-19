---
applyTo: "**"
---

# Instrucciones para generación de README con Copilot

- Antes de generar o actualizar el README, analiza la estructura y los archivos reales del proyecto.
- Si el archivo README ya existe, **preserva y adapta el contenido existente** al nuevo formato, nunca elimines información relevante.
- El README debe comenzar con el nombre del proyecto y una breve descripción de su propósito.
- Explica claramente qué hace el proyecto y su caso de uso principal.
- Incluye una sección de estructura del proyecto, detallando los directorios y archivos principales.
- Añade una sección de variables de entorno requeridas, explicando cada variable y su propósito, solo si existen variables de entorno en el proyecto.
- Incluye una sección de "Cómo iniciar el proyecto" con los pasos necesarios para la instalación y ejecución.
- Si existe un archivo `.devcontainer`, explica cómo usar el entorno de desarrollo remoto con VS Code.
- Si existe un archivo `docker-compose.yml`, explica cómo levantar el entorno con Docker Compose, incluyendo los comandos necesarios.
- Si el proyecto tiene un archivo `package.json`, documenta los comandos disponibles (scripts) y su función.
- Si el proyecto es una API, genera un archivo adicional `API_DOC.md` que explique los endpoints, métodos, parámetros, respuestas y ejemplos de uso.
- **No incluyas secciones sobre Docker Compose, Devcontainer, scripts de package.json, etc., si los archivos correspondientes no existen en el proyecto.**
- El README debe ser siempre una adaptación fiel al contexto y archivos presentes, evitando plantillas genéricas.
- Si el proyecto requiere pasos de configuración adicionales (migraciones, seeds, etc.), documenta el proceso solo si aplica.
- Si el proyecto tiene dependencias externas importantes, menciónalas y justifica su uso.
- Si el proyecto tiene pruebas, explica cómo ejecutarlas.
- Si el proyecto tiene integración continua o despliegue automatizado, documenta el flujo básico solo si aplica.
- Si el README reemplaza o depreca otro archivo, indícalo claramente.
- **Utiliza emojis y elementos visuales llamativos (tablas, listas, bloques destacados) para mejorar la legibilidad y hacer el README más atractivo.**
