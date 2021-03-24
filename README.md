<p align="center">
<img src="https://github.com/pufferbian/gtk-theme/raw/repo-assets/pufferbian%20gtk%20banner.png"/>
</p>

-------------------

A GTK+ theme for Pufferbian


### Required Components
-------------------
Puffershell supports Gtk+ 3.22.x

 ```
 * Gtk+-3.0             >= 3.22
 * Gtk+-2.0             >= 2.24.30
 * gtk2-engines-pixbuf  >= 2.24.30
 * gtk2-engines-murrine >= 0.98.1
 ```

### Installation
----------------------------

###### Note: You must have sassc installed in order to build Puffershell. Users of Ububtu/Pop_OS! 17.04 or later can all build-dependencies using:

```
sudo apt install sassc meson libglib2.0-dev 
```

For making modifications to assets, you will additionally need these two:

```
sudo apt install inkscape optipng
```


1. If previous versions were installed/existed, remove them first.

 ```
 sudo rm -rf /usr/share/themes/Puffershell*
 rm -rf ~/.local/share/themes/Puffershell*
 rm -rf ~/.themes/Puffershell*
 ```

2. Generate the theme files.

```
meson build && cd build
ninja
```

3. Install the theme.

```
ninja install
```

#### Rebuilding after modifications:

You shouldn't need to rebuild the entire theme after modifications. If you make
changes to any GTK3 or GTK2 assets, delete the old rendered copies and use the
`render-assets.sh` script to regenerate those with new ones with your 
modifications. 

Public License
--------------
 Most files: GPL-3.0+
 Upstream Adwaita: LGPLv2.1
 Sound theme: CC-BY-SA-4.0


 > **Note:**
 >
 > SVG files are licensed under CC BY-SA 4.0

Special Thanks to
--------------
 System76, developers of the Pop!_OS GTK+ Theme: https://github.com/pop-os/gtk-theme<br>
 Nana-4, the developer of Materia.<br>
 tista500 and the Adapta Theme Project: https://github.com/adapta-project/<br>
