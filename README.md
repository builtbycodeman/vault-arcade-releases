# Vault Arcade Releases

[English installation guide](docs/INSTALL.en.md) · [中文安装手册](docs/INSTALL.zh-CN.md) · [Interactive Vault Runtime](https://github.com/builtbycodeman/interactive-vault-runtime)

Vault Arcade is an offline-first collection of 11 games for Obsidian, built for desktop and mobile with autosave and Simplified Chinese, English, and Japanese interfaces.

> This repository only distributes compiled release packages. It does not contain the game source code.

[Download the latest `vault-arcade.ivpkg`](https://github.com/builtbycodeman/vault-arcade-releases/releases/latest/download/vault-arcade.ivpkg)

## Screenshots

See the [screenshot guide](assets/screenshots/README.md) for filenames, recommended dimensions, and capture instructions.

### Game library

![Vault Arcade game library in English](assets/screenshots/vault-arcade-home-en.jpg)

### Immersive game view

![Inkbreak immersive game view in English](assets/screenshots/inkbreak-immersive-en.jpg)

### Package installer

![Interactive Vault Runtime package installer in English](assets/screenshots/runtime-package-install-en.jpg)

<details>
<summary>简体中文截图</summary>

### 游戏大厅

![Vault Arcade 游戏大厅](assets/screenshots/vault-arcade-home-zh.jpg)

### 游戏沉浸模式

![墨斗：旧城沉浸模式](assets/screenshots/inkbreak-immersive-zh.jpg)

### 应用包安装入口

![Interactive Vault Runtime 应用包安装入口](assets/screenshots/runtime-package-install-zh.jpg)

</details>

## Included games

- Minesweeper / 扫雷
- Sudoku / 数独
- Linked / 联结
- Tidal Islands / 潮汐群岛
- Gravity Twins / 引力双生
- Battle City / 坦克大战
- Tetris: Crystal Fall / 俄罗斯方块：晶落
- Gomoku / 五子棋
- 2048: Flow / 2048：合流
- Tessera / 缀景
- Inkbreak / 墨斗：旧城

## Quick install

1. In Obsidian, open **Settings → Community plugins → Browse**, install **Obsidian42 - BRAT**, and enable it.
2. Open the command palette and run **BRAT: Plugins: Add a beta plugin for testing**.
3. Enter `https://github.com/builtbycodeman/interactive-vault-runtime`, track the **latest** version, and add the plugin.
4. Open **Settings → Community plugins** and enable **Interactive Vault Runtime**.
5. Open **Settings → Interactive Vault Runtime → Interactive packages**.
6. Select **Enter URL** and paste the stable download URL below:

   ```text
   https://github.com/builtbycodeman/vault-arcade-releases/releases/latest/download/vault-arcade.ivpkg
   ```

7. Review the package and destination folder, then select **Install**.
8. Open Vault Arcade from the installed package list, or open the `Home` note in its installation folder.

BRAT keeps Runtime updated from its GitHub Releases. For Runtime management, manual fallback installation, local `.ivpkg` installation, and troubleshooting, see the [English installation guide](docs/INSTALL.en.md).

## Requirements

- Obsidian 1.7.2 or later for the recommended BRAT installation
- BRAT 1.1.0 or later
- Interactive Vault Runtime 0.1.12 or later
- Desktop or mobile

## Security

An `.ivpkg` contains executable JavaScript that runs with Obsidian plugin permissions. Download Vault Arcade only from this repository and verify the SHA-256 checksum published with each release.

## 中文说明

Vault Arcade 是一套运行在 Obsidian 中的离线优先游戏合集，包含 11 款适配桌面端和移动端的游戏，支持自动存档、简体中文、English 和日本語。

本仓库只用于发布已构建的下载包，不包含游戏源码。完整安装、更新和故障排查说明请参阅[中文安装手册](docs/INSTALL.zh-CN.md)。

[下载最新版 `vault-arcade.ivpkg`](https://github.com/builtbycodeman/vault-arcade-releases/releases/latest/download/vault-arcade.ivpkg)
