# Vault Arcade 中文安装手册

[返回首页](../README.md) · [English](INSTALL.en.md) · [Runtime 源码仓库](https://github.com/builtbycodeman/interactive-vault-runtime)

## 运行要求

- 使用推荐的 BRAT 安装方式需要 Obsidian 1.7.2 或更高版本
- BRAT 1.1.0 或更高版本
- Interactive Vault Runtime 0.1.12 或更高版本
- macOS、Windows、Linux、iOS 或 Android 上的 Obsidian

Vault Arcade 安装完成后可以离线运行，不需要注册账号。部分游戏的局域网联机功能需要设备位于同一网络。

## 第一步：安装并启用 BRAT

Vault Arcade 不是独立 Obsidian 插件，必须通过开源插件 Interactive Vault Runtime 安装和运行。

请使用 [BRAT（Beta Reviewers Auto-update Tool）](https://github.com/TfTHacker/obsidian42-brat)安装和持续更新 Runtime：

1. 在 Obsidian 中打开**设置 → 第三方插件**。
2. 点击**浏览**，搜索 **BRAT**，然后安装 **Obsidian42 - BRAT**。
3. 启用 **BRAT**。

## 第二步：使用 BRAT 安装和管理 Interactive Vault Runtime

1. 使用 Windows/Linux 的 `Ctrl+P` 或 macOS 的 `Cmd+P` 打开命令面板。
2. 运行 **BRAT: Plugins: Add a beta plugin for testing**。旧版 BRAT 中的命令名称可能显示为 **BRAT: Add a beta plugin for testing**。
3. 输入 Runtime 源码仓库地址：

   ```text
   https://github.com/builtbycodeman/interactive-vault-runtime
   ```

4. 选择跟踪 **latest** 版本并确认 **Add Plugin**。除非确实希望停留在某个版本，否则不要选择冻结版本。
5. 等待 BRAT 从对应的 GitHub Release 下载 `main.js`、`manifest.json` 和 `styles.css`。
6. 打开**设置 → 第三方插件**；如有需要先刷新插件列表，然后启用 **Interactive Vault Runtime**。

BRAT 对 Runtime 的管理与 Vault Arcade 游戏包相互独立。以后可以打开**设置 → BRAT**，在 Beta 插件列表中管理 Interactive Vault Runtime：

- 保持 **latest**，即可跟踪 Runtime 的新版本。
- 使用 BRAT 设置页中的更新按钮，或在命令面板运行 **BRAT: Plugins: Check for updates to all beta plugins and UPDATE**。
- 使用编辑按钮在最新版本和指定的冻结版本之间切换。
- 从 BRAT 跟踪列表移除 Runtime 只会停止 BRAT 更新，不会卸载插件；如需卸载，请再到**设置 → 第三方插件**中操作。

更多更新选项参见 [BRAT 官方文档](https://tfthacker.com/BRAT)。

## 第三步：从 URL 安装 Vault Arcade

![Runtime 应用包安装页面](../assets/screenshots/runtime-package-install-zh.jpg)

1. 打开**设置 → Interactive Vault Runtime → 互动应用包**。
2. 在“从 URL 安装”区域点击**输入 URL**。
3. 粘贴固定下载地址：

   ```text
   https://github.com/builtbycodeman/vault-arcade-releases/releases/latest/download/vault-arcade.ivpkg
   ```

4. 等待 Runtime 下载并校验安装包。
5. 核对包名、发布者、版本、文件数量和安装目录。
6. 使用建议目录或选择一个专用目录，然后点击**安装**。
7. 安装完成后，从已安装列表打开 Vault Arcade，或打开安装目录中的 `Home` 笔记。

建议始终使用上面的固定 URL。Runtime 会保存安装来源，以后可以通过“检查更新”获取新版。

## Runtime 手动安装备用方案

只有在 BRAT 无法使用时才采用此方式：

1. 打开 [Interactive Vault Runtime 最新 Release](https://github.com/builtbycodeman/interactive-vault-runtime/releases/latest)。
2. 下载 Release 中的以下文件：

   - `main.js`
   - `manifest.json`
   - `styles.css`

3. 在你的 Vault 中创建插件目录：

   ```text
   <你的 Vault>/.obsidian/plugins/interactive-vault-runtime/
   ```

4. 将三个文件放入该目录。
5. 重新启动 Obsidian，或重新加载当前 Vault。
6. 打开 **设置 → 第三方插件**，启用 **Interactive Vault Runtime**。

`.obsidian` 是隐藏目录。如果在文件管理器中看不到它，可以先在 Obsidian 中打开 **设置 → 文件与链接 → 配置文件夹位置**确认目录名称，再让系统显示隐藏文件。

## 使用本地文件安装

如果网络环境无法直接下载：

1. 打开 [Vault Arcade 最新 Release](https://github.com/builtbycodeman/vault-arcade-releases/releases/latest)。
2. 下载版本化 `.ivpkg` 文件或 `vault-arcade.ivpkg`。
3. 可选：使用同一 Release 中的 `.sha256` 文件核对下载内容。
4. 在 Runtime 设置的“安装本地包”区域点击**选择文件**。
5. 选择下载的 `.ivpkg`，核对信息后安装。

通过本地文件安装的版本不能使用 URL 自动检查更新。升级时需要重新下载新版 `.ivpkg` 并再次选择该文件。

## 打开游戏

![Vault Arcade 游戏大厅](../assets/screenshots/vault-arcade-home-zh.jpg)

进入沉浸模式后，游戏会覆盖 Obsidian 的普通工作区并使用完整窗口：

![墨斗：旧城沉浸模式](../assets/screenshots/inkbreak-immersive-zh.jpg)

- 从 Vault Arcade 的 `Home` 页面选择游戏。
- 每款游戏都可以从笔记进入沉浸模式。
- 默认语言跟随 Obsidian，也可以从游戏大厅右上角切换简体中文、English 或日本語。
- 游戏进度会自动保存在当前 Vault 中。

## 更新 Vault Arcade

如果最初通过固定 URL 安装：

1. 打开 **设置 → Interactive Vault Runtime → 互动应用包**。
2. 在 Vault Arcade 条目旁点击**检查更新**。
3. 如果远端版本较新，确认更新。

更新会替换应用文件，但不会删除独立保存的游戏进度。更新前仍建议正常备份或同步 Vault。

## 常见问题

### 设置中没有 Interactive Vault Runtime

打开**设置 → BRAT**，确认 Beta 插件列表中存在 `builtbycodeman/interactive-vault-runtime`。执行 BRAT 的重新安装或更新操作，然后刷新**设置 → 第三方插件**并启用 Runtime。如果采用了手动备用方案，请确认插件目录名称为 `interactive-vault-runtime`，且目录内直接包含 `main.js`、`manifest.json` 和 `styles.css`。

### BRAT 无法安装或更新 Runtime

确认仓库地址完整填写为 `https://github.com/builtbycodeman/interactive-vault-runtime`，并确认 BRAT 正在跟踪最新版本。如果 BRAT 提示 GitHub API 请求频率受限，请稍后再试；安装这个公开仓库通常不需要填写 GitHub Token。必要时可采用 Runtime 手动安装备用方案。

### URL 下载失败

确认地址以 `https://` 开头，并能在浏览器中直接下载 `.ivpkg`。也可以改用本地文件安装。

### 安装后找不到 Home

返回 Runtime 的已安装应用包列表并点击打开；也可以在 Obsidian 快速切换中搜索 `Home`。如果 Vault 中已有同名笔记，请从 Vault Arcade 的安装目录打开。

### 游戏无法启动

确认 Runtime 已启用、应用包没有被移动或手工修改，并重新加载当前 Vault。仍无法运行时，请记录 Obsidian 版本、Runtime 版本、Vault Arcade 版本和错误信息，在本仓库提交 Issue。

## 安全与完整性

`.ivpkg` 包含可执行 JavaScript，并会以 Obsidian 插件权限运行。请只从本仓库的 Releases 下载，并核对 Release 提供的 SHA-256。安装包中的校验清单可以发现文件损坏，但不能代替对下载来源的信任。
