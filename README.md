# org.fcitx.Fcitx5.Addon.OpenBangla

### Install
- Download [fcitx-openbangla.flatpak](https://github.com/tazihad/org.fcitx.Fcitx5.Addon.OpenBangla/releases)
- Install `flatpak install --user fcitx5-openbangla.flatpak`

### Build

```
flatpak remote-add --user --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
flatpak install flathub org.flatpak.Builder
flatpak run org.flatpak.Builder --user --force-clean \
  --install-deps-from=flathub \
  --repo=repo \
  --install build-dir \
  org.fcitx.Fcitx5.Addon.OpenBangla.yml
```
Export single package for installation on other machine
```sh
flatpak build-bundle --runtime repo fcitx5-openbangla.flatpak org.fcitx.Fcitx5.Addon.OpenBangla stable
```

Original issue https://github.com/OpenBangla/OpenBangla-Keyboard/issues/390

run settings:
```sh
flatpak run --command="/app/addons/OpenBangla/bin/openbangla-gui" org.fcitx.Fcitx5
```

### What's not working:
- settings is black

