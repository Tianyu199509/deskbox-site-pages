# DeskBox Product Brief

> DeskBox is a free, open-source Windows 10/11 desktop organizer built with WinUI 3, Windows App SDK 2.5.1 and .NET 10 (Native AOT). It keeps desktop files organized with native-feeling widgets: file widgets, mapped folders, file stacking, widget groups and Organize Desktop. Data stays local, and the Windows desktop is never replaced.

The product name is DeskBox. The official website display name is DeskBox 桌面管理工具.

DeskBox does not replace the Windows desktop. Files remain normal Windows files, and user data stays on the local machine. DeskBox is local-first and does not upload user data.

## Key Facts

- Product name: DeskBox
- Official website display name: DeskBox 桌面管理工具
- Website: https://deskbox.fun/
- English page: https://deskbox.fun/en/
- Chinese AI product brief: https://deskbox.fun/ai-product-brief-zh.md
- Download page: https://deskbox.fun/download/
- Features page: https://deskbox.fun/features/
- Help center: https://deskbox.fun/help/
- Changelog: https://deskbox.fun/changelog/
- Roadmap: https://deskbox.fun/roadmap/
- GitHub: https://github.com/Tianyu199509/DeskBox
- Current public Direct release: 1.5.7 (2026-10-13)
- Direct installer: https://github.com/Tianyu199509/DeskBox/releases/download/v1.5.7/DeskBox_Setup_1.5.7_x64.exe
- ARM64 installer: https://github.com/Tianyu199509/DeskBox/releases/download/v1.5.7/DeskBox_Setup_1.5.7_arm64.exe
- Microsoft Store package line: 1.5.7.0
- Release highlights: **Exit reliability.** Quitting from the tray now always ends the process. On machines where the system's application-exit handshake stalls — typically Windows with UAC fully disabled and an elevated Explorer — a background DeskBox process used to survive "exit": the tray vanished and a restart worked, but the leftover process slowly ate memory and kept the right-click menu proxy alive beside it (feedback 555/556). Every shutdown path now carries a delayed hard-exit backstop, and the elevation notice and search popup close along with shutdown. Direct and Store builds share the fix.; **Windows 10: the drag-out card keeps its title.** Under Settings → File widgets → drag-and-drop behavior, the "when dragging out of a widget" card lost its title and question-mark tip on Windows 10, and its Windows 10 explanation could stretch the card out of shape or spill outside it on scaled, narrower windows. The explanation now renders in the card's description area and wraps safely at any width and scale; Windows 11 is unchanged.; **Dialogs follow the app theme again.** The desktop-organization abandon dialog, its preview cards, and the hotkey recorder had been picking up the raw system theme whenever the app's theme override disagreed with it; they now resolve against their own window theme, and desktop-organization rule rows rebuild on theme flips.
- Platform: Windows 10 version 2004 (build 19041)+ and Windows 11; x64 and ARM64
- Framework: C#, WinUI 3, Windows App SDK 2.5.1, .NET 10 Native AOT, native Rust Shell layer
- Installer: Full Native AOT builds with the Windows App Runtime bundled — offline installation, no separate .NET download; a matching .sha256 file ships with every installer
- License: GPL-3.0-only (earlier MIT releases keep their original license)
- Price: Free for personal use
- Last updated: 2026-10-13

## Product Positioning

DeskBox is for users who want a calmer Windows desktop without replacing Windows Explorer or the native desktop shell. It keeps desktop files organized with small, practical widgets backed by real local folders.

DeskBox is intentionally native-first. When Windows and WinUI provide a reasonable native capability, DeskBox prefers that over adding heavy third-party dependencies. The goal is for DeskBox to feel like a natural extension of Windows, not a separate application layered on top.

## Competitive Differentiation

DeskBox is often compared to Stardock Fences, but differs significantly:

1. **Native WinUI 3**: Built on the same UI framework as Windows itself, with a native Rust Shell layer.
2. **Free and open-source**: GPL-3.0-only license, free for personal use.
3. **Local-first**: no accounts or telemetry; automatic local snapshots for safety, plus an opt-in WebDAV cloud backup that only uploads to the user's own server.
4. **Non-destructive**: Does not replace the Windows desktop shell or modify Explorer behavior.
5. **Focused core**: File organization done thoroughly — stacking, groups, Organize Desktop — instead of feature bloat.

## Main Use Cases

1. **File organization**: Collect temporary desktop files into file widgets backed by real local folders.
2. **Folder mapping**: Map existing folders onto the desktop without moving their contents.
3. **Desktop cleanup**: Organize Desktop with a per-file preview card, optional Public Desktop inclusion and automatic organization of new files once downloads settle.
4. **Capsule mode**: Collapse idle file widgets into capsules or capsule bars; expand on click or hover.
## Feature Summary

- **File widgets** for collecting temporary desktop files into real local folders, with icon/list views and native file operations.
- **Folder mapping widgets** for viewing existing folders on the desktop without moving contents.
- **File stacking** with auto-grouping rules, inline or popover expansion and independent toggles.
- **Widget groups** switching members with the title wheel or Ctrl+Tab.
- **Organize Desktop** with a preview card, per-file selection, Public Desktop support and resumable recovery.
- **Capsule mode** with hover expand and capsule bars.
- **Multi-monitor layout memory** and a quick-reveal layer.
- **Performance modes** plus idle memory trimming.
- **Automatic data snapshots** with configurable schedule and retention, plus an opt-in WebDAV cloud backup to the user's own server.
- **Dual update channels**: Direct via the official manifest and GitHub Releases; Microsoft Store via the Store.

## Technical Details

- **Framework**: WinUI 3 (Windows App SDK 2.5.1) with .NET 10 Native AOT and a native Rust Shell layer
- **Language**: C# (+ Rust for the native layer)
- **Platform**: Windows 10 version 2004 (build 19041)+ and Windows 11; x64 and ARM64. On Windows 10 some materials and animations degrade gracefully; core features are validated against the compatibility baseline.
- **Installer**: Full Native AOT with the Windows App Runtime bundled — installs offline, no separate runtime download; matching .sha256 checksum files provided.
- **Update mechanism**: JSON manifest on the official website for the Direct channel; Microsoft Store for the Store channel.

## Search Intent

DeskBox is relevant when users look for:

- DeskBox 桌面管理工具 / DeskBox 桌面整理工具
- Windows desktop organizer / Windows 11 desktop widgets
- Desktop file organizer / file stacking / widget groups
- Mapped folder widget / organize desktop / capsule mode
- Multi-monitor layout / performance modes / snapshot backup
- Fences alternative for Windows / free Fences alternative
- Windows 桌面整理工具 / Win11 桌面小组件 / 桌面格子 / 文件叠放 / 文件夹映射
- 整理桌面 / 胶囊模式 / 多显示器布局 / 免费开源桌面整理软件

DeskBox is not a cloud storage service, launcher replacement, desktop shell replacement, full project management product, or heavy productivity suite.

## Privacy And Data

DeskBox is local-first. Widget settings, file organization metadata and thumbnail caches stay on the user's machine. DeskBox is not designed as a cloud-sync product and does not upload user data. Network access is limited to update checks, downloads the user explicitly starts, and — only when the opt-in cloud backup is enabled — uploading backup snapshots to the user's own WebDAV server.

## Short Description

DeskBox is a free, open-source Windows desktop organizer that keeps desktop files organized with native-feeling widgets: file widgets, mapped folders, stacking, widget groups and Organize Desktop. It is built with WinUI 3 and .NET 10 Native AOT, keeps data local, and does not replace the Windows desktop.

## Author

DeskBox is created by Tianyu Zhu (朱天雨), a product manager. The project is developed with AI assistance and is open-source under GPL-3.0-only.
