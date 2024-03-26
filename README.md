# helix-config

- [keymap](https://docs.helix-editor.com/keymap.html)

- clone this repo directly in the configuration directory for helix
  - on Windows, the configuration directory is `%APPDATA%\helix`

## add python support

- requires `nodejs` (via `npm`) and `python`!!

```bat
npm install --location=global pyright
py -m pip install -U ruff-lsp
```
