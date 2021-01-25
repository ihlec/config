# Config Files

## Vim
Mostly Rob's .vimrc from https://rwx.gg/vi

### Caps-Lock as ESC
Easy config in KDE.

Universal config:
Create the config file for keyboard custom keyboard maps:
```
$ xmodmap -pke > ~/.Xmodmap
```
For my lenovo x230 I needed to put:
```
 clear lock
 keycode  66 = Escape NoSymbol Escape
```

Test out the new mapping:
```
$ xmodmap ~/.Xmodmap
```
Manjaro i3 default config uses already the .Xmodmap file. If you use a diffrent i3 config add `$ xmodmap ~/.Xmodmap` into `~.xinitrc` to load the map at startup.

## Visual Studio Code Settings
{
    "explorer.confirmDelete": false,
    "workbench.editorAssociations": [
        {
            "viewType": "jupyter.notebook.ipynb",
            "filenamePattern": "*.ipynb"
        }
    ],
    "keyboard.dispatch": "keyCode",
    "python.showStartPage": false,
    "window.zoomLevel": 0,
    "nim.buildOnSave": true,
    "git.enableSmartCommit": true,
    "latex-workshop.intellisense.bibtexJSON.replace": {
    
        
    },
    "latex-workshop.view.pdf.viewer": "tab",

    "vim.handleKeys": {
    "<C-c>": false,
    "<C-v>": false,
    "<C-f>": false,
    "<C-y>": false,
    "<C-z>": false,
    "<C-x>": false,
}
}

## i3
```
~/.i3/config
```
The default condig of i3 uses `semicolon` in `resize-mode` to grow window width.
I like to use `h` for that instead.

Also change the hotkey `mod + F2` to `chromium`.

## Additional Installs
- Chromium + uBlock
- Tmux
- CodeStream
- VSCode Grammerly
- git & tig
