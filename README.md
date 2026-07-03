# OpenCode · Cheat-sheet de comandos

Cheat-sheet interactiva con todos los comandos de [OpenCode](https://opencode.ai) (TUI, atajos y CLI), más una guía de **estructura AI-Ready** para proyectos. Buscador en vivo, filtros por categoría, botón de copiar, selector de tema y más.

🔗 **Demo:** https://maxuber79.github.io/opencode-cheatsheet/

## Características

- 🔍 Buscador en vivo (atajo `/` para enfocarlo)
- 🏷️ Filtros por categoría: atajos, configuración, modelos, contexto, símbolos, personalización, estructura y CLI
- 📋 Copiar al portapapeles en un clic
- 🧱 Estructura AI-Ready — archivos recomendados para que cualquier IA entienda tu proyecto, con árbol visual y comandos para crear la estructura
- 🎨 Selector de tema: Amber Phosphor (terminal) o Monokai, con persistencia en localStorage
- ⬆️ Botón scroll-to-top que aparece al hacer scroll
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

---

**Powered by webmain · © 2026 Claudio Muñoz Meza (maxuber)**
