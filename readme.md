# Komari Agent

## 安装

### Linux

默认安装 1.1.93：

```bash
wget -qO- https://raw.githubusercontent.com/Taylor000/komari-agent/refs/heads/main/install.sh | sudo bash -s -- -e YOUR_PANEL_URL -t YOUR_AGENT_TOKEN --disable-web-ssh --disable-auto-update --ignore-unsafe-cert
```

安装 1.2.0：

```bash
wget -qO- https://raw.githubusercontent.com/Taylor000/komari-agent/refs/heads/main/install.sh | sudo bash -s -- --install-version 1.2.0 -e YOUR_PANEL_URL -t YOUR_AGENT_TOKEN --disable-web-ssh --disable-auto-update --ignore-unsafe-cert
```

### Windows

请在管理员 PowerShell 中运行。

默认安装 1.1.93：

```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -Command "iwr 'https://raw.githubusercontent.com/Taylor000/komari-agent/refs/heads/main/install.ps1' -UseBasicParsing -OutFile 'install.ps1'; & '.\install.ps1' '-e' 'YOUR_PANEL_URL' '-t' 'YOUR_AGENT_TOKEN' '--disable-web-ssh' '--disable-auto-update' '--ignore-unsafe-cert'"
```

安装 1.2.0：

```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -Command "iwr 'https://raw.githubusercontent.com/Taylor000/komari-agent/refs/heads/main/install.ps1' -UseBasicParsing -OutFile 'install.ps1'; & '.\install.ps1' '--install-version' '1.2.0' '-e' 'YOUR_PANEL_URL' '-t' 'YOUR_AGENT_TOKEN' '--disable-web-ssh' '--disable-auto-update' '--ignore-unsafe-cert'"
```

请将 `YOUR_AGENT_TOKEN` 替换为实际 Token；不要将真实 Token 提交到公开仓库。

安装后强制关闭自动更新。所有 Agent 二进制均从本仓库 Release 下载并校验 SHA-256；Windows 所需的 NSSM 也已固定归档在本仓库。

本仓库不使用 GitHub Actions，也不会跟随上游更新。安装和运行时不依赖 `komari-monitor` 仓库。

版本参数也兼容简写：`1.93` 等同于 `1.1.93`，`1.20` 等同于 `1.2.0`。
