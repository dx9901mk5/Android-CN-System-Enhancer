# Android-CN-System-Enhancer（Android 補強整合 CN / Android_Enhancer_CN）

[繁體中文](#繁體中文說明) | [English](#english)

> **⚠️ 重要運行需求 / Important Requirement**：  
> 本 App **必須搭配 [Shizuku](https://shizuku.rikka.app/)** 運行（透過無線偵錯或 ADB 啟動），才能自動授予系統權限並啟用相簿守護、語音攔截與環境隱身等功能。  
> This app **requires [Shizuku](https://shizuku.rikka.app/)** (started via Wireless Debugging or ADB) to grant system permissions and power Photo Sync Guard, Voice Intercept, and Environment Stealth.

---

## 📦 下載與發布管道 / Download & Release Channel

| 管道 / Channel | 連結 / URL | 說明 / Notes |
| :--- | :--- | :--- |
| **GitHub Releases** | https://github.com/dx9901mk5/Android-CN-System-Enhancer/releases | 最新穩定版與完整發行說明 / Latest stable releases & release notes |

---

## 繁體中文說明

**Android 補強整合 CN（`Android_Enhancer_CN`）** 是一款專為陸版 Android 手機／平板（OriginOS、ColorOS、HyperOS 等）打造的**四合一系統補強整合工具**。採用頂部文件資料夾樣式分頁與左右滑動切換，支援**繁體中文、簡體中文、英文、日文**四語系即時切換，並支援 App 內自動檢測更新與進度條直接下載安裝。

### ✨ 四大核心功能分頁

1. **Tab 1 — 來電音樂（CallMusicGuard）**
   - 監聽 LINE、Telegram、Messenger 等通訊軟體來電通知，通話時自動暫停音樂，掛斷後自動恢復播放。
   - 支援自訂搜尋與勾選「監測的通訊軟體」與「控制的音樂播放軟體」（含 App 圖示）。

2. **Tab 2 — 相簿守護（PhotoSyncGuard）**
   - 開啟相機拍照或錄影期間，自動暫時限制 Google 相簿背景網路連線（支援 30–180 秒延遲恢復），避免相簿搶傳或傳送未算圖完成的照片。
   - 支援查看近期攔截紀錄與一鍵手動立即恢復網路。

3. **Tab 3 — 語音攔截（CnVoiceIntercept）**
   - 透過 Shizuku 底層 `events` 兩段式精準偵測陸版語音助理喚醒（如 vivo 藍心小V、OPPO 小布、小米小愛），瞬間終止原廠助理並直接喚起 **Google Gemini** 或自訂 AI App。

4. **Tab 4 — 環境隱身（ADB 與無障礙反偵測）**
   - **開機 Shizuku 檢測與通知**：開機後每 30 秒自動檢查 Shizuku 授權狀態，未就緒時顯示提示通知，確認取得 Shizuku 授權後立即自動移除通知（可設為偵測到 Shizuku 後自動啟動隱身）。
   - **反偵測 ADB 與無障礙隱藏**：進入一般 App 時自動隱藏 `adb_enabled`、`adb_wifi_enabled` 與 `development_settings_enabled`（預設自動排除本身需使用 Shizuku 的 App）；亦可自訂勾選需同時隱藏「開發者模式與無障礙」的目標 App（如行動支付／銀行／會員 App），離開 App 或關閉螢幕時自動還原。
   - **自動消除 vivo 開發模式通知**：自動清除系統因切換開發者模式所彈出的風險提醒通知。

5. **Tab 5 — 免費工具箱（永久免費・專為 Vivo / iQOO 陸版 ROM 設計 / Permanently Free・For Vivo CN ROM）**
   - **雙擊電源鍵啟動相機（Vivo 陸版修復）**：專為 Vivo / iQOO OriginOS 陸版無電源鍵雙擊快啟相機之系統限制打造，透過 Shizuku 監聽電源鍵雙擊，支援任何時候／僅鎖屏息屏／僅解鎖後觸發，提供息屏雙擊音量下鍵與直呼安全相機雙模式。
   - **Vivo / iQOO 陸版導航語音修復（Google TTS）**：免接電腦，直接透過 Shizuku 一鍵修復 Vivo CN ROM 導航語音識別（標準直接修復／深度突破修復）。
   - **Shizuku 靜默安裝 APK**：選取手機內任意 `.apk` 安裝檔，透過 Shizuku 權限免點擊確認視窗直接靜默安裝（支援覆蓋、測試版與選配降級 `-d` 安裝）。
   - **開發者／USB 通知檢測與 Gmail 寄出 Log**：透過 Shizuku 讀取系統目前通知並產生診斷 `.txt` Log（協助分辨不同品牌手機的開發者模式／USB 偵錯通知來源），可一鍵啟動 Gmail 並附上 Log 自選收件人寄出。
   - **陸版開啟 Google 地圖時間軸（640 dp 解法）**：透過 Shizuku 先記憶使用者原本 DPI 後切換為 `640 dp` 最小寬度、支援一鍵重開機、進入 Google 時間軸後一鍵精準還原原本 DPI（含解除 GMS／地圖背景定位與省電限制）。

### 🔄 近期版本更新摘要（`v0.1.0` → `v3.0.7`）

- **`v3.0.7`**：Tab 5「免費工具箱」新增 **陸版開啟 Google 地圖時間軸（640 dp 解法）**，支援自動記憶原本 DPI 後套用 `640 dp`、確認重開機、一鍵精準還原原本 DPI，以及解除 GMS／地圖背景定位與省電限制。
- **`v3.0.6`**：Tab 5「免費工具箱」新增 **開發者／USB 通知檢測與 Gmail 寄出 Log** 功能，透過 Shizuku 擷取不同品牌手機的系統通知資訊產生 Log 檔，並支援一鍵啟動 Gmail 附上 Log 自選收件人寄出。
- **`v3.0.5`**：Tab 5「免費工具箱」新增 **Shizuku 靜默安裝 APK** 功能，支援直接選取 `.apk` 串流靜默安裝（含允許降級 `-d` 開關）。
- **`v3.0.4`**：修正開機檢測通知在取得 Shizuku 授權後未移除的問題（輪詢每 30 秒主動呼叫 `ShizukuProvider.requestBinderForNonProviderProcess` 重新取得 Binder 並監聽授權結果，確認授權即自動撤除通知）。
- **`v3.0.3`**：Bug 修復與精簡更新檢查（移除雲端資料夾檢查，僅保留 GitHub Releases 更新）。
- **`v3.0.2`**：Tab 5 頂部橫幅改為固定顯示「永久免費（不佔用方案額度）」並隱藏付費按鈕；暫時隱藏「Vivo 雙開通知修復」選項，聚焦雙擊電源鍵相機與導航語音修復。
- **`v3.0.1`**：新增 **Tab 5「免費工具」分頁（永久免費）**，整合兩項專為 **Vivo / iQOO CN ROM** 打造的 Shizuku 免電腦修復功能。
- **`v2.3.5`**：設定備份的「匯出」與「匯入」新增 **Google 雲端硬碟 App** 選項，可直接呼叫手機 Google 雲端硬碟 App 選擇上傳位置或選取雲端 JSON 備份檔（保留本地檔案選項與系統 Fallback）。
- **`v2.3.4`**：Tab 3（語音攔截）最上方新增「預設數位語音助理」設定卡片與「選擇預設助理」按鈕，可一鍵跳轉系統預設數位助理應用程式設定（含四語系翻譯與設定頁 Fallback）。
- **`v2.3.3`**：移除測試版更新通道常數與本地測試資料夾，僅保留 GitHub 與正式版更新通道，並清理正式發布目錄僅保留最新正式版 APK。
- **`v2.3.2`**：修正已取得 Shizuku 授權後待機通知未移除的問題，改為每 30 秒定期檢查並於 `onDestroy` 確保撤除通知；設定內「無障礙／通知讀取／使用情況」授權按鈕點擊後自動高亮捲動至本 App 名稱附近；補齊中英文 `README` 與各發布頁面摘要。
- **`v2.3.1`**：於 `UnifiedNotificationListenerService` 加入自動偵測並消除 vivo／系統「開發模式風險提示」通知。
- **`v2.3.0`**：Tab 4 底部新增「針對全家 APP」設定與還原操作引導。
- **`v2.2.4`～`v2.2.7`**：補齊 `WRITE_SECURE_SETTINGS` 宣告與依序歸零（`adb_wifi_enabled` → `adb_enabled` → `development_settings_enabled`）；加入 `DeviceHardwareId` 記憶體快取與背景預熱，大幅縮短啟動耗時。
- **`v2.2.0`～`v2.2.3`**：完成繁中／簡中／英／日四語系全介面與動態文字翻譯、Google 帳號免序號查單還原、Gumroad 分級方案與 `+1` 分頁疊加授權。
- **`v2.0.0`～`v2.1.2`**：整合「環境隱身」至頂部文件資料夾分頁（支援左右滑動切換）、App 內底部進度條下載安裝、設定備份匯出／匯入與 Widevine 硬體指紋綁定。

---

## English

**Android CN System Enhancer (`Android_Enhancer_CN`)** is a **4-in-1 Android system enhancement suite** built for Chinese-ROM smartphones and tablets (OriginOS, ColorOS, HyperOS, etc.). It features top document-folder-style tabs with horizontal swipe navigation, 4-language live switching (`zh-TW`, `zh-CN`, `EN`, `JA`), and in-app update downloading with a bottom progress bar.

### ✨ Four Core Modules

1. **Tab 1 — Call Music Guard (`CallMusicGuard`)**
   - Automatically pauses music during incoming VoIP calls (LINE, Telegram, Messenger, etc.) and resumes playback after the call ends.
   - Searchable multi-select pickers with app icons for both monitored communication apps and target music players.

2. **Tab 2 — Photo Sync Guard (`PhotoSyncGuard`)**
   - Temporarily suspends Google Photos network access while the camera is active (configurable 30–180s delay) so raw/unprocessed photos are not uploaded prematurely.

3. **Tab 3 — Voice Intercept (`CnVoiceIntercept`)**
   - Uses two-stage Shizuku event correlation to intercept built-in Chinese voice assistants (vivo XiaoV, OPPO Breeno, Xiaomi XiaoAI) and launch **Google Gemini** or a custom AI app instead.

4. **Tab 4 — Environment Stealth (`ADB & Accessibility Stealth`)**
   - **Boot Shizuku Watchdog**: Checks Shizuku authorization every 30 seconds after boot, displays a reminder notification while waiting, and automatically dismisses it once Shizuku is ready (with optional auto-enable).
   - **Anti-ADB & Accessibility Hiding**: Hides `adb_enabled`, `adb_wifi_enabled`, and `development_settings_enabled` for regular apps while excluding Shizuku-dependent apps by default. Supports a custom app list to hide both Developer Options/ADB and Accessibility Services, restoring them automatically on exit or screen off.
   - **Auto-Dismiss System Dev Warnings**: Automatically clears repetitive vivo/system "Developer Mode active" warning notifications.

5. **Tab 5 — Free Tools (`Permanently Free・Tailored for Vivo / iQOO CN ROM`)**
   - **Double-Tap Power Key Camera (Vivo CN ROM Fix)**: Specifically built to restore double-tap power key camera launch on Vivo / iQOO OriginOS CN ROMs via Shizuku, supporting Always / Locked-only / Unlocked-only scopes and dual lockscreen modes.
   - **Vivo / iQOO CN Navigation Voice Fix (Google TTS)**: PC-free, Shizuku-driven one-tap repair specifically for Vivo CN ROMs (Standard direct mode & Deep Breakthrough mode).
   - **Shizuku Silent APK Installer**: Pick any `.apk` file on your device and install it silently via Shizuku without confirmation prompts (supports optional downgrade `-d` flag).
   - **Developer / USB Notification Diagnostics & Gmail Export**: Uses Shizuku to dump active system notifications into a `.txt` diagnostic log (identifying brand-specific Developer Mode / USB Debugging notification packages & channels) and launches Gmail with the log attached so users can choose a recipient.
   - **CN ROM Google Maps Timeline Unlock (640 dp Workaround)**: Uses Shizuku to save the user's original DPI before switching to `640 dp` smallest width, supports one-tap reboot, restores the exact saved original DPI afterward, and unlocks GMS/Maps background location & battery whitelist.

### 🔄 Recent Changelog Summary (`v0.1.0` → `v3.0.7`)

- **`v3.0.7`**: Added **CN ROM Google Maps Timeline Unlock (640 dp Workaround)** to Tab 5 (Free Tools), saving the user's original DPI before applying `640 dp`, offering reboot & exact DPI restoration, plus GMS/Maps location & battery-whitelist helpers.
- **`v3.0.6`**: Added **Developer / USB Notification Diagnostics & Gmail Log Export** to Tab 5 (Free Tools), using Shizuku to capture brand-specific system notification packages/channels into a `.txt` log and launch Gmail with the log attached.
- **`v3.0.5`**: Added **Shizuku Silent APK Installer** to Tab 5 (Free Tools), streaming selected `.apk` files directly to `pm install` via Shizuku with optional downgrade (`-d`) support.
- **`v3.0.4`**: Fixed Shizuku boot-watch notification not clearing after authorization (polls every 30s and actively refreshes Shizuku binder via `ShizukuProvider.requestBinderForNonProviderProcess`).
- **`v3.0.3`**: Bug fixes and streamlined update checker (GitHub Releases only).
- **`v3.0.2`**: Tab 5 top banner now displays "Permanently Free" with no paid prompt, and hides the Vivo Dual-App notification repair option.
- **`v3.0.1`**: Added **Tab 5 "Free Tools" (permanently free)**, integrating two Shizuku-powered fixes tailored for **Vivo / iQOO CN ROM**.
- **`v2.3.5`**: Added **Google Drive App** integration to Settings Backup Export & Import, allowing users to pick an upload folder or select a JSON backup directly via the Google Drive app (alongside Local storage and system fallbacks).
- **`v2.3.4`**: Added a "Default Digital Assistant" card and "Select Default Assistant" shortcut at the top of Tab 3 (Voice Intercept) to open the system default assistant settings directly (with 4-language translations and settings fallbacks).
- **`v2.3.3`**: Removed beta update channel references and local testing folder; streamlined releases to keep only the latest official APK alongside GitHub updates.
- **`v2.3.2`**: Fixed Shizuku boot notification remaining after authorization (polls every 30s and clears foreground notification in `onDestroy`); system permission buttons in Settings now highlight & auto-scroll directly to this app; added bilingual EN/ZH documentation and release summaries.
- **`v2.3.1`**: Added automatic dismissal/snoozing of vivo/system "Developer Mode risk warning" notifications in `UnifiedNotificationListenerService`.
- **`v2.3.0`**: Added FamilyMart app stealth setup guide at the bottom of Tab 4.
- **`v2.2.4`–`v2.2.7`**: Declared `WRITE_SECURE_SETTINGS` in `AndroidManifest.xml`, implemented strict zeroing (`adb_wifi_enabled` → `adb_enabled` → `development_settings_enabled`), and cached Widevine `MediaDrm` IDs asynchronously to eliminate startup lag.
- **`v2.2.0`–`v2.2.3`**: Full 4-language localization (`zh-TW` / `zh-CN` / `EN` / `JA`), Google account order lookup & license restore, and Gumroad tiered licensing with `+1` tab slot stacking.
- **`v2.0.0`–`v2.1.2`**: Top folder-style swipeable tabs, in-app APK download progress bar, JSON settings backup/restore, and Widevine hardware fingerprint binding.
