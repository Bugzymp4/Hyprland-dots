Bugzy’s Hyprland Dots

These are my personal Hyprland dotfiles. Follow the steps below to set everything up.

Installation

Clone the repo
Clone this repository and enter it:
git clone https://github.com/yourusername/bugzy-dots.git
cd bugzy-dots

Replace your hyprland.conf
Backup your current config first (usually at ~/.config/hypr/hyprland.conf) and then copy mine:
mv ~/.config/hypr/hyprland.conf ~/.config/hypr/hyprland.conf.bak
cp hypr/hyprland.conf ~/.config/hypr/hyprland.conf

Install Hyprpaper and set wallpaper
Install Hyprpaper with your package manager (pacman -S hyprpaper or yay -S hyprpaper).
Make sure the config folder exists: mkdir -p ~/.config/hypr
Copy my Hyprpaper config: cp hypr/hyprpaper.conf ~/.config/hypr/hyprpaper.conf
Copy the Zelda wallpaper into your Pictures folder: mkdir -p ~/Pictures and cp wallpapers/Zelda1.png ~/Pictures/Zelda1.png

Install Waybar and apply config
Install Waybar (sudo pacman -S waybar).
Backup your old config: mv ~/.config/waybar ~/.config/waybar.bak
Copy my config: cp -r waybar ~/.config/
Check ~/.config/waybar/config for required fonts and install them.

Set up Kitty terminal
Install Kitty (sudo pacman -S kitty).
Make sure the config folder exists: mkdir -p ~/.config/kitty
Copy my Kitty config: cp kitty/kitty.conf ~/.config/kitty/kitty.conf
Make sure transparency is set to 0.5 inside the config: background_opacity 0.5
