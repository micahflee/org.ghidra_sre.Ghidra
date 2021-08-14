# Ghidra networkless Flatpak

This fork of the Ghidra [Flathub package](https://flathub.org/apps/details/org.ghidra_sre.Ghidra) removes network access from the Flatpak sandbox.

To install locally, you need `flatpak` and `flatpak-builder`:

```sh
# Add flathub repo, if you don't already have it
flatpak remote-add --if-not-exists --user flathub https://flathub.org/repo/flathub.flatpakrepo

# Build and install
flatpak-builder build --force-clean --install-deps-from=flathub --install --user org.ghidra_sre.Ghidra.json
```
