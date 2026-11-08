# vibTTY

为 coding agent 打造的 macOS 终端。Claude Code、Codex、tilx 现在是在跑、在等你确认、已经跑完还是出错了,面板标题栏、侧栏和 Agent 面板上一眼就能看到;需要你处理时,还会用系统通知提醒你。

这个仓库只放安装包和自动更新源,不含源码。

## 下载安装

1. 打开[最新版本](https://github.com/his1devil/vibTTY-releases/releases/latest),在 Assets 里下载 `vibTTY-版本号.dmg`。
2. 双击 DMG,把 vibTTY 拖进「应用程序」。
3. 从「应用程序」或 Spotlight 打开 vibTTY。第一次打开时 macOS 会提示这是从互联网下载的 App,点「打开」即可。

安装包有 Developer ID 签名,并通过了 Apple 公证,不需要去「隐私与安全性」里手动放行。

**系统要求**:macOS 13 或更高版本,Apple Silicon(M 系列芯片)的 Mac。暂不支持 Intel Mac。

## 开始用

1. 第一次启动时,如果检测到 Claude Code、Codex 或 tilx,vibTTY 会问「在侧栏显示 agent 状态?」,点「安装 Hook」。
2. 之后照常在 vibTTY 里启动 `claude`、`codex` 或 `tilx`,状态会自动显示出来。按 ⌘J 跳到正在等你处理的 agent。
3. 新版 Codex 第一次启动时会让你审核外部 Hook,选「Trust all and continue」,vibTTY 才能显示 Codex 的状态。

## 更新

从 0.6.0 起,vibTTY 会自动检查更新。有新版本时会弹窗提示,按提示就能下载、安装并重启,不用再手动下载 DMG。

- 手动检查:菜单栏「vibTTY › 检查更新…」
- 关闭自动检查:「设置 › 关于 › 更新」
- 0.5.0 及更早的版本还没有自动更新,需要手动下载安装一次。

每个更新包除了经过 Apple 公证,还带 vibTTY 自己的更新签名,校验不通过就不会安装。

各版本的改动见 [Releases](https://github.com/his1devil/vibTTY-releases/releases)。

## English

vibTTY is a macOS terminal built for coding agents. For Claude Code, Codex and tilx it shows whether each agent is running, waiting for you, done or failed (in the pane title bar, the sidebar and an Agents panel) and sends a notification when one needs you.

This repository only hosts installers and the update feed; there is no source code here.

- **Install**: download the `.dmg` from the [latest release](https://github.com/his1devil/vibTTY-releases/releases/latest), open it and drag vibTTY into Applications. It is signed with a Developer ID and notarized by Apple.
- **Requirements**: macOS 13 or later on Apple Silicon. Intel Macs are not supported.
- **Agent status**: on first launch vibTTY offers to install its status hooks for the agents it finds. Newer Codex versions ask you to review external hooks; choose "Trust all and continue".
- **Updates**: from 0.6.0 on, vibTTY checks for updates itself (vibTTY › Check for Updates…). Every update is notarized and EdDSA-signed, and vibTTY won't install one that fails verification.
