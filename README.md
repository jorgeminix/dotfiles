# My Arch Linux dotfiles

These dotfiles are designed around my most common workflow: using a web browser, the terminal, a code editor, and a terminal-based file manager. As a result, they currently do not include themes or configuration for graphical file managers or other desktop applications.

## Installation

Installation is currently manual:
1. Clone or download this repository.
2. Move the configuration directories to your home directory.
3. Install the required packages listed below.
4. Start or restart the relevant applications.

For example:

```bash
git clone <repository-url>
cd <repository-directory>

mv .config ~/
mv .local ~/
```

## Required Packages

### Audio

```bash
sudo pacman -S pipewire pipewire-pulse wireplumber
```

### Apps

```bash
sudo pacman -S feh kitty neovim rofi scrot
```

### Font

```bash
sudo pacman -S ttf-jetbrains-mono-nerd
```

### X server

```bash
sudo pacman -S xorg-server xorg-xinit xorg-xrandr
```

### Window manager

```bash
sudo pacman -S i3-wm i3lock i3status
```

### Optional applications

These aplications are not required for the configuration to work, but they are useful for my daily workflow.

```bash
sudo pacman -S firefox yazi
```

## Keymaps

### Open and close apps

- `Super + Enter` — Open Terminal
- `Super + d` — Open Rofi
- `Super + Shift + q` — Kill focused window

### Volume

- `Super + bracketright` — Increase volume
- `Super + bracketleft` — Decrease volume
- `Super + semicolon` — Mute and unmute volume
- `Super + apostrophe` — Mute and unmute microphone

### Navigation

- `Super + h/j/k/l` — Change focus
- `Super + Shift + h/j/k/l` — Move the focused window
- `Super + u/i/o/p/7/8/9/0` — Change focus to another group
- `Super + Shift + u/i/o/p/7/8/9/0` — Move the focused window to another group

### Window managing

- `Super + f` — Full screen toggle
- `Super + s` — Stacking layout
- `Super + w` — Switch to tabbed layout
- `Super + e` — Layout toggle split
- `Super + r` — Resize
- `Super + m` — Split horizontally
- `Super + Shift + m` — Split vertically

### Useful shortcuts

- `Super + n` — Take screenshot
- `Super + Shift + n` — Take selected screenshot
- `Alt + Shift` — Change layout between us/latam

### i3

- `Super + Shift + c` — Reload
- `Super + Shift + r` — Restart
- `Super + Shift + e` — Exit the X session

## Neovim keymaps

- `jk` — Exit from insert mode
- `Esc` — Remove highlight in search mode
- `<leader>e` — Open neotree
- `<leader>o` — Switch between neotree and buffer

## Command to change colorscheme

The `theme` command changes the colorscheme for Kitty, Rofi and Neovim.

- `theme rose-pine-main` or `theme main`
- `theme rose-pine-dawn` or `theme dawn`
- `theme rose-pine-moon` or `theme moon`
