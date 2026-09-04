# Homebrew tap for Tessera

[Tessera](https://github.com/OrionApplePie/Tessera) is a native macOS window
switcher that draws every window on a map of your Spaces.

```sh
brew tap OrionApplePie/tessera
brew install tessera
brew services start tessera
```

`brew install --HEAD tessera` builds `main` instead of the latest release.

Tessera needs Screen Recording to list windows and capture their previews, and
Accessibility to raise a particular one; `tessera permissions` says which of them
is still missing.

The formula is kept in the main repository at `Formula/tessera.rb` and copied
here. `docs/packaging.md` there explains why a tap is a repository of its own —
`brew tap` finds taps by name — and what a release needs.
