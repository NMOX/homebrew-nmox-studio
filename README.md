# NMOX Studio — Homebrew Tap

The official Homebrew tap for [NMOX Studio](https://github.com/NMOX/NMOX-Studio),
the web developer's IDE with a hardware-style task rack.

```bash
brew trust --cask nmox/nmox-studio/nmox-studio
brew install nmox/nmox-studio/nmox-studio
```

The `brew trust` step is a one-time acknowledgment Homebrew requires for
any third-party tap; you won't be asked again for updates. The cask
bundles its own Java runtime — nothing else to install. The DMG it
downloads is signed with an Apple Developer ID and notarized by Apple, so
Gatekeeper accepts it as it stands. Updates arrive with
`brew upgrade --cask nmox-studio`, and the app also updates itself in
place via Tools ▸ Plugins. Remove cleanly with
`brew uninstall --cask --zap nmox-studio`.

The cask here is updated automatically by NMOX Studio's release
pipeline on every tagged release.
