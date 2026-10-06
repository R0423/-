# AIPS 安装说明 / Installation

## 简体中文

下载 Releases 的 AIPS-0.2.0-Windows-x64.zip，右键「全部解压」，双击 Install-AIPS.cmd。不要从压缩包窗口内直接运行。安装脚本核对文件 SHA256，复制到 %LOCALAPPDATA%\Programs\AIPS\0.2.0，运行离线模型和运行库自检，然后创建桌面、开始菜单中的 AIPS 快捷方式。

适用 Windows 11 x64 和 Windows 10 22H2 x64（19045+），Intel/AMD。无需管理员权限。没有 Mac、ARM64 或 32 位 Windows 包。本地构建没有数字签名。

便携使用：直接启动 AIPS/AIPS.exe。给另一台电脑使用时复制整个解压目录，不要只拷贝 exe。旧版本目录会保留；保存工作后自行退出旧程序，再启动 AIPS。安装不会强制关闭旧窗口，也不改变 PSD 默认关联。

打开 PSD：Ctrl+O；打开 .comp 工程：Ctrl+Alt+O。Ctrl+S 保存 .comp 文件夹，不会写回 PSD。文字和智能对象等按缓存像素导入，高级效果可能不同。更多内容见 README 和快捷键说明。

卸载：先退出该版本，删除上述版本目录及指向它的 AIPS 快捷方式。自己的 .comp 工程应保留。重复运行安装程序会校验同一版本；遇到内容不同的已存在目录会停止，避免覆盖。

自动化检查：powershell.exe -NoProfile -ExecutionPolicy Bypass -File ./Install-AIPS.ps1 -Plan。自动化安装可用 -NoLaunch；ExecutionPolicy 只影响本次进程，不修改系统策略。

## English

Download the Windows x64 ZIP from Releases, extract it completely, and run Install-AIPS.cmd. The script verifies SHA256 checksums, installs per user at %LOCALAPPDATA%\Programs\AIPS\0.2.0, checks runtime/model health and creates AIPS shortcuts. No administrator rights or development tools are needed.

Windows 11 x64 and Windows 10 22H2 x64 (19045+) on Intel/AMD are supported. The build is unsigned; no macOS, ARM64 or 32-bit build is included. For portable use, run AIPS/AIPS.exe with all accompanying files present.

Save work and close older versions yourself; the installer does not terminate editing sessions or change PSD file associations. Ctrl+O imports PSD/PSB; Ctrl+Alt+O opens a .comp project. Saving writes .comp, not PSD. Read the compatibility table before editing important documents.

To uninstall, exit AIPS and remove its version folder and shortcuts. Keep your own project folders. Install-AIPS.ps1 -Plan validates without installing; -NoLaunch installs without opening the editor.
