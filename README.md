# Argentina Light — Omarchy theme

A light Omarchy theme inspired by Argentina — the white-and-celeste of its flag and the bright southern light: white surfaces with a celeste tint, celeste accents, and gold of the Sol de Mayo.

![preview](preview.png)

## Install

```bash
omarchy theme install https://github.com/santiagoei/omarchy-argentina-light.git
omarchy theme set argentina-light
```

## Palette

| Token | Color | Inspiration |
|---|---|---|
| accent | `#3f7fb5` | Celeste (legible on white) |
| background | `#f4f9fd` | Blanco celeste |
| foreground | `#16324a` | Azul bandera |
| yellow | `#e0a800` | Sol de Mayo |
| green | `#3f9d6e` | Pampa verde |
| red | `#c9425a` | Papel picado |
| brown | `#8f6a3f` | Yerba mate |

Window borders use a celeste→gold gradient.

## Backgrounds

20 photos of Argentina — Buenos Aires (the Obeliscos, Congreso, Caminito,
the neighborhoods, Mar del Plata), Iguazú, El Calafate, Aconcagua, Los
Alerces, Jujuy's Siete Colores and estadio, the seven lakes of Neuquén,
Córdoba, a map, and one for Diego. Filenames carry their priority tier,
so the alphabetical cycle runs first-pick first:
`01_arg_tierradelfuego_glaciar.jpg` opens the theme. The dark sister
shares this exact pool, renumbered around its own opener.

## Sister theme

[omarchy-argentina](https://github.com/santiagoei/omarchy-argentina.git) — the dark variant: deep navy.

## Development

This repo root is the theme directory itself; `omarchy theme install` clones it to `~/.config/omarchy/themes/<name>`. Everything here is color data: no `*.lua`, terminal configs, or `vscode.json` are shipped (those are dropped by the installer and regenerated from `colors.toml`).

To hack on it locally:

```bash
git clone <this-repo> ~/code/omarchy-argentina-light
ln -s ~/code/omarchy-argentina-light ~/.config/omarchy/themes/argentina-light
omarchy theme set argentina-light
```

Remove the symlink before testing `omarchy theme install` — the installer deletes the destination directory.

## License

MIT
