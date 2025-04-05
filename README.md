# .Archdots install

```
cd ~
git clone https://github.com/Paulobox/.Archdots
```

```
cd ~/.Archdots
stow zsh shell x11 alacritty kitty nsxiv tmux myscripts rofi vscode fish lf picom dunst zathura
sudo ln -s ~/.config/shell/profile ~/.zprofile
sudo ln -s ~/.config/x11/xprofile ~/.xprofile
chmod +x ~/.config/shell/zprofile
chmod +x ~/.config/x11/xprofile
```

##### for scripts make [symbolic links](https://github.com/Paulobox/.dotfiles/blob/main/myscripts/.myscripts/README.md)


## remove symbolic links:

`
find ~/.config -xtype l -delete
`

```
setopt dotglob
mv -f *(D) ../ 2>/dev/null
```

```
mv -f * ~/.config/ 2>/dev/null
```
