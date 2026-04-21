# Lintalist 中文版说明

Lintalist 是一个 Windows 上的开源文本扩展器、Snippet 管理器和可搜索文本片段工具。它可以把常用文本保存到可交换的 Bundle 中，并支持增量搜索、快捷键、缩写触发、交互式插件、AutoHotkey 脚本、HTML/Markdown/RTF/图片等格式化文本。

## 完整中文文档

完整中文文档已整理为独立 HTML 页面：

[打开 docs/index_cn.html](docs/index_cn.html)

英文原文档仍保留在：

[打开 docs/index.html](docs/index.html)

`docs/index_cn.html` 可直接双击在浏览器中打开，也可作为 Lintalist 的中文参考文档继续独立存在。

## 快速开始

1. 下载或解压 Lintalist 到一个有写权限的目录，不建议放在 `C:\Program Files`。
2. 如果已经安装 AutoHotkey，运行 `lintalist.ahk`。
3. 如果没有安装 AutoHotkey，运行 `lintalist.exe`。
4. 默认按 `CapsLock` 打开 Lintalist 搜索窗口。
5. 输入关键词搜索 Snippet，按 `Enter` 粘贴 Part 1，按 `Shift+Enter` 粘贴 Part 2。
6. 按 `F7` 新增 Snippet，按 `F4` 编辑选中的 Snippet，按 `F10` 编辑 Bundle 属性。

## 主要能力

- 全文搜索 Snippet，支持 Regular、Fuzzy、RegEx、Magic 四种搜索模式。
- 根据当前窗口标题或程序名自动加载上下文相关 Bundle。
- 使用快捷键 Hotkey 直接触发常用 Snippet。
- 使用 Shorthand 缩写展开常用文本。
- 通过 `[[Input]]`、`[[Choice]]`、`[[DateTime]]`、`[[Counter]]`、`[[Selected]]`、`[[Clipboard]]` 等插件生成交互式文本。
- 支持运行 AutoHotkey 脚本。
- 支持本地变量，适合保存姓名、地址、签名等个人信息。
- 支持 HTML、Markdown、RTF 和图片格式化 Snippet。
- 支持 Bundle 转换器，可从列表、CSV、UltraEdit、Texter 等格式导入。
- 便携使用，设置和 Bundle 都保存在程序目录中。

## 常用快捷键

| 快捷键 | 说明 |
| --- | --- |
| `CapsLock` | 打开搜索窗口，默认热键。 |
| `Ctrl+CapsLock` | 以 OmniSearch 模式搜索所有 Bundle。 |
| `Enter` | 粘贴选中 Snippet 的 Part 1，或运行脚本。 |
| `Shift+Enter` | 粘贴选中 Snippet 的 Part 2，或运行脚本。 |
| `Ctrl+Enter` | 粘贴 Part 1，但不运行脚本。 |
| `Ctrl+Shift+Enter` | 粘贴 Part 2，但不运行脚本。 |
| `Alt+Enter` | 只复制 Part 1 到剪贴板。 |
| `Alt+Shift+Enter` | 只复制 Part 2 到剪贴板。 |
| `F2` | 在搜索窗口中切换 OmniSearch。 |
| `F4` | 编辑 Snippet。 |
| `F5` | 复制 Snippet 并编辑。 |
| `F6` | 移动 Snippet 到另一个 Bundle。 |
| `F7` | 新增 Snippet。 |
| `F8` | 删除 Snippet。 |
| `F10` | 编辑 Bundle 属性。 |

## 重要文件

| 文件或目录 | 用途 |
| --- | --- |
| `lintalist.ahk` | 主程序源码。 |
| `lintalist.exe` | 便携版可执行入口，本质是重命名后的 AutoHotkey.exe。 |
| `settings.ini` | 主配置文件。手动编辑前请先退出 Lintalist。 |
| `bundles\` | Bundle 文件目录。 |
| `bundles\backup\` | 编辑或删除 Snippet 后的 Bundle 备份目录。 |
| `local\local.txt` | 本地变量文件。 |
| `plugins\` | 内置插件与自定义插件目录。 |
| `docs\index_cn.html` | 完整中文文档。 |
| `docs\index.html` | 英文原文档。 |

## 安全提示

Lintalist 可以运行 AutoHotkey 脚本，因此导入第三方 Bundle 前请检查每个 Snippet 的脚本部分。如果只是试用不熟悉的 Bundle，可先通过托盘菜单选择 `Pause scripts` 暂停脚本。

## 资源链接

- Lintalist 项目主页：[https://github.com/lintalist/lintalist](https://github.com/lintalist/lintalist)
- 最新发布版：[https://github.com/lintalist/lintalist/releases](https://github.com/lintalist/lintalist/releases)
- Bundle 仓库：[https://github.com/lintalist/lintalist-bundles](https://github.com/lintalist/lintalist-bundles)
- 主题仓库：[https://github.com/lintalist/lintalist-themes](https://github.com/lintalist/lintalist-themes)
- AutoHotkey：[https://autohotkey.com/](https://autohotkey.com/)

## 版权

Copyright 2009-2026 Lintalist. See `license.txt`.