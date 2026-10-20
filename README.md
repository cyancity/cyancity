<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img src="assets/banner-light.svg" width="100%" alt="YOLO: I build tools that let AI agents do real work without being handed your secrets. Stack: TypeScript, React, Node.js, Go, Kotlin, Swift, Python, Shell, Cloudflare Workers.">
</picture>

<p align="center">
  <sub><b>主推</b> skill 集合 → <b>主力</b> easy-unlocker、yolo-bot → <b>工具</b> hy2-proxy-setup → <b>自用</b> kindle-gadget</sub>
</p>

### 01 · 主推 · [curated-agent-skills](https://github.com/cyancity/curated-agent-skills)

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/skills-dark.svg">
  <img src="assets/skills-light.svg" width="100%" alt="两个已审阅技能：dycopy 用于媒体归档，包工头（herdr-subagent）用于 agent 协作">
</picture>

<sub>SKILL.md · JSON · MIT — 找“包工头”skill 就点这里：<a href="https://github.com/cyancity/curated-agent-skills/tree/main/skills/herdr-subagent"><code>herdr-subagent</code></a></sub>

- :white_check_mark: **强项** — 每个 skill 人工审阅、脱敏后才公开，`catalog.json` 让 agent 自己按任务匹配；包工头让一个 agent 派活给其他 CLI agent，并逐个验收交付物。
- :warning: **局限** — 目前只有 2 个 skill；包工头要先装 Herdr CLI。
- :arrow_right: **入口** — [包工头](https://github.com/cyancity/curated-agent-skills/tree/main/skills/herdr-subagent) · [全部 skill](https://github.com/cyancity/curated-agent-skills)

---

### 02 · 主力

<table>
  <tr>
    <td width="50%" valign="top">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="assets/easy-unlocker-dark.png">
        <img src="assets/easy-unlocker-light.png" width="100%" alt="easy-unlocker logo">
      </picture>
      <h4><a href="https://github.com/cyancity/easy-unlocker">easy-unlocker</a> <sub>Kotlin · Swift · Go</sub></h4>
      <img src="https://img.shields.io/github/v/release/cyancity/easy-unlocker?color=2f9e44" alt="release"> <img src="https://img.shields.io/github/stars/cyancity/easy-unlocker?color=2f9e44" alt="stars">
      <p><sub>Agent 要密钥时，明文不进对话、日志和磁盘；指纹在另一台设备上批准，值端到端加密直达进程。</sub></p>
      <p>:white_check_mark: <b>强项</b> — 审批不在请求方机器上，无屏服务器和 CI 也能用；有正式 Release 和现成 skill。<br>
      :warning: <b>局限</b> — 桌面端只有 Windows 端到端测过，macOS 未测且不在 Releases；不是密码管理器，不做浏览器自动填充。<br>
      :arrow_right: <b>入口</b> — <a href="https://github.com/cyancity/easy-unlocker/releases/latest">下载</a> · <a href="https://easy-unlocker.pages.dev/">站点</a> · <a href="https://github.com/cyancity/easy-unlocker/blob/main/docs/AGENTS-SETUP.md">Agent 手册</a></p>
    </td>
    <td width="50%" valign="top">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="assets/yolo-bot-dark.png">
        <img src="assets/yolo-bot-light.png" width="100%" alt="yolo-bot channel view with the Lead and employees">
      </picture>
      <h4><a href="https://github.com/cyancity/yolo-bot">yolo-bot</a> <sub>TypeScript · React</sub></h4>
      <img src="https://img.shields.io/github/v/release/cyancity/yolo-bot?include_prereleases&color=0b7285" alt="release"> <img src="https://img.shields.io/github/stars/cyancity/yolo-bot?color=0b7285" alt="stars">
      <p><sub>DeepSeek Harness 里的数字员工团队：只跟负责人说需求，它拆解、派工、汇总。</sub></p>
      <p>:white_check_mark: <b>强项</b> — 每个员工有自己的模型、skill 和记忆，换任务不用重新交代；成果落成文件，有版本能定稿。<br>
      :warning: <b>局限</b> — 绑定 DSH 0.2.1-rc.2，自身还在 pre-release；偶尔问一两句的场景用不上。<br>
      :arrow_right: <b>入口</b> — <a href="https://github.com/cyancity/yolo-bot/releases">下载</a> · <a href="https://github.com/cyancity/yolo-bot#快速开始">快速开始</a></p>
    </td>
  </tr>
</table>

### 03 · 工具 · [hy2-proxy-setup](https://github.com/cyancity/hy2-proxy-setup)

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/hy2-proxy-setup-dark.svg">
  <img src="assets/hy2-proxy-setup-light.svg" width="220" alt="hy2-proxy-setup shield icon">
</picture>

<sub>Shell · PowerShell · MIT — 不是产品，是一份能直接交给 agent 执行的部署 SOP</sub>

- :white_check_mark: **强项** — 一条命令装完服务端：架构识别、自签证书、BBR、防火墙；客户端带 WebRTC/IPv6/DNS 防泄露规则。
- :warning: **局限** — 需要一台自己的 Linux VPS；没有发布物和界面，纯脚本；可用性要按当地网络自测。
- :arrow_right: **入口** — [部署指南](https://github.com/cyancity/hy2-proxy-setup)

---

### 04 · 自用与配套

<sub>优先级最低，不占主推位</sub>

- **[kindle-gadget](https://github.com/cyancity/kindle-gadget)** <sub>Python · Shell · MIT</sub> — 把越狱 Kindle 当 agent 推送的墨水屏看板，一条命令推 HTML 或 PNG。<br>
  <sub>⚠️ 前提：先越狱；只在 Kindle Oasis 3 + 5.18.2 + Windows 上实测过。</sub>
- **[easy-unlocker-site](https://github.com/cyancity/easy-unlocker-site)** <sub>JavaScript</sub> — easy-unlocker 的官网。
- **[dycopy-public](https://github.com/cyancity/dycopy-public)** <sub>Python</sub> — dycopy skill 背后的源码，处理你有权访问的抖音内容。

<p align="center"><sub>Docs an agent can run end to end · verified and unverified stated plainly · secrets never in the chat</sub></p>
