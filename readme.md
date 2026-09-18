# Komari Agent 1.1.93 / 1.2.0

## 安装

### Linux

默认安装 `1.1.93`：

```bash
wget -qO- https://raw.githubusercontent.com/Taylor000/komari-agent/refs/heads/main/install.sh | sudo bash -s -- -e YOUR_PANEL_URL -t YOUR_AGENT_TOKEN --disable-web-ssh --disable-auto-update --ignore-unsafe-cert
```

安装 `1.2.0`：

```bash
wget -qO- https://raw.githubusercontent.com/Taylor000/komari-agent/refs/heads/main/install.sh | sudo bash -s -- --install-version 1.2.0 -e YOUR_PANEL_URL -t YOUR_AGENT_TOKEN --disable-web-ssh --disable-auto-update --ignore-unsafe-cert
```

也可运行 `tool`，选择 `16. Komari Agent`。

### Windows

管理员 PowerShell，默认安装 `1.1.93`：

```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -Command "iwr 'https://raw.githubusercontent.com/Taylor000/komari-agent/refs/heads/main/install.ps1' -UseBasicParsing -OutFile 'install.ps1'; & '.\install.ps1' '-e' 'YOUR_PANEL_URL' '-t' 'YOUR_AGENT_TOKEN' '--disable-web-ssh' '--disable-auto-update' '--ignore-unsafe-cert'"
```

安装 `1.2.0`：

```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -Command "iwr 'https://raw.githubusercontent.com/Taylor000/komari-agent/refs/heads/main/install.ps1' -UseBasicParsing -OutFile 'install.ps1'; & '.\install.ps1' '--install-version' '1.2.0' '-e' 'YOUR_PANEL_URL' '-t' 'YOUR_AGENT_TOKEN' '--disable-web-ssh' '--disable-auto-update' '--ignore-unsafe-cert'"
```
