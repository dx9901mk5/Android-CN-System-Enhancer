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
| **YouTube 實機示範 / Demo Video** | https://youtube.com/shorts/1QtWvg_pKqc | CN陸版啟用仿捲動翻譯(Google驅動) / Enable Google-Powered Scroll Translate on CN ROM |

---

## 繁體中文說明

**Android 補強整合 CN（`Android_Enhancer_CN`）** 是一款專為陸版 Android 手機／平板（OriginOS、ColorOS、HyperOS 等）打造的**六分頁系統補強整合工具**。採用頂部文件資料夾樣式分頁與左右滑動切換，支援**繁體中文、簡體中文、英文、日文**四語系即時切換，並支援 App 內自動檢測更新與進度條直接下載安裝。

### ✨ 六大核心功能分頁

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

5. **Tab 5 — 穿透式捲動翻譯（仿 Google 捲動翻譯）〔Pro / Premium 專屬〕**
   - 🎬 **實機操作示範影片**：https://youtube.com/shorts/1QtWvg_pKqc
   - **免 Root・Google 翻譯＋ML Kit 視覺雙引擎驅動**：解決陸版 CN ROM 因唯讀系統屬性無法使用原生 Google 畫圈捲動翻譯的痛點。將翻譯文字直接原位覆蓋於原文座標正上方，手指可直接觸控穿透上下滑動網頁、社群、漫畫與 App，滑動停頓後自動即時重翻！啟動後懸浮膠囊支援「按住 `👁` 透視原文、切換來源／目標語系、手動重翻」，並支援控制中心快捷磁貼一鍵開關。
   - **獨立啟動器捷徑 App「仿G 捲動」**：提供一鍵產生名為 **「仿G 捲動」**（簡中：`仿G 滚动` / 英文：`G-Scroll`）的極小獨立啟動器 App，方便各家邊緣手勢 App、系統智慧側邊欄、自訂桌面啟動器於「啟動應用程式」清單中直接選取綁定；使用者可隨時單獨移除「仿G 捲動」（本體 App 自動偵測存在狀態），且移除本體 App 時亦會自動一併移除。
   - **方案與既有購買者權益**：開放 **專業 Pro（NT\$260）** 與 **頂級 Premium（NT\$380）** 用戶開通（進階 Plus 維持 NT\$120，加購升級擴充為 NT\$150）；**既有已購買 Pro 與 Premium 的用戶直接享有開通資格，不受價格調整影響**。

6. **Tab 6 — 免費工具箱（永久免費・專為 Vivo / iQOO 陸版 ROM 設計）＋ 推薦友情連結**
   - **雙擊電源鍵啟動相機（Vivo 陸版修復）**：透過 Shizuku 監聽電源鍵雙擊，支援任何時候／僅鎖屏息屏／僅解鎖後觸發，提供息屏雙擊音量下鍵與直呼安全相機雙模式。
   - **Vivo / iQOO 陸版導航語音修復（Google TTS）**：免接電腦，直接透過 Shizuku 一鍵修復 Vivo CN ROM 導航語音識別（標準直接修復／深度突破修復）。
   - **Shizuku 靜默安裝 APK**：選取手機內任意 `.apk` 安裝檔，透過 Shizuku 權限免點擊確認視窗直接靜默安裝（支援覆蓋、測試版與選配降級 `-d` 安裝）。
   - **開發者／USB 通知檢測與 Gmail 寄出 Log**：透過 Shizuku 讀取系統目前通知並產生診斷 `.txt` Log，可一鍵啟動 Gmail 並附上 Log 自選收件人寄出。
   - **陸版開啟 Google 地圖時間軸（640 dp 解法）**：透過 Shizuku 記憶原本 DPI 後切換為 `640 dp`、支援一鍵重開機、開啟時間軸後精準還原原本 DPI（含解除 GMS／地圖定位與省電限制）。
   - **Vivo 小螢幕模式自動關閉／恢復無障礙** ＆ **自動移除 Android 系統警示通知**（收到通知與每次點亮螢幕時 0s／1s／2s 三次連環清除）。
   - **精選陸版補強友情連結**：
     1. **Vivo 陸版 CN ROM 雙開通知修復**（飛雪連天／冷大）：https://github.com/Reeky-ux/VIVO_Notification_Fix
     2. **MiCTS（觸發 Google 翻譯／畫圈搜尋）**：https://github.com/parallelcc/MiCTS — 推薦安裝 `MiCTS.apk`（觸發畫圈搜尋翻譯）與 `VISTrigger.apk`（手動觸發 Gemini 圈選語音呼喚介面）
     3. **Bada（陸版手機 CN ROM 可接入國際版快速分享渠道）**：https://github.com/kyujin-cho/Bada — 讓陸版 CN ROM 選擇接入國際版 Android 鄰近分享傳輸（快速分享 Quick Share），雖尚無法接通 AirDrop，但可讓國際版與陸版 Android 手機互找、互傳。

### 🔄 近期版本更新摘要（`v0.1.0` → `v3.2.0`）

- **`v3.2.0`**：新增獨立 **Tab 5「穿透式捲動翻譯（仿 Google 捲動翻譯）」**（Pro／Premium 專屬，Google 翻譯＋ML Kit 雙引擎免 Root 觸控穿透原位翻譯，支援產生獨立啟動器捷徑 App **「仿G 捲動」** 供各家邊緣手勢與系統側邊欄選取，可單獨移除、移除本體亦自動一併移除）；原免費工具箱移至 **Tab 6** 並於底部補上三大精選陸版補強友情連結（`VIVO_Notification_Fix`、`MiCTS`、`Bada`）；同步調整方案價格（Plus 維持 NT\$120、Pro NT\$260、Premium NT\$380、加購升級 NT\$150，**既有已購買 Pro／Premium 用戶不受影響直接開通**），並完整校對繁體中文、簡體中文、英文、日文全介面語系一致性。

- **`v3.1.6`**：Tab 5「免費工具箱」新增兩項實用工具——① **Vivo 小螢幕模式自動關閉／恢復無障礙**（自動處理 `com.vivo.minscreen`「功能衝突」彈窗點擊關閉、進入小螢幕清空無障礙、退出 `minscreen_state_switch=0` 自動全數恢復）；② **自動移除 Android 系統警示通知**（仿照 MacroDroid 連環清除腳本，提供可打勾選擇的 App 清單如 FanRecentGesture／Edge 等，於收到通知與每次點亮螢幕時執行 0s／1s／2s 三次清除）。另移除 Tab 5 各卡片標題多餘的「（永久免費）」後綴，僅保留頁頂永久免費橫幅。
- **`v3.1.5`**：Tab 4 介面極簡化，將多餘子開關收斂為清楚說明內文（上方預設 `ADB=2`＋暫停無障礙、下方預設完整嚴格歸零＋關閉開發者與無障礙）；移除原本隱藏的「Vivo 雙開通知修復」區塊；更新「針對全家 APP」實測操作提示並將「立即手動還原 ADB 與開發者選項」移至 Tab 4 最下方。
- **`v3.1.4`**：修正 `isA11yStealthActive` 旗標殘留導致指定嚴格 App 未觸發隱藏的 Bug，並針對全家等於啟動 15ms 內檢查的嚴格 App 加入「套用隱藏後自動重啟一次」機制；補齊設定備份／還原涵蓋全部 5 個分頁（含 Tab 5 免費工具箱與無障礙守護），另為所有 App 選擇清單加上轉圈過度動畫與背景快取加速。
- **`v3.1.3`**：Tab 4 改為清晰的兩層式設計——上方「一般隱藏」支援隱藏 `ADB=2` ＋選配關閉無障礙（不動開發者選項與無線偵錯）；下方「嚴格／激進指定 App」整合關閉開發者選項與「激進歸零（`ADB=0`／`無線=0`）」選項，並修復同時啟用一般隱藏時進指定 App 跳過關閉開發者選項的 Bug。
- **`v3.1.2`**：Tab 4「一般隱藏」補回客製化目標 App 選擇選單（僅隱藏 ADB／開發者，不關閉無障礙）；下方「攔截指定 App 偵測開發者模式與無障礙」新增「若上方無效再使用」說明，並於選好後自動檢查上方清單移除重複 App、保留於下方。
- **`v3.1.1`**：Tab 4「針對指定 App 隱藏」新增獨立開關「進入指定 App 時一併關閉開發者選項（離開自動還原）」，並附上「建議全家／麥當勞等極嚴格 App 使用、原本方法無法通過再開啟」說明；另新增開機殘留狀態自動還原保護，確保重開機後開發者選項與無障礙不會卡在關閉狀態。
- **`v3.1.0`**：移除 Tab 4「嚴格 ADB 歸零（`adb_wifi_enabled = 0`）」選項並強制永久停用（統一採 `adb_enabled = 2` 偽裝，確保 Shizuku 與無線偵錯不失效）；「隱藏開發者選項」改為重安裝與每次重開機後預設關閉（且指定 App 隱藏亦遵循此開關）。
- **`v3.0.9`**：徹底修正「環境隱身」導致無法開啟無線偵錯及使 Shizuku 失效的問題：將「偵測 Shizuku 自動開啟環境隱身」與「嚴格 ADB 歸零（`adb_wifi_enabled = 0`）」改為預設關閉（改用 `adb_enabled = 2` 不砍無線偵錯）；在「設定」與「Shizuku」之間切換或經過桌面時提供 15 秒保護期且不於桌面重套隱身，確保正常配對與保持 Shizuku 連線。
- **`v3.0.8`**：修正 Tab 4「環境隱身」在各廠牌機型（全家／一般手機相容性）反覆觸發開發者模式開開關關提示的問題（修正鎖屏不再重複還原切換一般隱身、原始關閉狀態如實備份不再誤開、過濾系統暫時性視窗與 IME、新增系統反彈 60 秒冷卻保護）。
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

**Android CN System Enhancer (`Android_Enhancer_CN`)** is a **6-tab Android system enhancement suite** built for Chinese-ROM smartphones and tablets (OriginOS, ColorOS, HyperOS, etc.). It features top document-folder-style tabs with horizontal swipe navigation, 4-language live switching (`zh-TW`, `zh-CN`, `EN`, `JA`), and in-app update downloading with a bottom progress bar.

### ✨ Six Feature Tabs

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

5. **Tab 5 — Pass-Through Scroll Translate (`Google-Style Live Translate`・Pro / Premium Exclusive)**
   - 🎬 **Live Demo Video**: https://youtube.com/shorts/1QtWvg_pKqc
   - **Root-Free・Google Translate + ML Kit Vision OCR Dual Engine**: Overlays translated text directly over original screen coordinates while allowing touch gestures to pass straight through—automatically re-translating as you scroll! Includes a draggable floating control capsule (hold `👁` to peek original text, switch source/target languages, manual refresh) and a Control Center Quick Settings Tile.
   - **Standalone Launcher Shortcut App (`G-Scroll` / `仿G 捲動`)**: Generates a tiny standalone launcher app so any edge-gesture app, system smart sidebar, or custom launcher can bind it under "Launch Application". Users can uninstall it individually anytime (detected dynamically by the main app), and uninstalling the main app automatically removes it together.
   - **Licensing & Existing Buyers**: Unlocked for **Pro (NT\$260)** and **Premium (NT\$380)** users (Plus remains NT\$120; +1 Tier Upgrade Add-on is NT\$150). **Existing Pro and Premium buyers retain full entitlement automatically without price re-evaluation.**

6. **Tab 6 — Free Tools (`Permanently Free・Tailored for Vivo / iQOO CN ROM`) & Recommended Links**
   - **Double-Tap Power Key Camera (Vivo CN ROM Fix)**, **Vivo / iQOO CN Navigation Voice Fix (Google TTS)**, **Shizuku Silent APK Installer**, **Developer / USB Notification Diagnostics & Gmail Export**, **CN ROM Google Maps Timeline Unlock (640 dp Workaround)**, **Vivo Mini-Screen Mode Accessibility Guard**, and **Auto-Dismiss Android System Warning Notifications**.
   - **Recommended Companion Projects (Friend Links)**:
     1. **Vivo CN ROM Dual-App Notification Fix** (by Reeky-ux / 飛雪連天 冷大): https://github.com/Reeky-ux/VIVO_Notification_Fix
     2. **MiCTS (Trigger Circle to Search / Translate)**: https://github.com/parallelcc/MiCTS — Recommended APKs: `MiCTS.apk` (triggers Circle to Search translation) & `VISTrigger.apk` (manually triggers the Gemini voice/circle overlay)
     3. **Bada (Global Quick Share Channel for CN ROMs)**: https://github.com/kyujin-cho/Bada — Connects CN ROM Android phones to global Android Nearby Share / Quick Share channels (does not connect to AirDrop yet, but enables mutual discovery and file transfer between Global and CN Android phones).

### 🔄 Recent Changelog Summary (`v0.1.0` → `v3.2.0`)

- **`v3.2.0`**: Introduced dedicated **Tab 5 "Pass-Through Scroll Translate (Google-Style Live Translate)"** (exclusive to Pro & Premium users; Google-powered dual-engine in-place touch-pass-through translation + one-click generator for standalone **`G-Scroll` / `仿G 捲動`** launcher shortcut app for edge gestures & smart sidebars, individually removable and auto-removed with the host app); moved Free Tools to **Tab 6** and added three recommended CN ROM companion project links (`VIVO_Notification_Fix`, `MiCTS`, `Bada`); updated pricing (Plus unchanged at NT\$120, Pro NT\$260, Premium NT\$380, +1 Tier Add-on NT\$150 — **existing Pro & Premium buyers retain full access without re-judging**), with complete UI localization across Traditional Chinese, Simplified Chinese, English, and Japanese.

- **`v3.1.6`**: Added two new tools to Tab 5 (Free Tools): (1) **Vivo Mini-Screen Mode Accessibility Guard** (auto-snapshots Accessibility Services, clicks "關閉" on the `com.vivo.minscreen` conflict dialog, clears remaining services on `minscreen_state_switch=1`, and restores all on exit `0`), and (2) **Auto-Dismiss Android System Warning Notifications** (multi-select app picker with auto-selected FanRecent/Edge apps; clears matching system alerts on notification arrival and every screen-on event at 0s/1s/2s). Also removed redundant "(Permanently Free)" suffixes from individual Tab 5 card titles while keeping the top banner.
- **`v3.1.5`**: Simplified Tab 4 UI by consolidating sub-switches into clear inline descriptions (upper tier: `ADB=2` + pause Accessibility; lower tier: turn off Developer Options + zero ADB + pause Accessibility), removed the hidden Vivo Dual-App notification repair section, updated the FamilyMart tip (1st/odd launch detected -> swipe away & 2nd/even launch passes; add to lower strict list), and moved "Restore ADB & Dev Options Now" to the bottom of Tab 4.
- **`v3.1.4`**: Fixed stale `isA11yStealthActive` flag skipping strict per-app stealth, added one-shot auto-relaunch when hiding flags for apps that check `adb_enabled` within 15ms of launch (e.g., FamilyMart), expanded Settings Backup/Restore to cover all 5 tabs (including Tab 5 Free Tools & A11y Guard), and added a loading spinner + background cache for all app picker dialogs.
- **`v3.1.3`**: Reorganized Tab 4 into a clear two-tier stealth design: upper General Stealth supports `ADB=2` + optional per-app Accessibility pause (keeping Developer Options & Wireless Debugging intact), while the lower Strict/Aggressive section consolidates "Turn off Developer Options" and "Aggressive Mode (`ADB=0` / `Wireless=0`)" and fixes the condition bug when General Stealth was active.
- **`v3.1.2`**: Added a custom target app picker to Tab 4's upper General Stealth section (hides ADB/Dev only without turning off Accessibility), clarified the lower section is for apps where the upper stealth is ineffective, and automatically removes overlapping apps from the upper list when saved in the lower list.
- **`v3.1.1`**: Added an independent "Also turn off Developer Options when entering selected apps" toggle under Tab 4's per-app stealth section (with guidance for strict apps like FamilyMart & McDonald's when the default ADB=2 + Accessibility hide isn't enough), plus automatic boot-time state restoration if the device reboots while inside a hidden app.
- **`v3.1.0`**: Removed the user-facing "Strict ADB=0" toggle and permanently disabled `adb_wifi_enabled = 0` zeroing (always uses `adb_enabled = 2` so Shizuku stays alive); "Hide Developer Options" now defaults to OFF on fresh install, update, and every reboot (and per-app stealth also respects this flag).
- **`v3.0.9`**: Fixed Environment Stealth blocking Wireless Debugging setup and killing Shizuku: `auto_start_on_shizuku` and `strict_adb_zero` (`adb_wifi_enabled = 0`) now default to `false` (using `adb_enabled = 2` so Shizuku stays alive), and added Launcher skip + 15-second grace window when switching between Settings and Shizuku.
- **`v3.0.8`**: Fixed repeated "Developer Mode enabled/disabled" notification loops across OEM ROMs in Tab 4 (Environment Stealth): screen-off no longer toggles General Stealth off/on, original `0` developer state is backed up accurately without forcing `1`, transient system/IME windows are ignored, and a 60s bounce cooldown prevents retry loops.
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
