# Komari Agent

自用发行仓库，仅支持：

- `1.1.93`（默认）
- `1.2.0`

## 安装

### Linux

默认安装 1.1.93：

```bash
curl -fsSL https://raw.githubusercontent.com/Taylor000/komari-agent/main/install.sh \
  | sudo bash -s -- -e https://你的面板地址 -t TOKEN
```

安装 1.2.0：

```bash
curl -fsSL https://raw.githubusercontent.com/Taylor000/komari-agent/main/install.sh \
  | sudo bash -s -- --install-version 1.2.0 -e https://你的面板地址 -t TOKEN
```

### Windows

请在管理员 PowerShell 中运行。

默认安装 1.1.93：

```powershell
& ([ScriptBlock]::Create((irm 'https://raw.githubusercontent.com/Taylor000/komari-agent/main/install.ps1'))) -e 'https://你的面板地址' -t 'TOKEN'
```

安装 1.2.0：

```powershell
& ([ScriptBlock]::Create((irm 'https://raw.githubusercontent.com/Taylor000/komari-agent/main/install.ps1'))) --install-version 1.2.0 -e 'https://你的面板地址' -t 'TOKEN'
```

安装后默认关闭自动更新。所有二进制均从本仓库 Release 下载并校验 SHA-256。
