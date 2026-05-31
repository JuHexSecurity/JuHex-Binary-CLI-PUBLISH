# JuHex Binary CLI Publish

This repository hosts public release metadata and installation documents for JuHex Binary CLI.

Native binary packages are distributed through GitHub Releases. The git tree intentionally keeps large binary archives out of history.

## Latest Release

Latest release page:

https://github.com/JuHexSecurity/JuHex-Binary-CLI-PUBLISH/releases/latest

Current prepared version: `v1.0.21`.

## Downloads

Download native packages from the matching GitHub Release assets:

- `juhex-native-win-x64-1.0.21.zip`
- `juhex-native-macos-arm64-1.0.21.tar.gz`
- `juhex-native-macos-x64-1.0.21.tar.gz`
- `juhex-native-linux-x64-baseline-glibc-1.0.21.tar.gz`
- `juhex-native-linux-x64-musl-baseline-1.0.21.tar.gz`
- `juhex-native-linux-arm64-musl-1.0.21.tar.gz`

## Articles

Public articles and product notes are available under:

https://github.com/JuHexSecurity/JuHex-Binary-CLI-PUBLISH/tree/main/docs/articles

## Verify Downloads

Use the checksum file for the same release:

```sh
sha256sum -c SHA256SUMS.txt
```

On Windows PowerShell:

```powershell
Get-FileHash .\juhex-native-win-x64-1.0.21.zip -Algorithm SHA256
```

Compare the output with `checksums/v1.0.21/SHA256SUMS.txt` or the `SHA256SUMS.txt` release asset.

## Source Repository

Source repository:

https://github.com/JuHexSecurity/JuHex-Binary-CLI

## Repository Policy

- Public docs and release metadata may be committed here.
- Large binary packages should be uploaded as GitHub Release assets, not committed to git.
- Internal notes, private configs, secrets, databases, logs, and unpublished build work should not be committed here.
