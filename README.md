# Ayün Awesome

Default theme of the Ayün Linux distribution. Based on the theme designed by (elenapan)[https://github.com/elenapan] for ArchLabs.

## Test it

After installing Arch Linux:
```shell
sudo pacman -S awesome inotify-tools git # Install needed software
```
The `pamac` package is required, which is no longer available in the official repositories. This requires some AUR Helper. You can install `yay` as follows, then install the `pamac-aur` package from the AUR:

```shell
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
yay -S pamac-aur
```

```shell
git clone https://github.com/elenapan/archlabs-awesome.git
cp -rT archlabs-awesome ~ # Copy files to home directory. WARNING: THIS WILL OVERWRITE EXISTING FILES!
xrdb ~/.Xresources # Load xrdb settings
fc-cache # Refresh font cache
rm ~/.git ~/screenshots # Delete the repo's non needed folders
```

## Extra packages and why they are needed
1. `pamac`: GUI frontend for pacman

   Launched by clicking the update widget.
2. `inotify-tools`: Monitors file modifications

   Monitors power supply status (plugged/unplugged) in order to update the battery widget icon.

## Screenshot previews

