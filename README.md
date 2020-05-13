https://github.com/bitwarden/desktop/releases/download/v1.17.2/Bitwarden-1.17.2-x86_64.AppImage

# build deps:

`flatpak install -y flathub org.gnome.Sdk/x86_64/3.36`

# build and install

```
flatpak-builder --force-clean build-dir org.flatpak.Bitwarden.yaml --install --user
```

# launch

```
flatpak run org.flatpak.Bitwarden
```

# cleanup-uninstall

```
flatpak --user uninstall -y org.flatpak.Bitwarden
```
