<div align="center">

# YOLO

**I build tools that let AI agents do real work without being handed your secrets.**

Frontend and Node.js by background. Lately: credential approval for agents,<br>
multi-agent workbenches, and an e-ink screen that agents can write to.

</div>

<br>

## Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/cyancity/easy-unlocker"><b>easy-unlocker</b></a><br>
      <sub>Kotlin · Swift · Go · TypeScript</sub><br><br>
      Secrets management for AI agents. The agent asks for a key, you approve on your phone with a fingerprint, and the value arrives end-to-end encrypted in the one process that asked. The relay only sees ciphertext. Android and iOS apps, a desktop approver, a CLI, and a self-hosted broker.
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/cyancity/yolo-bot"><b>yolo-bot</b></a><br>
      <sub>TypeScript · React</sub><br><br>
      A digital-employee workbench plugin for DeepSeek Harness. You give a task in a channel; a lead agent breaks it down, assigns it to employees with their own models, skills and memory, and hands back versioned deliverables. Docs in Chinese.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/cyancity/kindle-gadget"><b>kindle-gadget</b></a><br>
      <sub>Python · Shell</sub><br><br>
      Turns a jailbroken Kindle into an always-on e-ink dashboard. Any agent writes HTML, the PC renders and dithers it, and one command puts it on the screen over SSH. Includes a resident daemon, boot-time autostart and a local web studio.
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/cyancity/hy2-proxy-setup"><b>hy2-proxy-setup</b></a><br>
      <sub>Shell · PowerShell</sub><br><br>
      A Hysteria 2 server install script (BBR, self-signed cert, systemd) plus client routing rules and a Windows DNS leak hardening script, written as a runbook an agent can execute on any Linux server. Docs in Chinese.
    </td>
  </tr>
</table>

## How I work

- **Write docs an agent can run.** The projects ship runbooks an agent can follow from install to verification: easy-unlocker's [AGENTS-SETUP.md](https://github.com/cyancity/easy-unlocker/blob/main/docs/AGENTS-SETUP.md), kindle-gadget's [setup guide](https://github.com/cyancity/kindle-gadget/blob/main/docs/opensource/SETUP.en.md), the hy2 install SOP.
- **Say what is verified.** kindle-gadget keeps verified, unverified and known-broken lists; easy-unlocker tracks feature parity across Android, iOS, desktop, CLI and broker in one table.
- **Keep secrets out of the chat.** Credentials never go into conversations, commits or logs. easy-unlocker exists because of that rule.

## Stack

TypeScript · React · Node.js · Go · Kotlin (Android) · Swift (iOS) · Python · Shell · Cloudflare Workers
