# Allymote — 安裝檔下載

用 iPhone 看和操作電腦上 [herdr](https://herdr.dev) 裡的 AI agent（Claude Code、Codex），只走你自己的網路（Tailscale 或 SSH）。

這裡只放安裝檔。最快的做法是一行指令，它會自己下載你電腦的那一個、解壓縮、執行安裝程式：

```sh
# Mac（終端機）
curl -fsSL https://github.com/aeronan/allymote-releases/releases/latest/download/install.sh | sh
```

```powershell
# Windows（PowerShell）
irm https://github.com/aeronan/allymote-releases/releases/latest/download/install.ps1 | iex
```

或者自己下載你電腦的那一個（永遠是最新版，不用登入）：


- Apple 晶片的 Mac（M1 以後）：<https://github.com/aeronan/allymote-releases/releases/latest/download/allymote-macos-arm64.zip>
- Intel Mac：<https://github.com/aeronan/allymote-releases/releases/latest/download/allymote-macos-x64.zip>
- Windows：<https://github.com/aeronan/allymote-releases/releases/latest/download/allymote-windows-x64.zip>

裡面已經帶好 Node.js，不用另外安裝。解壓縮後照裡面的 `README.txt` 安裝：

- **Mac**：打開「終端機」，輸入 `sh `，把 `Install-Mac.command` 拖進視窗，按 Enter。
- **Windows**：右鍵「全部解壓縮」，再雙擊 `Install-Windows.cmd`。

需要先裝好：herdr。要用 Tailscale 連線的話，電腦和 iPhone 登入同一個 Tailscale 帳號。

裝好之後會自動更新。[Releases](https://github.com/aeronan/allymote-releases/releases) 頁上檔名裡有版本號的 `allymote-<版本>-…` 和 `latest.json` 是給已安裝的電腦自動更新用的，內容和上面三個相同。想馬上更新，在電腦上執行 `allymote update`。
