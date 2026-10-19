# PhD Pilot · 下载

PhD Pilot 是一个面向个人科研工作的 Windows 桌面工具，用于集中管理项目、资源入口、任务和手工进度。原始资料继续在 Obsidian、WPS、飞书或本地 Office 等来源中维护。

**当前版本：0.1.0-alpha.10.3 · Windows 11 x64 · Alpha 预发布**

[下载安装包](https://github.com/blackblues360/phd-pilot-downloads/releases/download/v0.1.0-alpha.10.3/PhD.Pilot_0.1.0-alpha.10.3_x64-setup.exe) · [版本说明](https://github.com/blackblues360/phd-pilot-downloads/releases/tag/v0.1.0-alpha.10.3) · [全部版本](https://github.com/blackblues360/phd-pilot-downloads/releases)

本仓库公开提供使用说明和安装包，不包含应用源码、内部设计文档、运行数据库或用户备份。无需登录 GitHub 即可查看和下载。

## 安装与升级

1. 下载 **PhD.Pilot_0.1.0-alpha.10.3_x64-setup.exe**。
2. 运行安装程序，按提示完成当前 Windows 用户的安装。本版面向 Windows 11 x64，使用 WebView2 Runtime。
3. 首次启动为空工作区，可先创建项目，再添加资料索引；在 Connections 中选择要连接的来源。

升级前请先在 Settings 导出 Pilot 备份并退出旧版，再安装新版。本版数据库结构保持 schema11。Pilot 备份不包含外部文档、附件或网站登录状态，原稿需在原应用中另行备份。

应用仍在 Alpha 阶段，尚未进行 Windows 数字签名，也没有自动更新；后续版本从本仓库的 Releases 下载。

## 可以做什么

| 功能 | 说明 |
|---|---|
| 项目看板 | 项目范围切换，调整并保存卡片布局 |
| 资料索引 | 用标题、链接、文件路径、标签和项目关联整理资料入口 |
| 任务与进度 | 内部任务、甘特视图、实验状态与手工进度树 |
| 本地文件与 Obsidian | 选定目录的受限索引、文件位置认领及手动元数据同步 |
| 内置浏览器 | 多页签、搜索、常用网站、登录会话，以及经确认的地址索引保存 |
| 个人 WPS 云文档 | 登录入口、原地址登记，以及经确认后转到 WPS Office 客户端 |
| 飞书日历 | 配置 CalDAV 后只读展示日程并自动刷新 |
| 备份恢复 | 导出和恢复 Pilot 自己的索引、关联与手工数据 |

## alpha10.3 说明

- WPS：在云文档文件菜单选择“用 WPS Office 打开”，再由 Pilot 确认启动客户端。需要已安装 WPS，并使用有权限的账号。点击索引一步直达客户端尚未实现。
- 飞书日历：使用现有 CalDAV 配置，启动、可见期间每 5 分钟及返回窗口时检查更新；失败保留上次结果，成功空结果清除旧日程。
- WPS 的来源核验和确认/取消已通过隔离页面测试；安装版真实账号登录后跳转、跨重启及其他文档类型仍待验收。

当前未提供 WPS 云目录 API 同步，不承诺所有云文档类型兼容。Pilot 维护索引与关系，外部原稿仍由来源应用管理；用户主动浏览网页与索引器获准读取的元数据是不同范围。

## 下载完整性

安装包 **PhD.Pilot_0.1.0-alpha.10.3_x64-setup.exe** 的 SHA-256：

```text
E8AFE6FB5EF8F2992FACA7C2D298089CDC960FCB9CCB6CEBF1ED125F445A5933
```

可在 PowerShell 中核对：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\PhD.Pilot_0.1.0-alpha.10.3_x64-setup.exe'
```

本下载仓库独立于应用源码仓库，不附带开发历史或个人科研资料。GitHub 自动提供的 Source code 压缩包仅包含本仓库的 README；安装软件请下载上方的 exe 安装包。
