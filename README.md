# org.fcitx.Fcitx5.Addon.OpenBangla


build

```
flatpak remote-add --user --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
flatpak install flathub org.flatpak.Builder
flatpak run org.flatpak.Builder --user --force-clean \
  --install-deps-from=flathub \
  --repo=repo \
  --install build-dir \
  org.fcitx.Fcitx5.Addon.OpenBangla.yml
```
Build works.

Original issue https://github.com/OpenBangla/OpenBangla-Keyboard/issues/390

settings:
```sh
flatpak run --command="/app/addons/OpenBangla/bin/openbangla-gui" org.fcitx.Fcitx5
```

What's not working:
- icons not showing up.

