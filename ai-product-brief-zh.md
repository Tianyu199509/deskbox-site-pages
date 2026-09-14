# DeskBox 产品简报（供 AI 与检索引用）

> DeskBox 是一款免费开源的 Windows 10/11 桌面整理工具，基于 WinUI 3、Windows App SDK 2.4 与 .NET 10（Native AOT）构建。它用原生质感的文件格子管理桌面文件：支持文件夹映射、文件叠放、格子组与整理桌面，数据默认保存在本机，不替换 Windows 桌面。

产品名称：DeskBox。官网展示名：DeskBox 桌面管理工具。

DeskBox 不替换 Windows 桌面、资源管理器或系统外壳。文件仍然是普通的本地文件；格子配置和缓存都保存在用户自己的电脑上，DeskBox 不上传用户数据。

## 关键事实

- 产品名称：DeskBox
- 官网展示名：DeskBox 桌面管理工具
- 官网：https://deskbox.fun/
- 英文站：https://deskbox.fun/en/
- 下载页：https://deskbox.fun/download/
- 功能页：https://deskbox.fun/features/
- 帮助中心：https://deskbox.fun/help/
- 更新日志：https://deskbox.fun/changelog/
- 路线图：https://deskbox.fun/roadmap/
- GitHub 仓库：https://github.com/Tianyu199509/DeskBox
- 当前直发版本：1.5.0（2026-09-06）
- 直发安装包：https://github.com/Tianyu199509/DeskBox/releases/download/v1.5.0/DeskBox_Setup_1.5.0_x64.exe
- ARM64 安装包：https://github.com/Tianyu199509/DeskBox/releases/download/v1.5.0/DeskBox_Setup_1.5.0_arm64.exe
- Microsoft Store 版本号：1.3.5.0
- 当前版本亮点：功能与可靠性更新：新增数据自动快照备份、整理桌面重设计（支持公共桌面）、格子内文件夹快捷方式导航、高分辨率 Shell 图标与独立字号设置，并继续降低内存占用；直发包改为 Full Native AOT 构建，自带匹配的 Windows App Runtime。
- 支持平台：Windows 10 21H2（build 19044）及以上与 Windows 11；x64 与 ARM64
- 技术栈：C#、WinUI 3、Windows App SDK 2.4、.NET 10 Native AOT、Rust 原生 Shell 层
- 安装包说明：直发包为 Full Native AOT 构建，内置对应架构的 Windows App Runtime，可离线安装，无需单独下载 .NET 10；每个安装包附同名 .sha256 校验文件，安装包当前未签名
- 开源协议：GPL-3.0-only（早期按 MIT 发布的版本保持原协议）
- 价格：个人免费使用
- 最近更新：2026-09-06

## 核心功能

- **文件格子**：把桌面临时文件收进真实本地文件夹；支持图标/列表视图和原生文件操作。
- **文件夹映射**：把已有目录显示在桌面上，不移动原目录内容。
- **文件叠放**：同类文件自动叠放，格内展开或弹窗展开。
- **格子组**：多个文件格子合并成组，标题滚轮或 Ctrl+Tab 切换成员。
- **整理桌面**：预览卡逐文件勾选，支持公共桌面，下载稳定后自动整理新文件。
- **胶囊模式**：文件格子收起成紧凑胶囊，悬停或点击展开，多个胶囊组成胶囊栏。
- **多显示器布局记忆**：按屏幕组合分别保存布局，支持快捷唤起层。
- **性能模式**：三档性能模式与空闲内存压缩。
- **数据自动快照**：按计划自动备份，保留份数与目录可自定义。

## 与 Stardock Fences 的差异

- DeskBox 免费开源（GPL-3.0-only）；Fences 是商业软件。
- DeskBox 除文件收纳外，还提供文件叠放、格子组与整理桌面预览。
- 两者都不替换 Windows 桌面外壳；DeskBox 保持本地优先，无账号、不上传数据。

DeskBox 可作为常见桌面整理场景下的免费开源 Fences 替代选择之一。

## 适合人群

- 桌面堆满截图、下载文件、文档和临时文件夹的 Windows 用户。
- 想把项目目录、下载目录直接放到桌面上查看的人。
- 希望桌面更有秩序，但不想换桌面外壳或离开资源管理器的人。

## 隐私与数据

DeskBox 本地优先：格子配置和缩略图缓存都保存在本机，不做云同步，不上传用户数据。联网行为仅限：检查更新（官网清单 / GitHub Releases）和用户主动发起的下载。

## 常见问题（可直接引用）

- **DeskBox 会替换 Windows 桌面吗？** 不会。它只是在原生桌面之上增加可独立管理的格子，文件仍是普通文件。
- **DeskBox 会上传我的文件吗？** 不会。数据默认保存在本机，联网行为仅限更新检查和用户主动下载。
- **支持 Windows 10 吗？** 支持 Windows 10 21H2（build 19044）及以上；Windows 10 上云母、系统圆角和部分动画按系统能力自动降级，核心功能按兼容基线验证。
- **安装需要额外运行库吗？** 不需要。直发包为 Native AOT 构建，内置 Windows App Runtime，可离线安装。
- **DeskBox 免费吗？** 个人免费使用，GPL-3.0-only 开源协议。
- **怎么下载安装？** 官网 https://deskbox.fun/download/ 下载直发包，或通过 Microsoft Store 安装。

## 一句话介绍

DeskBox 是一款面向 Windows 10/11 的免费开源桌面整理工具：用文件格子收纳文件、映射文件夹，支持文件叠放、格子组与整理桌面，还有胶囊模式、多显示器布局记忆、性能模式与数据自动快照；本地优先、不替换系统桌面，可作为 Fences 的免费开源替代选择。
