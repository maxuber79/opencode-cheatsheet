# OpenCode · Cheat-sheet de comandos

Cheat-sheet interactiva con todos los comandos de [OpenCode](https://opencode.ai) (TUI, atajos y CLI), más una guía de **estructura AI-Ready** para proyectos. Buscador en vivo, filtros por categoría, botón de copiar y selector de tema.

🔗 **Demo:** https://maxuber79.github.io/opencode-cheatsheet/

## Características

- 🔍 Buscador en vivo (atajo `/` para enfocarlo)
- 🏷️ Filtros por categoría: atajos, configuración, modelos, contexto, símbolos, personalización, estructura y CLI
- 📋 Copiar al portapapeles en un clic
- 🧱 Estructura AI-Ready — archivos recomendados para que cualquier IA entienda tu proyecto
- 🎨 Selector de tema: Amber Phosphor (terminal) o Monokai
- ⬆️ Botón scroll-to-top al hacer scroll down
- 📱 Responsive y accesible (foco visible, `prefers-reduced-motion`)
- ⚡ 100% estático — sin backend, sin build

## Estructura

```
.
├── index.html      # Todo el sitio (HTML + CSS + JS embebidos)
├── .nojekyll       # Desactiva el procesamiento Jekyll de GitHub Pages
└── README.md
```

## Publicar en GitHub Pages

1. Sube estos archivos a un repo.
2. Ve a **Settings → Pages**.
3. En *Source*, elige **Deploy from a branch** → rama `main` → carpeta `/ (root)`.
4. Guarda. En un par de minutos el sitio queda en `https://TU-USUARIO.github.io/opencode-cheatsheet/`.

## Editar comandos

Los comandos viven en el array `COMMANDS` dentro del `<script>` de `index.html`.
Agregar o modificar uno es una sola línea; no hace falta tocar el HTML.

```js
{ cat:'cli', type:'cli', name:'opencode upgrade', desc:'Actualiza OpenCode a la última versión.' },
```

Los archivos de estructura viven en el array `STRUCTURE`. Se integran automáticamente al filtro y búsqueda.

---

Referencia verificada contra la documentación oficial (OpenCode v1.16.2, jun. 2026).
No reemplaza la [documentación oficial](https://opencode.ai/docs).

## Estructura AI-Ready para cualquier proyecto

Estos archivos ayudan a cualquier IA (Claude Code, OpenCode, Cursor, Copilot, etc.) a entender, navegar y contribuir al proyecto:

```
proyecto/
├── AI.md                 ← Instrucciones y reglas para la IA
├── README.md             ← Propósito, setup, comandos
└── docs/
    ├── ARCHITECTURE.md   ← Stack, estructura, flujo de datos
    ├── STYLEGUIDE.md     ← Convenciones de código
    ├── DECISIONS.md      ← Registro de decisiones técnicas (ADRs)
    ├── TODO.md           ← Tareas pendientes
    ├── CHANGELOG.md      ← Historial de cambios
    ├── CONTRIBUTING.md   ← Workflow de contribución
    ├── SECURITY.md       ← Consideraciones de seguridad
    ├── PROGRESS.md       ← Estado actual del proyecto
    └── PROMPTS.md        ← Prompts útiles para IA
```

> **Nota:** `AI.md` es el nombre recomendado. También funciona como `CLAUDE.md` (Claude Code) o `AGENTS.md` (OpenCode).

---

**Powered by webmain · © 2026 Claudio Muñoz Meza (maxuber)**
