# Noctalia plugin source: Niri Workspaces

A source repo for [Noctalia](https://github.com/noctalia-dev/noctalia), holding
one plugin: **Niri Workspaces**, a workspace switcher for niri that draws dots
for the workspaces you are not on and leaves named workspaces — a scratchpad's
shelf, for instance — out of the bar.

## Install

```sh
noctalia msg plugins source add madmedicnl git https://github.com/madmedicnl/noctalia-niri-workspaces
noctalia msg plugins enable madmedicnl/niri-workspaces
```

Then add **Niri Workspaces** to a bar from **Settings → Bar → Add widget**. The
widget type, if you edit the config by hand, is
`madmedicnl/niri-workspaces:niri-workspaces`.

Once it is in the plugin store, installing from there is enough — the source is
for anyone who would rather pin to this repository.

## Layout

```
catalog.toml                     index of what this source ships
niri-workspaces/                 the plugin, named after the id after the "/"
  plugin.toml                    manifest: id, metadata, entries, settings
  widget.luau                    the entry script (one bar widget)
  README.md                      the plugin's page in the store
  thumbnail.webp                 the store card image, 960×540
  screenshots/bar.webp           the picture in the README
  translations/en.json           every label and description the manifest names
```

## Requirements

`niri` on `PATH`, and Noctalia 5.2 or newer (plugin API 32).

## License

MIT. The plugin keeps my copyright; see [`LICENSE`](LICENSE).
