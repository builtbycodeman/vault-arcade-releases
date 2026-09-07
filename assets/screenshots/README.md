# Screenshot guide / 截图维护说明

本目录保存 README 和安装手册使用的产品截图。中文与英文截图采用相同构图和一一对应的文件名。

This directory contains the product screenshots used by the README and installation guides. Chinese and English screenshots should use matching compositions and paired filenames.

## 文件清单 / File list

| 内容 | 中文文件 | English file |
| --- | --- | --- |
| 游戏大厅 / Game library | `vault-arcade-home-zh.jpg` | `vault-arcade-home-en.jpg` |
| 墨斗沉浸页 / Inkbreak immersive view | `inkbreak-immersive-zh.jpg` | `inkbreak-immersive-en.jpg` |
| Runtime 安装页 / Runtime installer | `runtime-package-install-zh.jpg` | `runtime-package-install-en.jpg` |

英文版三个文件尚未加入仓库。按上表使用完全一致的文件名放入当前目录后，README 和英文安装手册会自动显示它们，不需要再修改 Markdown。

The three English files have not been added yet. Place them in this directory using the exact filenames above. The README and English guide will then display them without further Markdown changes.

## 推荐规格 / Recommended format

- 使用 JPEG，扩展名为 `.jpg`。
- 推荐 16:10 或 16:9，宽度至少 1600 px。
- 同一组中英文截图尽量保持相同窗口尺寸、缩放比例和界面位置。
- 截图前隐藏无关侧栏、开发目录、通知和个人 Vault 内容。
- 不要包含用户名、本地文件路径、设备名、私人笔记或同步服务信息。
- 保留应用主体周围少量空间，不要裁掉 Runtime 的退出沉浸按钮或重要操作入口。

- Use JPEG with the `.jpg` extension.
- Prefer a 16:10 or 16:9 frame at least 1600 px wide.
- Keep matching Chinese and English shots at the same window size, zoom level, and UI position.
- Hide unrelated sidebars, development folders, notifications, and personal Vault content.
- Do not include usernames, local paths, device names, private notes, or sync-service details.
- Leave a little space around the product UI. Do not crop out Runtime's immersive-exit control or important actions.

## 如何拍英文截图 / How to capture the English screenshots

### 1. 游戏大厅

1. 打开 Vault Arcade 的 `Home`。
2. 使用右上角语言菜单选择 **English**。
3. 隐藏无关侧栏并滚动到页面顶部。
4. 截图并导出为 `vault-arcade-home-en.jpg`。

### 2. 墨斗沉浸页

1. 保持 Vault Arcade 语言为 **English**。
2. 打开 Inkbreak / 墨斗：旧城并进入沉浸模式。
3. 在游戏首页截图，不要开始新游戏或覆盖已有进度。
4. 导出为 `inkbreak-immersive-en.jpg`。

### 3. Runtime 安装页

1. 临时把 Obsidian 界面语言切换为 **English**。
2. 打开 **Settings → Interactive Vault Runtime → Interactive packages**。
3. 确认画面中没有私人信息或无关通知后截图。
4. 导出为 `runtime-package-install-en.jpg`。
5. 如有需要，将 Obsidian 语言恢复为原来的设置。

## 放置位置 / Destination

把英文截图直接放到：

```text
vault-arcade-releases/assets/screenshots/
```

最终目录应如下：

```text
assets/screenshots/
├── README.md
├── vault-arcade-home-zh.jpg
├── vault-arcade-home-en.jpg
├── inkbreak-immersive-zh.jpg
├── inkbreak-immersive-en.jpg
├── runtime-package-install-zh.jpg
└── runtime-package-install-en.jpg
```

文件名区分大小写。不要只修改扩展名来转换图片格式；如果原图是 PNG，请在图片工具中真正导出为 JPEG。
