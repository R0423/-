# 安装包备份仓库

本仓库用于备份各类软件安装包及使用说明，防止原项目丢失或下架。

## AIPS 0.2.0（Windows 中文版）

**AIPS** 是一个面向 Windows 的开源图像编辑器，基于 Compositor 开发，支持 PSD 图层导入和接近 Photoshop 的常用快捷键。

- 原项目地址：[whiteg2030-alt/-PS-win-psd-](https://github.com/whiteg2030-alt/-PS-win-psd-)
- 版本：v0.2.0
- 平台：Windows 11 x64 / Windows 10 22H2 x64（19045 及以上）
- 安装包大小：约 260 MB

### 主要功能

- 简体中文界面
- PSD / PSB 图层导入（支持分组、蒙版、混合模式等）
- PS 常用快捷键（Ctrl+O、Ctrl+J、Ctrl+T、Ctrl+G、Ctrl+E 等）
- Alt + 滚轮缩放、Alt + 点击图层眼睛独显
- 保留 Compositor 的图层、蒙版、选区、画笔、滤镜等编辑能力
- 离线背景移除

### 文件说明

| 文件 | 说明 |
|------|------|
| `AIPS-0.2.0-Windows-x64.zip` | 主安装包（见 Release 附件） |
| `aips-install.md` | 安装说明 |
| `aips-windows-zh.png` | 软件截图 |
| `AIPS-0.2.0-Windows-x64.zip.sha256` | SHA256 校验码 |

### 安装方法

1. 下载 `AIPS-0.2.0-Windows-x64.zip`（在 Releases 中）
2. 右键「全部解压」
3. 双击 `Install-AIPS.cmd`
4. 从桌面快捷方式启动

详细说明见 [aips-install.md](aips-install.md)。

### 注意事项

- 本仓库仅作备份用途，请支持原项目
- 构建尚未数字签名，如遇 SmartScreen 提示请选择「仍要运行」
- 保存格式为 .comp 工程文件夹，不支持写回 PSD，可导出 PNG/JPEG
