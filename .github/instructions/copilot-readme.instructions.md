---
applyTo: "**"
---

# Instrucciones para generación de README con Copilot

- Antes de generar o actualizar el README, **analiza obligatoriamente la estructura y los archivos reales del proyecto** (incluyendo archivos y carpetas presentes en el sistema de archivos).
- Solo incluye secciones en el README que correspondan a archivos o configuraciones realmente detectados en el proyecto. **No generes secciones genéricas ni plantillas.**
- Si el archivo README ya existe, **preserva y adapta el contenido existente** al nuevo formato, nunca elimines información relevante.
- El README debe comenzar con el nombre del proyecto y una breve descripción de su propósito.
- Explica claramente qué hace el proyecto y su caso de uso principal.
- Si el proyecto es grande y tiene una estructura algo compleja de archivos, incluye una sección de estructura del proyecto, detallando los directorios y archivos principales.
- Solo añade una sección de variables de entorno requeridas si existen archivos `.env`, referencias a variables de entorno en el código (por ejemplo, `process.env`), o documentación relacionada en el proyecto. Si no existen, **no incluyas ninguna sección de variables de entorno**.
- Si el proyecto necesita comandos para inciarse, como npm i, python install requirements o el comando similar al lenguaje del proyecto, incluye una sección de "Cómo iniciar el proyecto" con los pasos necesarios para la instalación y ejecución
- Si existe un archivo `.devcontainer`, explica cómo usar el entorno de desarrollo remoto con VS Code. Si no existe, **no incluyas ninguna sección sobre Devcontainer**.
- Si existe un archivo `docker-compose.yml`, explica cómo levantar el entorno con Docker Compose, incluyendo los comandos necesarios. Si no existe, **no incluyas ninguna sección sobre Docker Compose**.
- Si el proyecto tiene un archivo `package.json`, documenta los comandos disponibles (scripts) y su función. Si no existe, **no incluyas ninguna sección sobre scripts de package.json**.
- Si el proyecto es una API, genera un archivo adicional `API_DOC.md` que explique los endpoints, métodos, parámetros, respuestas y ejemplos de uso.
- **No incluyas secciones sobre Docker Compose, Devcontainer, scripts de package.json, variables de entorno, etc., si los archivos o referencias correspondientes no existen en el proyecto.**
- El README debe ser siempre una adaptación fiel al contexto y archivos presentes, evitando plantillas genéricas.
- Si el proyecto tiene pruebas, explica cómo ejecutarlas.
- Si el proyecto tiene integración continua o despliegue automatizado (como una github action), documenta el flujo básico solo si aplica.
- **Utiliza emojis y elementos visuales llamativos (tablas, listas, bloques destacados) para mejorar la legibilidad y hacer el README más atractivo.**

