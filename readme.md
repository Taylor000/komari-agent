# Komari Agent

自用发行仓库，仅支持：

- `1.2.0`（默认）
- `1.1.93`

## 安装

默认安装 1.2.0：

```bash
curl -fsSL https://raw.githubusercontent.com/Taylor000/komari-agent/main/install.sh \
  | sudo bash -s -- -e https://你的面板地址 -t TOKEN
```

安装 1.1.93：

```bash
curl -fsSL https://raw.githubusercontent.com/Taylor000/komari-agent/main/install.sh \
  | sudo bash -s -- --install-version 1.1.93 -e https://你的面板地址 -t TOKEN
```

安装后默认关闭自动更新。所有二进制均从本仓库 Release 下载并校验 SHA-256。
