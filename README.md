# helix-config

- [keymap](https://docs.helix-editor.com/keymap.html)

- clone this repo directly in the configuration directory for helix
  - on Windows, the configuration directory is `%APPDATA%\helix`

## compile and run helix from sources

```bat
cd "%USERPROFILE%\Desktop"
if not exist helix git clone git@github.com:helix-editor/helix.git

:: make a small change to the helix-term\src\main.rs (function main_impl) just to be sure things works as expected!
cd "%USERPROFILE%\Desktop\helix" && cargo install --path helix-term --locked
cd "%USERPROFILE%\Desktop" && hx --help && cd "%USERPROFILE%\Desktop\helix"
```

## restore syntax highlight

```bat
del %USERPROFILE%\.cargo\bin\hx.exe
```

## add python support

- requires `nodejs` (via `npm`) and `python`!!

```bat
npm install --location=global pyright
py -m pip install -U ruff-lsp
```
