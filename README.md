# personal-copilot-instructions

Repositorio de instrucciones personalizadas para GitHub Copilot. Este proyecto sirve como template para definir reglas y convenciones que Copilot debe seguir al generar código, documentación, mensajes de commit y revisiones en proyectos de software.

## ¿Qué hace este proyecto?

Centraliza y define instrucciones detalladas para adaptar el comportamiento de Copilot a las necesidades y convenciones de equipos o proyectos. Incluye instrucciones para generación de código, documentación, mensajes de commit, revisiones de código y más.

## Estructura del proyecto

- `.github/instructions/`: Archivos de instrucciones para distintos contextos de Copilot.
  - `copilot-coding.instructions.md`: Reglas para generación de código.
  - `copilot-docs.instructions.md`: Reglas para documentación.
  - `copilot-explains.instructions.md`: Reglas para explicaciones de código.
  - `copilot-review.instructions.md`: Reglas para revisión de código.
  - `commit-messages.instructions.md`: Reglas para mensajes de commit.
  - `copilot-api-doc.instructions.md`: Reglas para documentación de APIs.
  - `copilot-readme.instructions.md`: Reglas para generación de README.
- `README.md`: Este archivo.

## Variables de entorno requeridas

No se requieren variables de entorno para el funcionamiento de este repositorio.

## Cómo usar este template

1. Copia los archivos de instrucciones a la carpeta `.github/instructions/` de tu proyecto.
2. Configura tu entorno de Copilot para que lea estas instrucciones (requiere integración personalizada o herramientas compatibles).
3. Adapta las instrucciones según las convenciones de tu equipo o proyecto.

## Notas adicionales

- Si tu proyecto es una API, consulta el archivo `API_DOC.md` para ver ejemplos de documentación generada.
- Si necesitas adaptar las instrucciones a otro idioma o convención, edita los archivos en `.github/instructions/`.

---
Este README reemplaza cualquier documentación previa sobre la estructura y propósito de este repositorio.