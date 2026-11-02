# TriadMind 桌面版发布产物

这个仓库**只放安装包与更新清单**，源码在私有仓库 `Jianfengwu2024/TriadMind`。

- `latest.json`：更新清单（版本 / 下载地址 / 签名），桌面版的「检查更新」就是读它。
- `*.exe` + `*.exe.sig`：Windows 安装包与签名。

客户端指向这里的方式（1.2.2 起支持，无需重新打包）：

```powershell
$env:TRIADMIND_UPDATE_ENDPOINT = "https://github.com/Jianfengwu2024/triadmind-releases/releases/latest/download/latest.json"
# 或写进 %APPDATA%\ai.triadmind.workbench\update-endpoint.txt 的第一行
```