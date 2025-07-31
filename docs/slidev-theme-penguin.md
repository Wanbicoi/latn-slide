**Install**:
Add to `slides.md` frontmatter:

```yaml
---
theme: penguin
---
```

Also install `vite-svg-loader` and update `vite.config.js`.

**Layouts included**:

* `intro`
* `presenter` (with `presenterImage`)
* `new-section`
* `text-image` (with `media`, optional `reverse`)
* `text-window` (with optional `reverse`, slot `::window::` for window content)

**Components**:

* `<fancy-link>`: auto-favicon links
* `<TheConsole>`: styled iframe embed
