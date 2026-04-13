## For transparency

The `.git` directories were removed from all included wallpaper sources because these folders were originally tracked as separate repositories. Using Git submodules would have created external links to the original upstream repositories, which would require recursive cloning to fully retrieve all content.

To avoid depending on external repository availability at clone time (for example, if any upstream repository changes access settings or becomes unavailable in the future), the content has been included directly instead of being managed as submodules.

This repository does not claim ownership of the wallpaper assets; they are collected from their respective original sources and remain subject to their original licenses and ownership.


```console
❯ cd ~/Pictures/Wallpapers
❯ l
drwxr-xr-x jelius staff  14 KB Thu Mar 26 10:25:23 2026  hyprland_wallpapers
drwxr-xr-x jelius staff 5.3 KB Thu Mar 26 10:17:12 2026  wallpaper
drwxr-xr-x jelius staff 224 B  Thu Mar 26 10:53:37 2026  Wallpaper-Bank
drwxr-xr-x jelius staff 256 B  Thu Mar 26 10:53:19 2026  Wallpaper-Collection
❯ rm -rf ./hyprland_wallpapers/.git
❯ rm -rf ./wallpaper/.git
❯ rm -rf ./wallpaper-bank/.git
❯ rm -rf ./wallpaper-collection/.git
❯ git init
Initialized empty Git repository in /Users/jelius/Pictures/Wallpapers/.git/
❯ git add --all
```
