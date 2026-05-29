# JuHex Binary CLI 安装说明

请从最新 GitHub Release 下载对应平台的安装包：

https://github.com/JuHexSecurity/JuHex-Binary-CLI-PUBLISH/releases/latest

## Windows

1. 下载 `juhex-native-win-x64-<version>.zip`。
2. 解压压缩包。
3. 在解压目录打开 PowerShell。
4. 执行：

```powershell
powershell -ExecutionPolicy Bypass -File .\install.ps1
```

如果安装器更新了 PATH，请重启终端后再运行 `juhex`。

## macOS

1. 按 CPU 下载对应安装包：
   - Apple Silicon: `juhex-native-macos-arm64-<version>.tar.gz`
   - Intel: `juhex-native-macos-x64-<version>.tar.gz`
2. 解压。
3. 执行：

```sh
chmod +x install.sh
./install.sh
```

如果 macOS Gatekeeper 提示 `juhex` 已损坏或无法打开，请按 `install.sh` 打印的实际路径命令解除 quarantine。

## Linux

1. 按系统下载对应安装包：
   - glibc x64: `juhex-native-linux-x64-baseline-glibc-<version>.tar.gz`
   - musl x64: `juhex-native-linux-x64-musl-baseline-<version>.tar.gz`
   - musl arm64: `juhex-native-linux-arm64-musl-<version>.tar.gz`
2. 解压。
3. 执行：

```sh
chmod +x install.sh
./install.sh
```

## 校验

请下载同一 release 下的 `SHA256SUMS.txt`，安装前核对安装包 SHA256。
