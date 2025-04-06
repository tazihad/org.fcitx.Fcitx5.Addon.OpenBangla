# org.fcitx.Fcitx5.Addon.OpenBangla


build

```
flatpak run org.flatpak.Builder --user --force-clean --install-deps-from=flathub --repo=repo --install build-dir 'org.fcitx.Fcitx5.Addon.OpenBangla.yml'
```

Build works.
But addon doesn't show up on Fcitx5. My best guess is because [fcitx5 flatpak](https://github.com/fcitx/flatpak-fcitx5/blob/master/org.fcitx.Fcitx5.yaml) built using kde 6.*. But Since OpenBangladesh is still on qt5 it won't build on KDE6. 

Original issue https://github.com/OpenBangla/OpenBangla-Keyboard/issues/390
