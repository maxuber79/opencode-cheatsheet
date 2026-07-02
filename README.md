# OpenCode · Cheat-sheet de comandos

Cheat-sheet interactiva con todos los comandos de [OpenCode](https://opencode.ai) (TUI, atajos y CLI), con buscador en vivo, filtros por categoría y botón de copiar en cada comando.

🔗 **Demo:** https://maxuber79.github.io/opencode-cheatsheet/

## Características

- 🔍 Buscador en vivo (atajo `/` para enfocarlo)
- 🏷️ Filtros por categoría: atajos, configuración, modelos, contexto, símbolos, personalización y CLI
- 📋 Copiar al portapapeles en un clic
- 🎨 Tema *amber phosphor terminal*
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

---

Referencia verificada contra la documentación oficial (OpenCode v1.16.2, jun. 2026).
No reemplaza la [documentación oficial](https://opencode.ai/docs).
