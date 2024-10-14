---
title: 設定「Window Decoration」
nav_order: 7023
has_children: false
parent: 如何
---


# 設定「Window Decoration」




## 主題

* [System Settings / Colors & Themes / Window Decorations](#system-settings--colors--themes--window-decorations)
* [Window Decoration / Breeze](#window-decoration--breeze)
* [Window Decoration / Oxygen](#window-decoration--oxygen)
* [Window Decoration / Aurorae](#window-decoration--aurorae)
* [Window Decoration / Aurorae / Plastik](#window-decoration--aurorae--plastik)
* [Window Decoration / Aurorae / Orchis-Dark](#window-decoration--aurorae--orchis-dark)
* [Window Decoration / Aurorae / Vimix-Dark](#window-decoration--aurorae--vimix-dark)
* [Window Decoration / Aurorae / Vimix-Light](#window-decoration--aurorae--vimix-light)
* [探索紀錄](#探索紀錄)




## System Settings / Colors & Themes / Window Decorations


執行

``` sh
grep '^Exec=' /usr/share/applications/kcm_kwindecoration.desktop
```

顯示

```
Exec=systemsettings kcm_kwindecoration
```

> 我們可以透過「`System Settings`」這個圖形界面程式，

> 切換到「`Colors & Themes / Window Decorations`」這個頁面，來設定「Window Decoration」

或是直接執行下面指令，也會開啟「`System Settings`」並且直接切換到「`Colors & Themes / Window Decorations`」這個頁面。

``` sh
systemsettings kcm_kwindecoration
```




## Window Decorations

| Window Decoration |
| ----------------- |
| [Breeze](#window-decoration--breeze) |
| [Oxygen](#window-decoration--oxygen) |
| [Aurorae / Plastik](#window-decoration--aurorae--plastik) |
| [Aurorae / Orchis-Dark](#window-decoration--aurorae--orchis-dark) |
| [Aurorae / Vimix-Dark](#window-decoration--aurorae--vimix-dark) |
| [Aurorae / Vimix-Light](#window-decoration--aurorae--vimix-light) |




## Window Decoration / Breeze

> 設定片段：「~/.config/kwinrc」

``` ini
[org.kde.kdecoration2]
library=org.kde.breeze
theme=Breeze
```

* /usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2/org.kde.breeze.so




## Window Decoration / Oxygen

> 設定片段：「~/.config/kwinrc」

``` ini
[org.kde.kdecoration2]
library=org.kde.oxygen
theme=Oxygen
```

* /usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2/org.kde.oxygen.so




## Window Decoration / Aurorae




## Window Decoration / Aurorae / Plastik

> 設定片段：「~/.config/kwinrc」

``` ini
[org.kde.kdecoration2]
library=org.kde.kwin.aurorae
theme=kwin4_decoration_qml_plastik
```

* /usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2/org.kde.kwin.aurorae.so
* 上面「`theme=kwin4_decoration_qml_plastik`」指的是「/usr/share/kwin/decorations/kwin4_decoration_qml_plastik」




## Window Decoration / Aurorae / Orchis-Dark

> 設定片段：「~/.config/kwinrc」

``` ini
[org.kde.kdecoration2]
library=org.kde.kwin.aurorae
theme=__aurorae__svg__Orchis-dark
```

* /usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2/org.kde.kwin.aurorae.so
* 上面「`theme=__aurorae__svg__Orchis-dark`」指的是「/usr/share/aurorae/themes/Orchis-dark」


執行下面指令，嘗試安裝「orchis-kde」

``` sh
sudo apt-get install orchis-kde
```

顯示

```
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  qt6-style-kvantum qt6-style-kvantum-l10n
Suggested packages:
  orchis-gtk-theme
The following NEW packages will be installed:
  orchis-kde qt6-style-kvantum qt6-style-kvantum-l10n
0 upgraded, 3 newly installed, 0 to remove and 0 not upgraded.
Need to get 2976 kB of archives.
After this operation, 12.2 MB of additional disk space will be used.
Do you want to continue? [Y/n]
```

執行下面指令，嘗試安裝「orchis-gtk-theme」

``` sh
sudo apt-get install orchis-gtk-theme
```

顯示

```
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  gnome-accessibility-themes gnome-themes-extra gnome-themes-extra-data
The following NEW packages will be installed:
  gnome-accessibility-themes gnome-themes-extra gnome-themes-extra-data orchis-gtk-theme
0 upgraded, 4 newly installed, 0 to remove and 0 not upgraded.
Need to get 3014 kB of archives.
After this operation, 92.8 MB of additional disk space will be used.
Do you want to continue? [Y/n]
```

若是安裝了「orchis-kde」，執行下面指令

``` sh
ls -1 /usr/share/aurorae/themes/
```

顯示

```
Orchis
Orchis-dark
Orchis-dark-solid
Orchis-dark_Nvidia
Orchis-dark_x1.25
Orchis-dark_x1.5
Orchis-solid
Orchis_Nvidia
Orchis_x1.25
Orchis_x1.5
```



## Window Decoration / Aurorae / Orchis-dark-solid

> 設定片段：「~/.config/kwinrc」

``` ini
[org.kde.kdecoration2]
library=org.kde.kwin.aurorae
theme=__aurorae__svg__Orchis-dark-solid
```


> 在「GitHub / vinceliuice / [repositories](https://github.com/vinceliuice?tab=repositories)」

> 可以使用「關鍵字：　[kde](https://github.com/vinceliuice?tab=repositories&q=kde&type=&language=&sort=)」查詢


``` sh
mkdir -p ~/.local/share/aurorae/themes
```

* https://github.com/vinceliuice/Vimix-kde/tree/master/aurorae

``` sh
git clone https://github.com/vinceliuice/Vimix-kde.git
```

``` sh
cp Vimix-kde/aurorae/. ~/.local/share/aurorae/themes -rf
```

``` sh
ls -1 ~/.local/share/aurorae/themes/
```

```
Vimix
Vimix-Amethyst
Vimix-Beryl
Vimix-Doder
Vimix-Jade
Vimix-Light
Vimix-Ruby
```




## Window Decoration / Aurorae / Vimix-Dark

> 設定片段：「~/.config/kwinrc」

``` ini
[org.kde.kdecoration2]
library=org.kde.kwin.aurorae
theme=__aurorae__svg__Vimix
```




## Window Decoration / Aurorae / Vimix-Light

> 設定片段：「~/.config/kwinrc」

``` ini
[org.kde.kdecoration2]
library=org.kde.kwin.aurorae
theme=__aurorae__svg__Vimix-Light
```





## 探索紀錄

``` sh
dpkg -L kwin-common | grep plugin
```

```
/usr/lib/x86_64-linux-gnu/qt6/plugins
/usr/lib/x86_64-linux-gnu/qt6/plugins/kf6
/usr/lib/x86_64-linux-gnu/qt6/plugins/kf6/packagestructure
/usr/lib/x86_64-linux-gnu/qt6/plugins/kf6/packagestructure/kwin_aurorae.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kf6/packagestructure/kwin_decoration.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kf6/packagestructure/kwin_effect.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kf6/packagestructure/kwin_scripts.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kf6/packagestructure/kwin_windowswitcher.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kcm_kwin4_genericscripted.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_blur_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_colorblindnesscorrection_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_diminactive_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_glide_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_hidecursor_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_invert_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_magiclamp_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_magnifier_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_mouseclick_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_mousemark_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_overview_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_showpaint_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_slide_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_thumbnailaside_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_tileseditor_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_trackmouse_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_windowview_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_wobblywindows_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/effects/configs/kwin_zoom_config.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/plugins
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/plugins/BounceKeysPlugin.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/plugins/StickyKeysPlugin.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/plugins/buttonsrebind.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/plugins/eis.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/plugins/krunnerintegration.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/plugins/nightlight.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/kwin/plugins/screencast.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2
/usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2/org.kde.kwin.aurorae.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2.kcm
/usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2.kcm/kcm_auroraedecoration.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings/kcm_kwin_effects.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings/kcm_kwin_scripts.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings/kcm_kwin_virtualdesktops.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings/kcm_kwindecoration.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings/kcm_kwinrules.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings/kcm_kwinxwayland.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings/kcm_virtualkeyboard.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings_qwidgets
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings_qwidgets/kcm_kwinoptions.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings_qwidgets/kcm_kwinscreenedges.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings_qwidgets/kcm_kwintabbox.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings_qwidgets/kcm_kwintouchscreen.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/plasma/kcms/systemsettings_qwidgets/kwincompositing.so
/usr/lib/x86_64-linux-gnu/qt6/qml/org/kde/kwin/decoration/libdecorationplugin.so
/usr/lib/x86_64-linux-gnu/qt6/qml/org/kde/kwin/decorations/plastik/libplastikplugin.so
/usr/lib/x86_64-linux-gnu/qt6/qml/org/kde/kwin/private/effects/effectsplugin.qmltypes
/usr/lib/x86_64-linux-gnu/qt6/qml/org/kde/kwin/private/effects/libeffectsplugin.so
```


``` sh
dpkg -L kwin-common | grep org.kde.kdecoration2
```

```
/usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2
/usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2/org.kde.kwin.aurorae.so
/usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2.kcm
/usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2.kcm/kcm_auroraedecoration.so
```

``` sh
ls -1 /usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2/
```

```
org.kde.breeze.so
org.kde.kwin.aurorae.so
org.kde.oxygen.so
```

``` sh
dpkg -S /usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2/
```

```
kwin-decoration-oxygen:amd64, kwin-common, kwin-style-breeze: /usr/lib/x86_64-linux-gnu/qt6/plugins/org.kde.kdecoration2
```


``` sh
dpkg -S /usr/share/kwin
```

```
kwin-addons:amd64, kwin-data: /usr/share/kwin
```

``` sh
ls /usr/share/kwin/decorations/
```

```
kwin4_decoration_qml_plastik
```





