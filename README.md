# 🚀 personal-copilot-instructions

🎯 **Template de instrucciones personalizadas para GitHub Copilot**  
Define reglas y convenciones para mejorar la generación de código, documentación, mensajes de commit y revisiones en tus proyectos.

---

## ⚡ Añade las instrucciones a tu proyecto en segundos

Si ya tienes un repositorio y quieres añadir estas instrucciones, ejecuta este comando en la raíz de tu proyecto:

### 🐧 Linux / 🐱 MacOS

```bash
git clone --depth=1 https://github.com/Ismola/personal-copilot-instructions tmp-copilot-instructions \
  && mkdir -p .github \
  && rm -rf .github/instructions \
  && mv tmp-copilot-instructions/.github/instructions .github/ \
  && rm -rf tmp-copilot-instructions
```

### 🪟 Windows (PowerShell)

```powershell
git clone --depth=1 https://github.com/Ismola/personal-copilot-instructions tmp-copilot-instructions
New-Item -ItemType Directory -Force -Path .github | Out-Null
Remove-Item .github\instructions -Recurse -Force -ErrorAction SilentlyContinue
Move-Item tmp-copilot-instructions\.github\instructions .github\
Remove-Item tmp-copilot-instructions -Recurse -Force
```

> 💡 **Esto reemplazará la carpeta `.github/instructions` de tu proyecto por la de este repositorio.**

---

## 📚 ¿Qué hace este proyecto?

Centraliza y define instrucciones detalladas para adaptar el comportamiento de Copilot a las necesidades y convenciones de equipos o proyectos.  
Incluye instrucciones para generación de código, documentación, mensajes de commit, revisiones de código y más.

---

## 🗂️ Estructura del proyecto

| Carpeta/Archivo                | Descripción                                               |
|--------------------------------|-----------------------------------------------------------|
| `.github/instructions/`        | Archivos de instrucciones para distintos contextos Copilot|
| ├─ `copilot-coding.instructions.md`   | Reglas para generación de código                |
| ├─ `copilot-docs.instructions.md`     | Reglas para documentación                       |
| ├─ `copilot-explains.instructions.md` | Reglas para explicaciones de código              |
| ├─ `copilot-review.instructions.md`   | Reglas para revisión de código                   |
| ├─ `commit-messages.instructions.md`  | Reglas para mensajes de commit                   |
| ├─ `copilot-api-doc.instructions.md`  | Reglas para documentación de APIs                |
| ├─ `copilot-readme.instructions.md`   | Reglas para generación de README                 |
| `README.md`                    | Este archivo                                            |

---

## 🔑 Variables de entorno requeridas

No se requieren variables de entorno para el funcionamiento de este repositorio.

---

## 💡 Notas adicionales

- Si tu proyecto es una API, consulta el archivo `API_DOC.md` para ver ejemplos de documentación generada.
- Si necesitas adaptar las instrucciones a otro idioma o convención, edita los archivos en `.github/instructions/`.

---

## 🧠 ¿Cómo cambia Copilot con estas instrucciones?

Al añadir estas instrucciones a tu proyecto, Copilot adaptará su comportamiento para ajustarse a tus convenciones y necesidades.  
A continuación, se resumen las reglas incluidas:

| Archivo de instrucciones                       | ¿Qué cambia en Copilot?                                                                                 |
|------------------------------------------------|---------------------------------------------------------------------------------------------------------|
| `copilot-coding.instructions.md`               | Genera código más claro, legible y seguro, siguiendo tus convenciones y buenas prácticas.               |
| `copilot-docs.instructions.md`                 | Crea documentación atractiva, concisa y útil, con ejemplos y emojis para mejor legibilidad.             |
| `copilot-explains.instructions.md`             | Explica el código de forma clara, en pasos si es complejo, y menciona riesgos, patrones y contexto.     |
| `copilot-review.instructions.md`               | Revisa el código buscando errores, mejoras y cumplimiento de convenciones, sugiriendo refactorizaciones.|
| `commit-messages.instructions.md`              | Genera mensajes de commit siguiendo Conventional Commits, con emojis y descripciones detalladas.         |
| `copilot-api-doc.instructions.md`              | Documenta APIs de forma estructurada, con ejemplos, parámetros, respuestas y notas de seguridad.         |
| `copilot-readme.instructions.md`               | Crea READMEs claros, visuales y completos, explicando estructura, comandos y configuración del proyecto.|

> ⚡ **Con estas reglas, Copilot será mucho más útil, consistente y alineado con tu equipo o proyecto.**

---

> 📝 **Este README reemplaza cualquier documentación previa sobre la estructura y propósito de este repositorio.**