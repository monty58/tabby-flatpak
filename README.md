# Tabby Flatpak

This is a [Tabby](https://eugeny.github.io/tabby/) build configuration for [Flatpak](https://flatpak.org/) based on several electron flatpak apps.

## Build instructions

```
flatpak install io.atom.electron.BaseApp org.freedesktop.Platform//23.08 org.freedesktop.Sdk//23.08
flatpak-builder build-dir com.eugeny.tabby.yml
flatpak-builder --user --install --force-clean build-dir com.eugeny.tabby.yml
flatpak run com.eugeny.tabby
```