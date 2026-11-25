<h1 align="center">紅果短劇 · 繁體桌面版</h1>

<p align="center">在 Windows 電腦上找劇、接著看、下載與合併。介面預設繁體。</p>

<p align="center">
  <img alt="目前正式版 4.9" src="https://img.shields.io/badge/正式版-4.9-8b3a3a?style=flat-square">
  <img alt="說明與介面使用繁體中文" src="https://img.shields.io/badge/文案-繁體中文-555555?style=flat-square">
  <img alt="Windows x64 安裝版" src="https://img.shields.io/badge/Windows-x64-55746b?style=flat-square">
  <img alt="GPL-3.0 授權" src="https://img.shields.io/badge/license-GPL--3.0-555555?style=flat-square">
</p>

這個倉庫只放 **Windows x64** 安裝檔與本說明。這是社群維護的開源修改版，**不是紅果、西飯或河馬的官方用戶端**。不提供付費分集解鎖。劇集、清晰度與可播放範圍取決於來源平臺。

## 系統需求

- Windows 10 或 11，64 位元
- 不必另外安裝 Node.js 或 FFmpeg；媒體工具已內建
- 安裝版支援應用內更新；便攜版需手動換成新檔

## 下載與安裝

**安裝版（建議）**：[hongguo-downloader-4.9-win-x64-setup.exe](https://github.com/Tanney-for/drama-hub-win/releases/download/v4.9/hongguo-downloader-4.9-win-x64-setup.exe)

依畫面安裝。預設目錄是 `C:\hongguo`，安裝時可以改。完成後從桌面或開始功能表的「紅果短劇」捷徑啟動。

**便攜版**：[hongguo-downloader-4.9-win-x64.zip](https://github.com/Tanney-for/drama-hub-win/releases/download/v4.9/hongguo-downloader-4.9-win-x64.zip)

解壓後直接執行裡面的程式，不必安裝。便攜版**不能**用應用內更新；要換新版時，先退出舊程式，再解壓新的 ZIP 並執行新檔。若之後改走安裝版，請先退出便攜版，再執行 Setup，並從安裝程式建立的捷徑啟動。

- 安裝檔未簽章。請只從本倉庫的 [4.9 正式版](https://github.com/Tanney-for/drama-hub-win/releases/tag/v4.9) 下載，並對照該頁的 SHA256。
- 先退出正在執行的舊程式再安裝。設定、觀看紀錄與已下載的影片會留在原來的資料目錄。
- 下載與安裝都要自己確認。

## 應用內更新

安裝版會檢查本倉庫標為最新的正式版。先讀 GitHub 的最新發行，讀不到時再讀發行頁的轉向。本倉庫暫時連不上時，會改查舊的公開發行倉庫。預發佈不會提示。

出現新版本時，先由你決定是否下載；下載完成後，再決定何時重啟安裝。關閉提醒可繼續使用目前版本。便攜版請回到本頁手動下載。

## 核對 SHA256

發行頁會列出安裝檔與便攜 ZIP 的 SHA256。下載後請自己核對，確認檔案沒有被改過。

在 PowerShell：

```powershell
Get-FileHash -Algorithm SHA256 .\hongguo-downloader-4.9-win-x64-setup.exe
```

把顯示的雜湊值（不分大小寫）對照發行頁上的 SHA256。不一致就不要執行，改從本倉庫重新下載。

## 常見問題

### 為什麼 Windows 說「已保護你的電腦」，或出現 SmartScreen 警告？

安裝檔未簽章。若你是從本倉庫的 4.9 正式版下載，並已對照 SHA256，可在警告畫面選擇「其他資訊」，再選「仍要執行」。這不能代替核對雜湊值。

### 影片與設定放在哪裡？

影片在設定裡的下載目錄。設定、任務與觀看紀錄在 Windows 上預設位於 `%APPDATA%\hongguo-downloader\`。安裝版重裝同一版本時，這些資料會保留。

### 裝了新版，為什麼還是舊版本？

先退出所有正在執行的紅果短劇，再執行新的安裝檔，並從安裝程式建立的捷徑啟動。設定頁顯示的版本號才是目前執行的版本。

### 為什麼有些分集鎖定，或清晰度不一樣？

片源由來源服務決定。鎖定集保持鎖定，這個程式不提供解鎖。在線播放看實際畫面。不保證每一集都有相同的清晰度。

## 4.9 更新摘要

- 河馬新增分類：真人劇／漫劇／仿真人動漫
- 河馬新增排行榜與 20 個熱門題材標籤
- 河馬切集更快，載入提示更清楚
- 優化海報讀取，首頁海報更快更穩
- 紅果「搶先上線日」更名為「預告新劇」
- 河馬四榜每頁與紅果一致並加名次角標
- 紅果金銀銅名次
- 河馬彈幕自動預取
- 開著防護軟體時海報與榜單載入大幅加快
- 紅果在線播放改走新介面

4.9 正式版，內部版本 4.9.0，發行標籤 `v4.9`。畫質設定維持不變。本程式以 GPL-3.0 授權；安裝檔裡沒有劇集影片。
