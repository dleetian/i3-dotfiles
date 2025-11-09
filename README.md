# My applications
## i3 environment
i3 
alacritty
fastfetch instead of neofetch
polybar
rofi
feh
copyq - clipboard manager (text + images)
maim - screenshot tool
xclip - copies image to clipboard
stow
picom
nerd-fonts - 67

## browser, development, and files
dolphin instead of nautilus
nvim
node
tmux
obsidian
brave-bin

## reading (books)
Foliate for epub files
Okular for everything else

# Setup 
Setting up the environment is simple. 
First, modify the system files to allow i3 to run. Just put `exec i3` in the `~/.xinitrc` file. 
What this does is that it runs i3 when we type the command `startx`.
`~/.xinitrc`
```bash
exec i3
```
****
Second, install the applications defined above using yay or pacman.
****
Third, clone my GitHub dotfiles and move it to `.config` using `stow .`.
Clone my repository
```bash
git clone https://github.com/dleetian/i3-dotfiles.git ~/dotfiles
cd dotfiles
stow .
```
****
The setup is complete at this point. Go run `startx` in the terminal to run the environment.
```bash
startx
```

# Controls
My controls are simple. `Super` key stands is the `Windows` key. 

## Opening Applications
`Super + D` opens the application launcher (`rofi`).

## Navigation Controls
`Super + H` focus on the left panel.
`Super + L` focus on the right panel.
`Super + J` focus on the bottom panel.
`Super + K` focus on the top panel.
`Super + [0-9]` go to workspace #.

## Moving the Panels
`Super + Shift + H` move the current panel to the left.
`Super + Shift + L` move the current panel to the right.
`Super + Shift + J` move the current panel to the bottom.
`Super + Shift + K` move the current panel to the top.
`Super + Shift + [0-9]` move the current panel to workspace #.

## Other modes
`Super + S` to allow layout stacking. To exit the layout stacking, move your panel to left/right/bottom/top.
`Super + T` to toggle floating/tiling on the current panel.
`Super + F` to toggle fullscreen on the current panel.
`Super + Shift + R` to restart the current X session.
`Super + Shift + E` to exit of the current X session.

# Resizing the Panels
First, press `Super + R` to allow resizing. Then do the following.
For the following keybinds, you can use arrow keys instead of `H/L/J/K`.
- `H/arrow left` shrink the width of the panel. 
- `L/arrow right` increase the width of the panel.
- `J/arrow down` shrink the height of the panel.
- `K/arrow up` increase the height of the panel.
After resizing, press `Super + R` again.
