# macOS Gatekeeper Troubleshooting

The macOS native packages are not currently Developer ID signed or Apple notarized.

If macOS says `juhex` is damaged or cannot be opened, remove the quarantine attribute from the extracted release directory and the installed JuHex directory.

The installer prints commands with the actual paths used during that install. They look like this:

```sh
xattr -dr com.apple.quarantine "<extracted-release-directory>"
xattr -dr com.apple.quarantine "$HOME/.local/share/juhex/versions/<version>"
chmod +x "$HOME/.local/share/juhex/versions/<version>/juhex" "$HOME/.local/share/juhex/uninstall.sh"
"$HOME/.local/share/juhex/versions/<version>/juhex" --version
```

After quarantine is removed, run `juhex --version` again.
