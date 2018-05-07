# Config Files

## Manjaro i3
I started using Manjaro as a distro at version 17.1.9.
Big thanks to the maintainers of the i3 build.

[Download Manjaro with i3](https://osdn.net/projects/manjaro-community/storage/i3/ "Manjaro i3")


## Vim

```
git clone --depth=1 https://github.com/amix/vimrc.git ~/.vim_runtime
sh ~/.vim_runtime/install_awesome_vimrc.sh
```

### Caps-Lock as ESC

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
add `$ xmodmap ~/.Xmodmap` into `~.xinitrc` to load the map at startup.



## Visual Studio Code
Make sure to use the `visual-studio-code-bin` package from AUR.
Available over `yaourt -S visual-studio-code-bin`.

## i3
```
~/.i3/config
```
The default condig of i3 uses `semicolon` in `resize-mode` to grow window width.
I like to use `h` for that instead.

## Additional Installs
- Chromium + uBlock
- Detex (to prepare Latex for Grammerly)
- 
