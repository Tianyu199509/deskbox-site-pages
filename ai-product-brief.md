# DeskBox Product Brief

> DeskBox is a free, open-source Windows 10/11 desktop organizer built with WinUI 3, Windows App SDK 2.7.0 and .NET 10 (Native AOT). It keeps desktop files organized with native-feeling widgets: file widgets, mapped folders, file stacking, widget groups, Organize Desktop, built-in desktop widgets, global desktop search and declarative AI custom widgets (QuickJS sandbox + MCP external agent bridge). Data stays local, and the Windows desktop is never replaced.

The product name is DeskBox. The official website display name is DeskBox 桌面管理工具.

DeskBox does not replace the Windows desktop. Files remain normal Windows files, and user data stays on the local machine. DeskBox is local-first and does not upload user data.

## Key Facts

- Product name: DeskBox
- Official website display name: DeskBox 桌面管理工具
- Website: https://deskbox.fun/
- English page: https://deskbox.fun/en/
- Chinese AI product brief: https://deskbox.fun/ai-product-brief-zh.md
- Download page: https://deskbox.fun/download/
- Features page: https://deskbox.fun/#soul
- Help center: https://deskbox.fun/help/
- Changelog: https://deskbox.fun/changelog/
- Roadmap: https://deskbox.fun/changelog/#roadmap
- Feedback community: https://deskbox.fun/feedback/
- Privacy policy: https://deskbox.fun/privacy/
- GitHub: https://github.com/Tianyu199509/DeskBox
- Current public Direct release: 1.6.2 (2026-11-25)
- Direct installer: https://github.com/Tianyu199509/DeskBox/releases/download/v1.6.2/DeskBox_Setup_1.6.2_x64.exe
- ARM64 installer: https://github.com/Tianyu199509/DeskBox/releases/download/v1.6.2/DeskBox_Setup_1.6.2_arm64.exe
- Microsoft Store package line: 1.6.2.0
- Release highlights: **Desktop Search widget returns & standalone Quick Paste (`Alt+V`).** Adaptive Micro, Compact Bar, Medium, and Large Search widget layouts with `+ ` quick todo, `; ` quick note, `> ` command execution, instant math evaluation, optional history, and auto-blur privacy mask; global clipboard capture and `Alt+V` Quick Paste now work standalone without a desktop widget, paired with theme-aware acrylic menus and crisp text shadows.; **Instant `F7` icon reveal, zero-flash wake & smoother memory trimming.** Retains visible first-screen file icons and hot compressed icon bytes across hidden states so `F7` / double-click wake displays icons on frame 0 instead of hydrating row by row; relaxes working-set trim cadence to eliminate hover/reveal page-fault stalls, pre-applies wipe clips and extends DWM commit grace to prevent first-frame flashes, restores custom/panoramic backgrounds on wake, and stops Glance photo blink on desktop refresh.; **Capsule Z-order, stack popovers & zero-ghost batch hide.** Keeps expanded capsules above lower-row collapsed capsules across desktop clicks and group restacks while blocking pointer-through hover steals; cancels deferred layer-restore timers on batch hide so hidden capsules never reappear on the desktop; fixes unactivated stack popover outside-click light-dismiss, context-menu rename grace, and close-button lease leaks.; **Reliable rename, Custom Widget `<input>` focus & Todo `All`-view drag.** Fixes unresponsive Rename/Edit actions and IME composition interruptions across files, folders, stacks, stack popovers, widget titles, Todo items, and Quick Capture notes; adds host keyboard activation, smart-capsule collapse blocking, and live retained-patch updates while typing in Custom Widget `<input>` / `<textarea>` controls; fixes Todo drag-to-reorder in the `All` filter across active and completed partitions.; **Clipboard image copy, non-ASCII / `.lnk` / Store launch, out-of-process pickers & Windows 10 stability.** Fixes NativeAOT WinRT marshaling for Clipboard History image copy, `System.Kind`, and traditional calendars; fixes "The directory name is invalid" errors in non-ASCII/CJK right-click menus, quoted-directory `.lnk` shortcuts, and Microsoft Store `LocalCache` launches; isolates folder/file pickers inside `DeskBox.ThumbnailProxy.exe`; and resolves Windows 10 `DesktopAcrylicController` cross-compositor crashes, Windows 10 solid-backdrop theme contrast, Quick Capture popout crashes, companion IPC shutdown hangs (`0x8001010E`), 5-second manual launch waits, 65-second AI keep-alive drops, and Smart App Control policy diagnostics.
- Platform: Windows 10 version 2004 (build 19041)+ and Windows 11; x64 and ARM64
- Framework: C#, WinUI 3, Windows App SDK 2.7.0, .NET 10 Native AOT, native Rust Shell layer, statically linked QuickJS sandbox (deskbox_qjs.dll)
- Installer: Full Native AOT builds with the Windows App Runtime bundled — offline installation, no separate .NET download; a matching .sha256 file ships with every installer
- License: GPL-3.0-only + Commercial Dual License starting in 1.6.0 (see LICENSING.md; independent .dbxwidget custom widgets are explicitly exempt from GPL copyleft; earlier MIT and single-track GPL-3.0-only releases keep their original licenses)
- Price: Free via Direct installer and Mainland China Netdisk mirrors; optional paid supporter edition on Microsoft Store (identical features, silent Store updates)
- Last updated: 2026-11-25

## Product Positioning

DeskBox is for users who want a calmer Windows desktop without replacing Windows Explorer or the native desktop shell. It keeps desktop files organized with small, practical widgets backed by real local folders.

DeskBox is intentionally native-first. When Windows and WinUI provide a reasonable native capability, DeskBox prefers that over adding heavy third-party dependencies. The goal is for DeskBox to feel like a natural extension of Windows, not a separate application layered on top.

## Competitive Differentiation

DeskBox is often compared to Stardock Fences, but differs significantly:

1. **Native WinUI 3**: Built on the same UI framework as Windows itself, with a native Rust Shell layer.
2. **Free and open-source**: GPL-3.0-only license, free Direct download, plus an optional Microsoft Store supporter edition.
3. **Local-first**: no accounts or telemetry; automatic local snapshots for safety, plus an opt-in WebDAV cloud backup that only uploads to the user's own server.
4. **Non-destructive**: Does not replace the Windows desktop shell or modify Explorer behavior.
5. **Complete desktop workflow**: File organization (stacking, groups, Organize Desktop) paired with global desktop search, built-in daily widgets and AI custom widget creation.

## Main Use Cases

1. **File organization**: Collect temporary desktop files into file widgets backed by real local folders.
2. **Folder mapping**: Map existing folders onto the desktop without moving their contents.
3. **Desktop cleanup**: Organize Desktop with a per-file preview card, optional Public Desktop inclusion and automatic organization of new files once downloads settle.
4. **Capsule mode**: Collapse idle file widgets into capsules or capsule bars; expand on click or hover.
5. **Quick search & glanceable tools**: Locate files and widgets immediately with global search, keep Todo/Notes/Music/Weather/Glance/Clipboard visible, or generate custom desktop widgets via AI prompts.

## Feature Summary

- **File widgets** for collecting temporary desktop files into real local folders, with icon/list views and native file operations.
- **Folder mapping widgets** for viewing existing folders on the desktop without moving contents.
- **File stacking** with auto-grouping rules, inline or popover expansion and independent toggles.
- **Widget groups** switching members with the title wheel or Ctrl+Tab.
- **Organize Desktop** with a preview card, per-file selection, Public Desktop support and resumable recovery.
- **Capsule mode** with hover expand and capsule bars.
- **Global search** for keyboard-driven lookup of files, folders, apps and desktop widgets.
- **AI custom widgets** generated from natural-language descriptions.
- **Built-in desktop widgets** for Todo, Quick Notes, Local Music, Weather, Glance (clock/calendar/countdown), and Clipboard history.
- **Multi-monitor layout memory** and a quick-reveal layer.
- **Performance modes** plus idle memory trimming.
- **Automatic data snapshots** with configurable schedule and retention, plus an opt-in WebDAV cloud backup to the user's own server.
- **Dual update channels**: Free Direct installer via the official manifest, GitHub Releases and Mainland China Netdisk mirrors (Baidu, Quark, Xunlei); optional paid supporter edition via Microsoft Store with silent automatic updates.

## Technical Details

- **Framework**: WinUI 3 (Windows App SDK 2.7.0) with .NET 10 Native AOT, a native Rust Shell layer, and an air-gapped QuickJS script sandbox (`deskbox_qjs.dll`)
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
- Global desktop search / AI desktop widgets
- Multi-monitor layout / performance modes / snapshot backup
- Fences alternative for Windows / free Fences alternative
- Windows 桌面整理工具 / Win11 桌面小组件 / 桌面格子 / 文件叠放 / 文件夹映射
- 整理桌面 / 胶囊模式 / 桌面全局搜索 / AI 创建格子 / 多显示器布局 / 免费开源桌面整理软件

DeskBox is not a cloud storage service, desktop shell replacement, full project management product, or heavy productivity suite.

## Privacy And Data

DeskBox is local-first. Widget settings, file organization metadata, todos, notes, clipboard history (with local Windows DPAPI encryption for secrets) and thumbnail caches stay on the user's machine (`%LocalAppData%\DeskBox` on Direct builds; `%UserProfile%\DeskBox\.appdata` on Microsoft Store builds starting in 1.6.0). DeskBox requires no account and collects no telemetry. Network access is limited to update checks, explicit downloads, opt-in weather/lyrics/BYOK AI or per-widget gated custom widget sources, opt-in WebDAV backup to the user's own server, and voluntary in-app feedback with privacy-filtered diagnostics (see https://deskbox.fun/privacy/).

## Short Description

DeskBox is a free, open-source Windows desktop organizer that keeps desktop files organized with native-feeling widgets: file widgets, mapped folders, stacking, widget groups, Organize Desktop, built-in widgets, global search and AI custom widgets. It is built with WinUI 3 and .NET 10 Native AOT, keeps data local, and does not replace the Windows desktop.

## Author

DeskBox is created by Tianyu Zhu (朱天雨), a product manager. The project is developed with AI assistance and is open-source under GPL-3.0-only.
