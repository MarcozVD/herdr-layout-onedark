# One Dark

Herdr's own window (spaces and agents on the left, tabs as pills, panes as cards, a status bar) in the One Dark palette as **herdr-desk** paints it, with a sky-blue `#60b9fc` accent. Flat, solid panels. One Dark in dark mode, One Light in light mode; it follows the system appearance by itself.

![One Dark](preview.png)

## What's inside

| File | What it is |
|---|---|
| `layouts/onedark.json` | the layout (Herdr's main window structure) |
| `layouts/onedark.png` | the picture Settings shows for it |
| `themes/herdr-onedark.json` | One Dark |
| `themes/herdr-onelight.json` | One Light |

Only Herdr's shipped mods are used: no custom code, no programs run, no network access.

## Install

Copy the folders into your Herdr home (`~/.config/herdr-app`, or `HERDR_APP_HOME`), then switch to the layout:

```sh
git clone https://github.com/MarcozVD/herdr-layout-onedark
cp -r herdr-layout-onedark/{layouts,themes} ~/.config/herdr-app/
herdr-app do layout.switch '{"name":"onedark"}'
```

On Windows PowerShell:

```powershell
git clone https://github.com/MarcozVD/herdr-layout-onedark
Copy-Item -Recurse -Force herdr-layout-onedark/layouts,herdr-layout-onedark/themes "$HOME/.config/herdr-app/"
herdr-app do layout.switch '{"name":"onedark"}'
```

`ctrl-shift-l` cycles back to your other layouts. To remove it, delete the files listed above from `~/.config/herdr-app`.

Or ask your agent to add it: *"add the Herdr layout at github.com/MarcozVD/herdr-layout-onedark"*.

## Build it yourself

[`RECIPE.md`](RECIPE.md) is the full brief (regions, sizes, exact colors, node tree, gotchas, checks): an agent with an empty folder can rebuild the layout from it.

The themes also work on their own: set `"theme": { "light": "herdr-onelight", "dark": "herdr-onedark" }` in `settings.json` to use them with any layout.

Palette: Atom's One Dark / One Light (MIT).

## Related

- [herdr-layout-catppuccin](https://github.com/MarcozVD/herdr-layout-catppuccin): Catppuccin Mocha / Latte, solid panels.
- [herdr-layout-onedark](https://github.com/MarcozVD/herdr-layout-onedark): One Dark / One Light, solid panels.
- [herdr-layout-glass](https://github.com/MarcozVD/herdr-layout-glass): glassmorphism in neutral graphite.
