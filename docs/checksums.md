# Checksum Verification

Always verify downloaded native packages against the checksum file from the same release.

## Linux or macOS

```sh
sha256sum -c SHA256SUMS.txt
```

If your macOS environment does not provide `sha256sum`, use:

```sh
shasum -a 256 <downloaded-file>
```

## Windows PowerShell

```powershell
Get-FileHash .\juhex-native-win-x64-1.0.18.zip -Algorithm SHA256
```

Compare the hash with `SHA256SUMS.txt`.
