# Install JuHex Binary CLI

Download the package for your platform from the latest GitHub Release:

https://github.com/JuHexSecurity/JuHex-Binary-CLI-PUBLISH/releases/latest

## Windows

1. Download `juhex-native-win-x64-<version>.zip`.
2. Extract the archive.
3. Run PowerShell in the extracted directory.
4. Install:

```powershell
powershell -ExecutionPolicy Bypass -File .\install.ps1
```

Restart the terminal after installation if PATH was updated.

## macOS

1. Download the package for your CPU:
   - Apple Silicon: `juhex-native-macos-arm64-<version>.tar.gz`
   - Intel: `juhex-native-macos-x64-<version>.tar.gz`
2. Extract it.
3. Run:

```sh
chmod +x install.sh
./install.sh
```

If Gatekeeper reports that `juhex` is damaged or cannot be opened, follow the commands printed by `install.sh`.

## Linux

1. Download the package for your target:
   - glibc x64: `juhex-native-linux-x64-baseline-glibc-<version>.tar.gz`
   - musl x64: `juhex-native-linux-x64-musl-baseline-<version>.tar.gz`
   - musl arm64: `juhex-native-linux-arm64-musl-<version>.tar.gz`
2. Extract it.
3. Run:

```sh
chmod +x install.sh
./install.sh
```

## Verify

Download `SHA256SUMS.txt` from the same release and compare the package checksum before installing.
