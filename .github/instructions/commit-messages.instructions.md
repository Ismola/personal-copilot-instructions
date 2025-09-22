---
applyTo: "**"
---

# Instrucciones para Mensajes de Commit - Proyecto General

## Estándar de Conventional Commits con Emojis

Todos los mensajes de commit deben seguir el formato de **Conventional Commits** incluyendo emojis apropiados.

### Formato:
```
<emoji> <tipo>[ámbito opcional]: <descripción>

[cuerpo opcional]

[pie(s) opcional(es)]
```

### Tipos de Commit con Emojis:

#### 🚀 **feat**: Nueva funcionalidad
- `🚀 feat: agregar autenticación de usuarios`
- `✨ feat(auth): implementar login con Google`

#### 🐛 **fix**: Corrección de errores
- `🐛 fix: corregir error de validación en formulario`
- `🔧 fix(api): resolver problema de timeout en peticiones`

#### 📚 **docs**: Documentación
- `📚 docs: actualizar README con instrucciones de instalación`
- `📖 docs(api): agregar documentación de endpoints`

#### 🎨 **style**: Formato de código (sin cambios de lógica)
- `🎨 style: formatear código según ESLint`
- `💄 style: mejorar diseño del botón de login`

#### ♻️ **refactor**: Refactorización de código
- `♻️ refactor: simplificar lógica de autenticación`
- `🔨 refactor(utils): optimizar funciones de validación`

#### ✅ **test**: Agregar o modificar tests
- `✅ test: agregar tests para servicio de usuarios`
- `🧪 test(auth): implementar tests de integración`

#### 📦 **build**: Cambios en el sistema de build
- `📦 build: actualizar dependencias de desarrollo`
- `⚙️ build(docker): optimizar configuración de contenedores`

#### 🔄 **ci**: Cambios en CI/CD
- `🔄 ci: configurar GitHub Actions para tests automáticos`
- `🚀 ci: mejorar pipeline de despliegue`

#### 🧹 **chore**: Tareas de mantenimiento
- `🧹 chore: limpiar archivos temporales`
- `🔧 chore: actualizar configuración de ESLint`

#### ⚡ **perf**: Mejoras de rendimiento
- `⚡ perf: optimizar consultas a la base de datos`
- `🚀 perf(client): implementar lazy loading en componentes`

#### 🔥 **remove**: Eliminar código o archivos
- `🔥 remove: eliminar componente obsoleto`
- `🗑️ remove: limpiar código comentado`

#### 🚑 **hotfix**: Corrección crítica
- `🚑 hotfix: corregir vulnerabilidad de seguridad`
- `🆘 hotfix: resolver error crítico en producción`

### Reglas Importantes:

1. **Usa minúsculas** para el tipo y descripción
2. **No uses punto final** en la descripción
3. **Máximo 50 caracteres** para la primera línea
4. **Incluye el ámbito** cuando sea relevante (ej: `auth`, `api`, `ui`)
5. **Usa el cuerpo** para explicar el "qué" y "por qué", no el "cómo"

### Ejemplos Completos:

```
✨ feat(auth): implementar autenticación con JWT

- Agregar middleware de verificación de tokens
- Implementar refresh tokens automático
- Configurar cookies seguras para sesiones

Closes #123
```

```
🐛 fix(api): resolver error de conexión a base de datos

El pool de conexiones se agotaba durante picos de tráfico.
Aumentar límite de conexiones y agregar retry logic.

Fixes #456
```

```
📚 docs: actualizar guía de contribución

- Agregar sección de mensajes de commit
- Incluir ejemplos de código
- Actualizar comandos de desarrollo
```

### Emojis Adicionales por Contexto:

- 🔒 **security**: Mejoras de seguridad
- 🌐 **i18n**: Internacionalización
- 📱 **responsive**: Diseño responsivo
- 🎯 **seo**: Optimización SEO
- ♿ **a11y**: Mejoras de accesibilidad
- 🔍 **analytics**: Implementar analytics
- 💾 **db**: Cambios en base de datos
- 🐳 **docker**: Cambios en Docker
- 🔧 **config**: Cambios de configuración

---

**Recuerda**: Un buen mensaje de commit cuenta una historia clara de lo que cambió y por qué.

---
applyTo: "client/**"
---

# Instrucciones para Commits del Cliente

## Conventional Commits para Frontend (Astro + Svelte)

### Tipos específicos para el cliente:

#### 🚀 **feat**: Nuevas funcionalidades del frontend
- `🚀 feat(ui): implementar componente de login`
- `✨ feat(pages): agregar página de empleados`
- `🎨 feat(components): crear componente de tabla`

#### 🐛 **fix**: Correcciones del frontend
- `🐛 fix(ui): corregir responsive en móviles`
- `🔧 fix(forms): resolver validación de formularios`
- `🚑 fix(navigation): corregir rutas rotas`

#### 💄 **style**: Mejoras visuales y UX
- `💄 style(ui): mejorar diseño del header`
- `🎨 style(theme): implementar modo oscuro`
- `✨ style(animations): agregar transiciones suaves`

#### 📱 **responsive**: Diseño responsivo
- `📱 responsive: optimizar diseño para tablets`
- `📲 responsive(mobile): mejorar navegación en móviles`
- `💻 responsive(desktop): ajustar layout para pantallas grandes`

#### ♿ **a11y**: Mejoras de accesibilidad
- `♿ a11y: agregar labels ARIA a formularios`
- `🔍 a11y(navigation): mejorar navegación por teclado`
- `👁️ a11y(contrast): ajustar contraste de colores`

#### 🌐 **i18n**: Internacionalización
- `🌐 i18n: agregar traducciones en inglés`
- `🗣️ i18n(es): actualizar textos en español`
- `🔄 i18n(setup): configurar sistema de traducciones`

#### ⚡ **perf**: Optimizaciones de rendimiento
- `⚡ perf: implementar lazy loading en imágenes`
- `🚀 perf(bundle): optimizar tamaño del bundle`
- `💾 perf(cache): implementar cache de componentes`

#### 🔍 **seo**: Optimización SEO
- `🔍 seo: agregar meta tags dinámicos`
- `📄 seo(sitemap): generar sitemap automático`
- `🏷️ seo(schema): implementar datos estructurados`

#### 🧪 **test**: Tests del frontend
- `🧪 test(components): agregar tests unitarios`
- `🎭 test(e2e): implementar tests end-to-end`
- `✅ test(integration): agregar tests de integración`

### Ámbitos específicos del cliente:
- `ui` - Componentes de interfaz
- `pages` - Páginas de Astro
- `components` - Componentes Svelte/React/Vue
- `layouts` - Layouts y plantillas
- `styles` - CSS y estilos
- `forms` - Formularios y validación
- `navigation` - Navegación y rutas
- `auth` - Autenticación frontend
- `api` - Llamadas al backend
- `utils` - Utilidades del cliente
- `services` - Servicios del frontend
- `stores` - Estado global (Svelte stores)
- `assets` - Recursos estáticos
- `config` - Configuración de Astro

### Frameworks específicos:
- `astro` - Configuración y páginas Astro
- `svelte` - Componentes Svelte
- `react` - Componentes React
- `vue` - Componentes Vue
- `solid` - Componentes SolidJS

### Ejemplos específicos del cliente:

```
🚀 feat(components): implementar tabla de empleados

- Crear componente Svelte reutilizable
- Agregar paginación y filtros
- Implementar ordenamiento por columnas
- Agregar acciones de editar/eliminar

Closes #123
```

```
💄 style(ui): rediseñar interfaz de login

- Modernizar diseño con Tailwind CSS
- Agregar animaciones de entrada
- Mejorar feedback visual de errores
- Implementar tema dark/light

Antes: interfaz básica sin validación visual
Después: experiencia moderna con micro-interacciones
```

```
📱 responsive: optimizar dashboard para móviles

El dashboard no era usable en dispositivos móviles.
- Convertir tabla en cards colapsables
- Ajustar navegación para pantallas pequeñas
- Optimizar tamaño de botones para touch

Performance: mejora del 60% en usabilidad móvil

Fixes #456
```

```
♿ a11y(forms): mejorar accesibilidad de formularios

- Agregar labels explícitos a todos los inputs
- Implementar navegación por teclado
- Mejorar contraste de colores
- Agregar mensajes de error accesibles

Cumple con WCAG 2.1 AA
```

### Casos específicos de Astro:

```
⚙️ config(astro): configurar integración con Svelte

- Habilitar SSR para páginas dinámicas
- Configurar optimización de imágenes
- Agregar soporte para TypeScript estricto
```

```
📦 build(astro): optimizar build de producción

- Implementar code splitting por rutas
- Configurar preload de recursos críticos
- Optimizar imports de componentes
```

### Patrones de UI comunes:

```
🎨 feat(ui): implementar sistema de diseño

- Crear tokens de color y tipografía
- Implementar componentes base (Button, Input, Card)
- Documentar guía de estilo
- Agregar Storybook para componentes
```

```
🔄 feat(stores): implementar gestión de estado global

- Crear stores Svelte para autenticación
- Implementar store de notificaciones
- Agregar persistencia en localStorage
```

### Comandos útiles para commits del cliente:

```bash
# Ver commits de UI
git log --oneline --grep="🎨\|💄\|✨"

# Ver mejoras de rendimiento
git log --oneline --grep="⚡ perf"

# Ver cambios de accesibilidad
git log --oneline --grep="♿ a11y"

# Ver commits por framework
git log --oneline --grep="(svelte)\|(astro)\|(react)"
```

---
applyTo: "server/**"
---

# Instrucciones para Commits del Servidor

## Conventional Commits para Backend

### Tipos específicos para el servidor:

#### 🚀 **feat**: Nuevas funcionalidades del backend
- `🚀 feat(api): implementar endpoint de usuarios`
- `✨ feat(auth): agregar middleware de autenticación`
- `🔌 feat(db): crear modelo de empleados`

#### 🐛 **fix**: Correcciones del servidor
- `🐛 fix(api): corregir validación de datos`
- `🔧 fix(db): resolver error de conexión`
- `🚑 fix(auth): corregir verificación de tokens`

#### 📊 **perf**: Optimizaciones del servidor
- `⚡ perf(db): optimizar consultas SQL`
- `🚀 perf(api): implementar cache de respuestas`
- `💾 perf(memory): reducir uso de memoria en procesos`

#### 🔒 **security**: Mejoras de seguridad
- `🔒 security(auth): implementar rate limiting`
- `🛡️ security(api): validar entrada de datos`
- `🔐 security(cors): configurar políticas CORS`

#### 💾 **database**: Cambios en base de datos
- `💾 db: crear migración de empleados`
- `🗃️ db(schema): actualizar estructura de logs`
- `📈 db(seed): agregar datos de prueba`

#### 🔧 **config**: Configuraciones del servidor
- `🔧 config: actualizar variables de entorno`
- `⚙️ config(docker): optimizar configuración de contenedor`
- `🐳 config(compose): agregar servicio de Redis`

#### 🤖 **bot**: Cambios en los bots
- `🤖 bot(ctaima): implementar scraping de documentos`
- `🔍 bot(docucae): mejorar extracción de datos`
- `📋 bot(coordina): agregar validación de tareas`
- `📊 bot(metacontratas): optimizar procesamiento`

#### 📝 **logs**: Sistema de logging
- `📝 logs: implementar logger estructurado`
- `📊 logs(analytics): agregar métricas de rendimiento`
- `🔍 logs(debug): mejorar trazabilidad de errores`

#### 🔄 **cron**: Tareas programadas
- `🔄 cron: agregar limpieza automática de logs`
- `⏰ cron(backup): implementar respaldo diario`
- `🕐 cron(sync): sincronizar datos cada hora`

### Ámbitos específicos del servidor:
- `api` - Endpoints y rutas
- `auth` - Autenticación y autorización
- `db` - Base de datos y modelos
- `middleware` - Middlewares de Express
- `services` - Servicios de negocio
- `utils` - Utilidades y helpers
- `types` - Tipos TypeScript
- `bot-ctaima` - Bot CTAIMA
- `bot-docucae` - Bot DOCUCAE
- `bot-coordina` - Bot Coordina
- `bot-metacontratas` - Bot Metacontratas
- `cronjobs` - Tareas programadas
- `providers` - Proveedores externos
- `scripts` - Scripts de utilidad

### Ejemplos específicos del servidor:

```
🚀 feat(api): implementar CRUD de empleados

- Crear endpoints GET, POST, PUT, DELETE
- Agregar validación con Joi
- Implementar paginación y filtros
- Agregar tests de integración

Closes #234
```

```
🔒 security(auth): implementar autenticación con JWT

- Generar y verificar tokens JWT
- Configurar refresh tokens
- Agregar middleware de autorización
- Implementar logout seguro

Refs #567
```

```
🤖 bot(ctaima): mejorar extracción de PDFs

El bot fallaba con documentos escaneados.
Implementar OCR con Tesseract para imágenes.

Performance: mejora del 40% en precisión de datos.

Fixes #890
```

```
💾 db: crear migración para tabla de documentos

- Agregar columnas de metadatos
- Crear índices para búsquedas
- Configurar claves foráneas
- Agregar constraints de validación
```

### Comandos útiles para commits del servidor:

```bash
# Ver logs estructurados
git log --oneline --grep="🚀 feat"

# Ver commits por bot específico
git log --oneline --grep="bot(ctaima)"

# Ver cambios de seguridad
git log --oneline --grep="🔒 security"
```
