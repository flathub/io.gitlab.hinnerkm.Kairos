### Build
```bash
flatpak-builder --repo=./repo --ccache --force-clean --compose-url-policy=full --mirror-screenshots-url=https://dl.flathub.org/media --user build_dir io.gitlab.hinnerkm.Kairos.json
```

### Lint
```
flatpak run --command=flatpak-builder-lint org.flatpak.Builder manifest io.gitlab.hinnerkm.Kairos.json
flatpak run --command=flatpak-builder-lint org.flatpak.Builder repo repo
```