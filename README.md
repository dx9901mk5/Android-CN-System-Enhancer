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
   - **免 Root・Google 翻譯全球百餘語系自動偵測＋ML Kit 視覺雙引擎驅動（翻譯速度與台版原生 Google 捲動翻譯相等）**：不僅適用於陸版 CN ROM 手機，**亦支援「國際版／台版但系統無內建捲動翻譯功能」的所有 Android 手機使用**！可像 Google 翻譯一樣自動判斷全球所有可用語言（英、日、韓、歐語、泰、越、俄、阿、印、簡繁等），將譯文直接原位覆蓋於原文座標正上方，手指可直接觸控穿透上下滑動並於停頓後自動即時重翻；開啟後持續鎖定翻譯、點擊螢幕絕不取消，僅透過懸浮膠囊右側 `✕` 按鈕或 App 本體開關關閉。
   - **獨立啟動器捷徑 App「仿G 捲動」**：提供一鍵產生名為 **「仿G 捲動」**（簡中：`仿G 滚动` / 英文：`G-Scroll`）的極小獨立啟動器 App，方便各家邊緣手勢 App、系統智慧側邊欄、自訂桌面啟動器於「啟動應用程式」清單中直接選取綁定；使用者可隨時單獨移除「仿G 捲動」（本體 App 自動偵測存在狀態），且移除本體 App 時亦會自動一併移除。
   - **方案與既有購買者權益**：開放 **專業 Pro（NT\$260）** 與 **頂級 Premium（NT\$380）** 用戶開通（進階 Plus 維持 NT\$120，加購升級擴充為 NT\$150）；**既有已購買 Pro 與 Premium 的用戶直接享有開通資格，不受價格調整影響**。

6. **Tab 6 — 免費工具箱（永久免費・專為 Vivo / iQOO 陸版 ROM 設計）＋ 推薦友情連結**
   - **雙擊電源鍵啟動相機（Vivo 陸版修復）**：透過 Shizuku 監聽電源鍵雙擊，支援任何時候／僅鎖屏息屏／僅解鎖後觸發，提供息屏雙擊音量下鍵與直呼安全相機雙模式。
   - **Vivo / iQOO 陸版導航語音修復（Google TTS）**：免接電腦，直接透過 Shizuku 一鍵修復 Vivo CN ROM 導航語音識別（標準直接修復／深度突破修復）。
   - **Shizuku 靜默安裝 APK**：選取手機內任意 `.apk` 安裝檔，透過 Shizuku 權限免點擊確認視窗直接靜默安裝（支援覆蓋、測試版、選配降級 `-d` 與**宣告安裝來源為 Google Play 商店 `-i com.android.vending`，適用 Android Auto**）。
   - **開發者／USB 通知檢測與 Gmail 寄出 Log**：透過 Shizuku 讀取系統目前通知並產生診斷 `.txt` Log，可一鍵啟動 Gmail 並附上 Log 自選收件人寄出。
   - **陸版開啟 Google 地圖時間軸（640 dp 解法）**：透過 Shizuku 記憶原本 DPI 後切換為 `640 dp`、支援一鍵重開機、開啟時間軸後精準還原原本 DPI（含解除 GMS／地圖定位與省電限制）。
   - **Vivo 小螢幕模式自動關閉／恢復無障礙** ＆ **自動移除 Android 系統警示通知**（收到通知與每次點亮螢幕時 0s／1s／2s 三次連環清除）。
   - **精選陸版補強友情連結**：
     1. **Vivo 陸版 CN ROM 雙開通知修復**（飛雪連天／冷大）：https://github.com/Reeky-ux/VIVO_Notification_Fix
     2. **MiCTS（觸發 Google 翻譯／畫圈搜尋）**：https://github.com/parallelcc/MiCTS — 推薦安裝 `MiCTS.apk`（觸發畫圈搜尋翻譯）與 `VISTrigger.apk`（手動觸發 Gemini 圈選語音呼喚介面）
     3. **Bada（陸版手機 CN ROM 可接入國際版快速分享渠道）**：https://github.com/kyujin-cho/Bada — 讓陸版 CN ROM 選擇接入國際版 Android 鄰近分享傳輸（快速分享 Quick Share），雖尚無法接通 AirDrop，但可讓國際版與陸版 Android 手機互找、互傳。

### 🔄 近期版本更新摘要（`v0.1.0` → `v3.5.1`）

- **`v3.5.1`**：**對比 Google 原廠捲動翻譯全面修復穿透式翻譯閃爍、板位字級排版、圖片文字翻譯，並新增極速畫圈連動開關**：
  - **零閃爍視窗直截與輪播廣告過濾**：Android 14+ 改採 `takeScreenshotOfWindow` 僅擷取底層 App 視窗（無須隱藏譯文畫布與底部控制條，實現 `0ms` 零閃爍並根除半中半英殘影）；同時攔截非觸控期間的背景橫幅廣告自動輪播事件，靜止閱讀不再跳掉重刷。
  - **對應頁面板位字級與段落排版**：依原文「單行像素字高」1:1 對應字級（支援 `6.5sp` 圖片微縮字至 `34sp` 粗體大標題，解決內文過大、標題過小及標副標誤黏問題），多行段落貼齊原文左上邊界。
  - **強化圖片與內嵌螢幕截圖翻譯**：提升 OCR 原生解析度至 `2460px`、調優微小文字門檻並加入 ML Kit Latin 雙引擎補盲，單頁上限提升至 `90` 筆，完整翻譯縮圖與內嵌手機截圖小字。
  - **新增極速畫圈「連動捲動翻譯」開關與穩定度修復**：於 Tab 6 極速畫圈卡片底部新增連動開關，並加入 Google 畫圈掛載自動置頂 Z-order 與雙保險偵測，解決冷啟動時圓鈕偶發未跳出的問題（同步更新四語系操作說明）。

- **`v3.5.0`**：**⚙ 設定頁新增「功能與操作說明」按鈕與四語系內建說明**：
  - 於右上角 **⚙ 設定** 視窗新增「功能與操作說明」按鈕（點擊後才展開完整可捲動視窗），涵蓋 Tab 1–6 各分頁操作重點、Tab 5 穿透式捲動翻譯用法，以及 Tab 5 × Tab 6 極速畫圈搜尋連動與長壓拖動／跟隨 Google Bar／摺疊機雙螢幕記憶說明。
  - 完整支援繁體中文、簡體中文、英文、日文四語系即時切換顯示。

- **`v3.4.9`**：**修復極速畫圈啟動變慢、穿透式小按鈕無法正常點擊／跳出太慢，以及退出畫圈後按鈕殘留問題**：
  - **恢復極速秒開且不回首頁**：保留無頭 `FastCircleTriggerProvider`（零雙跳、無 `singleInstance` 與空 `taskAffinity`），同時讓單一透明視窗維持短暫存活（`260ms` 或偵測畫圈取得焦點後 `45ms` 即收尾，`circlestub` 升級 `v1.2.0`），徹底消除 `AssistStructure` 3 秒逾時卡頓。
  - **徹底解除主執行緒阻塞與修復按鈕點按**：將 Google 畫圈視窗與介面 Bar 偵測全部移至背景執行緒（`a11yInspectExecutor`），並將長壓拖曳門檻調至 `420ms`、放寬短按點擊容許範圍且偵測畫圈視窗一就緒即於最上層彈出，恢復秒跳出與高靈敏單點。
  - **退出極速畫圈按鈕自動立即消失**：背景監控同步偵測 Google 畫圈視窗／焦點是否存在，一旦使用者未點擊按鈕而退出畫圈搜尋，於 ~`0.25 秒` 內自動清除按鈕不再殘留於畫面。

- **`v3.4.8`**：**徹底修復極速畫圈截圖後強制回到首頁的問題**：
  - 根因修復：移除 `FastCircleSearchActivity` 與獨立捷徑 `circlestub` 的 `launchMode="singleInstance"`、`taskAffinity=""` 以及截圖後 220ms 才 `finish()` 的延遲（該延遲會導致任務在截圖完成瞬間銷毀並把系統切回桌面首頁）；全面對齊 MiCTS 生命週期於 `onCreate()` 同步即時結束。
  - 消除雙重 Activity 跳轉：新增無頭 `FastCircleTriggerProvider`，獨立捷徑「極速畫圈」（升級至 `v1.1.0`）改以同步呼叫主程式直接喚起畫圈搜尋、完全不建立第二個透明視窗與任務，並支援於開啟主程式／更新後透過 Shizuku 自動靜默升級舊版「極速畫圈」捷徑。

- **`v3.4.7`**：**極速畫圈穿透式翻譯啟動鈕支援長壓微調拖動、跟隨 Google 畫圈介面 Bar 上下挪動、摺疊機內外螢幕各自記憶位置**：
  - **長壓微調位置**：極速畫圈叫出穿透式翻譯圓形啟動鈕後，短按照常切入穿透式翻譯，**長按約 0.3 秒**（震動回饋＋橘框放大提示）即可自由拖動微調按鈕位置並記憶；
  - **跟隨 Google 畫圈介面 Bar 上下挪動**：按鈕顯示期間即時偵測 Google 畫圈搜尋介面 Bar 的垂直高度變化（如圈選下方物件、展開翻譯列或上下拉動結果列），自動平滑同步上下移動維持相對對齊；
  - **摺疊機內／外螢幕獨立記憶位置**：依據即時顯示器寬度自動區分摺疊機內螢幕（展開）與外螢幕（折疊）以及直／橫向，分別獨立保存並於切換螢幕時即時套用穿透式啟動鈕與穿透式翻譯控制條的位置設定。

- **`v3.4.6`**：**設定備份支援直接選擇「本地」或「Google 雲端硬碟」指定路徑並自動記憶下次位置**：
  - 匯出備份視窗直接提供 **「本地備份」** 與 **「Google 雲端硬碟備份」**（皆附「變更路徑」按鈕，並保留雲端硬碟 App 分享備援）；
  - **本地備份**首次透過系統資料夾授權（`ACTION_OPEN_DOCUMENT_TREE`）指定並記憶資料夾後，下次點擊即可一鍵直接存入該資料夾；
  - **Google 雲端硬碟備份**透過 SAF 指定雲端硬碟路徑並採背景串流寫入（防 0 位元組空檔），自動記住雲端硬碟位置供下次備份與還原直接開啟同一資料夾；設定對話框與還原選單亦會同步顯示已記憶路徑。

- **`v3.4.5`**：**關螢幕時自動取消極速畫圈搜尋**：偵測到 `ACTION_SCREEN_OFF`（鎖屏／關閉螢幕）時立即移除右下角接手圓鈕，並自動關閉進行中的 Google 畫圈搜尋浮層（優先透過 `hideSessionFromSession(null)`／`hideCurrentSession()` 關閉語音互動工作階段，並具備無障礙返回／Shizuku 備援，且未開啟無障礙服務時亦能透過獨立廣播監聽觸發），避免重新解鎖後仍殘留畫圈搜尋畫面。

- **`v3.4.4`**：**穿透式翻譯靜止 2.5 秒最終補驗＋休眠等待下次觸控滑動**：無觸控／滑動滿 `2.5 秒` 時自動再判斷翻譯最後一次，隨後進入靜默鎖定（不再受背景廣告或計時器干擾重翻），直到下次手指觸控或滑動再立即喚醒翻譯。

- **`v3.4.3`**：**穿透式翻譯永不自行暫停（僅於手動關閉或鎖屏時停止）**：移除原本進入本體 App 或橫向／大螢幕重繪時自動切換回「待命」暫停的限制，並強化橫向旋轉後的自動重譯排程，確保無論在任何 App、直向或橫向大螢幕皆全程保持「啟動」持續翻譯，直到使用者手動點擊 `✕` 關閉。

- **`v3.4.2`**：**徹底修復穿透式翻譯「譯文閃一下又消失變待命」與「慣性滑動停穩後不翻譯」問題**：① 過濾本體 `TYPE_ACCESSIBILITY_OVERLAY` 懸浮窗觸發的 `TYPE_WINDOW_STATE_CHANGED` 自殺式清空事件，並改以 `TYPE_APPLICATION` 視窗判斷是否進入本體 App，解決譯文顯示 1 秒後被自身懸浮窗誤判清空退回「待命」的問題；② 升級觸控與慣性滑動定點補驗機制（`finalSettleVerifyRunnable`＋過濾 `1..2px` 微幅減速雜訊），避免手指提前離開過早判定，確保畫面完全停穩後必定完成翻譯。

- **`v3.4.1`**：① **關閉螢幕自動關閉穿透式翻譯**：鎖屏／關閉螢幕時自動停止穿透式捲動翻譯並移除浮動視窗，省電且避免解鎖誤觸；② **極速畫圈觸發瞬間鎖定原 App／啟動器狀態並交接給穿透式翻譯**：於極速畫圈啟動當下立即快照記錄原所在 App 或啟動器，切換穿透式翻譯時精準依該狀態決定進多工切回原 App 或維持首頁。

- **`v3.4.0`**：**強化穿透式翻譯「進多工選最近 App」返回機制**：若非於啟動器首頁觸發且啟動後掉回桌面，自動喚起系統多工畫面並點擊最近使用的 App 卡片回到原頁面；若啟動時原本就在啟動器首頁，則維持於首頁不進入多工程序。

- **`v3.3.9`**：① **穿透式翻譯改用多工任務切換回到剛使用的 App**：於啟動器狀態啟動時維持在啟動器；若啟動前在一般 App 內而啟動後誤掉回桌面，改以 Shizuku `moveTaskToFront`（或無障礙多工切換備援）直接切回原 App 的既有任務與畫面，不再重新開啟 App 首頁；② **穿透式翻譯控制條支援全條任意位置拖曳**：按住控制條任一處拖動即可移動並記憶位置，單點各按鈕仍維持原本功能。

- **`v3.3.8`**：① **穿透式翻譯啟動首頁防護**：啟動時立即記錄原本所在 App 與是否已在首頁；若啟動後誤掉回桌面首頁，立即自動跳回原 App 頁面繼續翻譯（若啟動前原本就在首頁則維持首頁狀態）；② **左右滑動與觸控暫停／放手即譯**：新增全螢幕無干擾觸控監測與 `scrollX` 水平捲動偵測，觸控或滑動期間暫停翻譯，停止觸控後立即進入翻譯，支援上下與左右滑動換頁。

- **`v3.3.7`**：① **防誤觸底部系統手勢回首頁**：`FastCircleHandoffOverlay` 與穿透式捲動翻譯控制條自動避開底部手勢導覽區並加上 `systemGestureExclusionRects` 防誤觸保護，避免在底部切換或操作時誤觸系統「回到首頁」；② **穿透式翻譯取消白框・改為沉浸式背景融合**：移除譯文框外圍邊框線條，並強化截圖週邊主色取樣與快取，讓譯文背景與原本畫面無縫融合、維持一致排版。

- **`v3.3.6`**：**Tab 6 新增「輸入法系統顯示／隱藏與預設管理」**：列出手機所有已安裝輸入法（含圖示與狀態），支援透過 Shizuku 切換各輸入法在系統中的顯示（啟用）／隱藏（停用），並提供一鍵設定預設輸入法按鈕。

- **`v3.3.5`**：**大螢幕／橫向自適應雙欄並排排版**：於手機橫向、摺疊機內螢幕展開、8 吋／10 吋平板橫向與 Pixelbook 狀態下，各分頁功能卡片自動改為左右雙欄並排顯示（直向手機維持單欄直排）。

- **`v3.3.4`**：① **極速畫圈浮動接手按鈕改為右下角小圓形捲動翻譯圖示鈕**（對齊 Google 原廠捲動翻譯圖示樣式，固定於右下角不遮擋畫面）；② **Tab 5 穿透式捲動翻譯控制條預設改至螢幕底部置中**（比照 Google 原廠畫圈翻譯底部膠囊位置，仍支援自由拖曳記憶）。

- **`v3.3.3`**：**修復極速畫圈啟動時退出到首頁的問題**：移除會切換前景 Task 並自動結束回桌面的 `AssistantHandoffActivity` 跳轉，改由透明隔離視窗（`taskAffinity=""`＋`singleInstance`）直接於當前 App 畫面上觸發 `VisTrigger.triggerCircleToSearch`，完整保留當下頁面供畫圈搜尋與穿透式翻譯接手（註：若已安裝獨立捷徑「極速畫圈」建議重新安裝一次以套用 `singleInstance` 清單更新）。
- **`v3.3.2`**：**極速畫圈啟動後新增「🌐 切換穿透式翻譯」浮動接手按鈕**（僅於本體 App 已開通穿透式翻譯付費權限時顯示）：點擊按鈕將自動關閉 Google 畫圈搜尋並立即由穿透式捲動翻譯接手現有畫面，無須回到桌面切換。
- **`v3.3.1`**：① 移除 Tab 6「Google 畫圈搜尋 / MiCTS 防凍結加速」卡片；② 修正 Tab 6 方案 B「極速畫圈搜尋」改用 `VisTrigger.triggerCircleToSearch`（對齊 MiCTS 的 `omni.entry_point = 1`、`invocation_time_ms`、`micts_trigger` 參數），觸發後直接進入 Google 畫圈搜尋／翻譯介面而非一般語音助理浮層。
- **`v3.3.0`**：**Tab 6「Shizuku 靜默安裝 APK」新增「宣告安裝來源為 Google Play 商店 (`-i com.android.vending`)」開關**：開啟後透過 Shizuku 靜默安裝 `.apk` 時將一併傳入 `-i com.android.vending`，讓系統與 Android Auto 判定為 Google Play 商店安裝來源（例如安裝 `AATube-Caster` 等車機相關 App）。
- **`v3.2.9`**：① **Tab 6 新增方案 B「極速畫圈搜尋（預熱防延遲版）」捷徑／磁貼／獨立啟動器 App「極速畫圈」**：先於背景 90ms 預熱 `AssistantHandoffActivity` 再呼叫 `VisTrigger`，徹底繞過 Vivo OriginOS 3 秒冷交接卡頓；可一鍵產生獨立啟動器 App「極速畫圈」供各家手勢「指定應用程式啟動」選取，本體動態偵測安裝狀態且移除本體時一併自動移除（覆蓋更新不影響）；② **修復 GitHub API 403 限流導致 App 無法檢查更新**：新增 `github.com/.../releases/latest` 網頁跳轉直連備援；③ **APK 體積瘦身**：鎖定 `arm64-v8a` 大幅縮減下載時間。
- **`v3.2.8`**：**Tab 5 新增「預載加速語言包」勾選下載與最新版本檢查**：可自由勾選預先下載常用語系（中、英、日、韓、泰、越、法、德、西、俄等 15 語）本機 ML Kit 神經翻譯包與 GMS 視覺 OCR 模組；已下載的語系組合於捲動翻譯時優先走本機 ~20ms 極速翻譯（免等網路延遲），並支援一鍵向 Google 檢查更新至最新版。
- **`v3.2.7`**：**App 覆蓋更新與啟動時全量自動回傳試算表登記**：無論是 `CN2M-` / `CN3M-` / `CNPRO-` 或 `CNFAM-` / `CNVIP` 等所有已兌換序號，於 App 覆蓋更新（`MY_PACKAGE_REPLACED`）或啟動時皆自動將「兌換碼、已登記 Google 帳號與裝置硬體 ID」回傳至雲端試算表完成登記與累計。
- **`v3.2.6`**：**補齊既有已兌換裝置自動結合 Google 帳號登記雲端**：針對先前已輸入過 10 台版兌換碼（`CN2M-` / `CN3M-` / `CNPRO-`）的裝置，啟動 App 或於「透過 Google 帳號還原授權」輸入 Email 時，自動將該裝置硬體指紋與 Google 帳號同步登記至雲端授權表單（納入 10 台裝置累計與去重）。
- **`v3.2.5`**：**10 台裝置版兌換碼（`CN2M-` / `CN3M-` / `CNPRO-`）新增雲端裝置數累計與去重**：兌換時自動向雲端授權表單登記 Widevine 硬體指紋並嚴格限制最多 10 台不同裝置（同機重裝不重複計算；`CNFAM-`／`CNVIP` 系列維持不限裝置）。
- **`v3.2.4`**：**Tab 3 陸版語音攔截新增「攔截後啟動目標 AI 選單」**：支援四種啟動模式切換——① **預設：Gemini 系統浮層視窗**；② **直接進入 Gemini Live（即時語音對話）**；③ **直接啟動客製化 AI 語音接收模式**（內建熱門 AI 清單含 ChatGPT 語音對話、Google Gemini 語音、Perplexity、Microsoft Copilot、Grok、豆包 Doubao、Claude、Kimi、DeepSeek，自動偵測本機安裝狀態）；④ **僅啟動目標 App**（可搜尋所有已安裝 App 含圖示選取）。
- **`v3.2.3`**：① **Tab 5 懸浮工作列全面重設計**：左側精簡為「待命／啟動」兩段明確狀態提示；右側改為「`來源語系` ⇄ `目標語言`」雙向獨立選單與一鍵左右互換按鈕（移除 App 內多餘的來源語系對話框選項）；② **Tab 6 新增「Google 畫圈搜尋 / MiCTS 防凍結加速」（預設開啟）**：透過 Shizuku 自動將 Google App 加入 Doze 省電與背景執行白名單，改善 OriginOS／陸版系統凍結導致的 3 秒延遲；③ **設定備份匯出支援自訂本機裝置名稱前綴**：於匯出設定上方可直接輸入裝置名稱並自動冠於 `.json` 備份檔名前方。
- **`v3.2.2`**：① 修復「穿透式捲動翻譯」於網頁（Chrome／WebView）含有行內超連結（`<a href>`）或置頂／置底懸浮廣告時出現段落斷裂漏翻、單詞誤譯與遮擋鬼影的問題——改採**截圖視覺 OCR 優先＋兩階段視覺段落重組引擎**（先橫向合併同行內超連結片段、再依單行字高跨區塊重組完整段落），並依畫面語系智慧選擇辨識器與對比度／最小字高過濾（消除微縮圖亂碼與暗角廣告誤翻），翻譯完整度對齊 Google 畫圈搜尋；② 修復動態廣告頻繁觸發 `WINDOW_CONTENT_CHANGED` 中斷翻譯或退回節點模式的問題，並為短按鈕（如 `Like` → `喜歡`）加入橫向膠囊自適應展寬避免直排擠壓；③ 排除 `MiCTS`／`VISTrigger` 與畫圈搜尋懸浮層於無障礙截圖與環境隱身的競爭，降低觸發干擾。
- **`v3.2.1`**：① 徹底修復「穿透式捲動翻譯」點擊螢幕時因外部觸控偵測／截圖冷卻與同 App 彈窗事件導致翻譯臨時消失、需再點一下才恢復的問題——改為全程鎖定持續翻譯，**唯一關閉入口僅限懸浮膠囊右側「✕」按鈕與 App 本體開關**；② 預設語系升級為**全球語言自動偵測（同 Google 翻譯自動判斷全球 130+ 種可用語言與簡繁轉換）**，並補充說明**國際版／台版無內建捲動翻譯之手機亦可直接使用**；③ 設定內新增 **「橘色灰黑底主題（Orange Dark）」**；④ 強化設定備份與還原，確保 **Tab 1～6 所有頁面參數、外觀主題（含橘色灰黑底）與介面語言** 100% 完整備份並於還原時即時重載生效。
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
   - **Root-Free・Global 130+ Language Auto-Detect + ML Kit Vision OCR Dual Engine (Matching Native Google Scroll Translate Speed)**: Works on **both CN ROM phones AND Global/International Android phones that lack built-in Scroll Translate**! Automatically detects all 130+ languages supported by Google Translate and overlays translated text directly over original screen coordinates with full touch pass-through. Stays continuously active without ever cancelling on screen taps—only the capsule's `✕` button or the App's Tab 5 switch turns it off.
   - **Standalone Launcher Shortcut App (`G-Scroll` / `仿G 捲動`)**: Generates a tiny standalone launcher app so any edge-gesture app, system smart sidebar, or custom launcher can bind it under "Launch Application". Users can uninstall it individually anytime (detected dynamically by the main app), and uninstalling the main app automatically removes it together.
   - **Licensing & Existing Buyers**: Unlocked for **Pro (NT\$260)** and **Premium (NT\$380)** users (Plus remains NT\$120; +1 Tier Upgrade Add-on is NT\$150). **Existing Pro and Premium buyers retain full entitlement automatically without price re-evaluation.**

6. **Tab 6 — Free Tools (`Permanently Free・Tailored for Vivo / iQOO CN ROM`) & Recommended Links**
   - **Double-Tap Power Key Camera (Vivo CN ROM Fix)**, **Vivo / iQOO CN Navigation Voice Fix (Google TTS)**, **Shizuku Silent APK Installer**, **Developer / USB Notification Diagnostics & Gmail Export**, **CN ROM Google Maps Timeline Unlock (640 dp Workaround)**, **Vivo Mini-Screen Mode Accessibility Guard**, and **Auto-Dismiss Android System Warning Notifications**.
   - **Recommended Companion Projects (Friend Links)**:
     1. **Vivo CN ROM Dual-App Notification Fix** (by Reeky-ux / 飛雪連天 冷大): https://github.com/Reeky-ux/VIVO_Notification_Fix
     2. **MiCTS (Trigger Circle to Search / Translate)**: https://github.com/parallelcc/MiCTS — Recommended APKs: `MiCTS.apk` (triggers Circle to Search translation) & `VISTrigger.apk` (manually triggers the Gemini voice/circle overlay)
     3. **Bada (Global Quick Share Channel for CN ROMs)**: https://github.com/kyujin-cho/Bada — Connects CN ROM Android phones to global Android Nearby Share / Quick Share channels (does not connect to AirDrop yet, but enables mutual discovery and file transfer between Global and CN Android phones).

### 🔄 Recent Changelog Summary (`v0.1.0` → `v3.5.1`)

- **`v3.5.1`**: **Zero-Flicker Window Capture, Matched Typography/Layout, Embedded Image OCR & Fast Circle Handoff Toggle**:
  - **Zero-Flicker & Ad-Carousel Immunity**: Uses `takeScreenshotOfWindow` on Android 14+ so overlays and the control bar never blink or capture ghost text, and ignores background auto-scrolling ad carousels while reading.
  - **Matched Font Scale & Layout**: Scales translated text to the original single-line height (`6.5sp` micro-labels up to `34sp` bold headings), left/top-aligns paragraphs, and prevents headings from merging into subtitles.
  - **Image & UI Screenshot Translation**: Boosted native OCR resolution (`2460px`), added dual Chinese+Latin OCR supplement in Auto mode, and raised per-screen capacity to `90` blocks.
  - **Fast Circle Handoff Toggle & Z-Order Fix**: Added a "Link Pass-Through Scroll Translate" switch on Tab 6, auto-raises Z-order above Google Circle to Search on cold starts, and updated the 4-language User Guide.

- **`v3.5.0`**: **Added "User Guide & Feature Overview" button in Settings (4 languages)**: Added a dedicated button inside the top-right **⚙ Settings** dialog that opens a scrollable, selectable guide covering all 6 tabs, Tab 5 Pass-Through Scroll Translate usage, and Tab 5 × Tab 6 Fast Circle handoff / long-press drag / bar tracking / foldable dual-screen position memory, fully localized in English, Traditional Chinese, Simplified Chinese, and Japanese.

- **`v3.4.9`**: **Fixed Fast Circle slow trigger, sluggish/unclickable handoff button, and lingering button after closing Circle to Search**: Kept the zero-hop no-`singleInstance` architecture while keeping the translucent trigger alive briefly (~260ms / until focus loss, `circlestub` `v1.2.0`) to eliminate the 3-second `AssistStructure` timeout; moved all Google Circle window/bar inspection off the main thread (`a11yInspectExecutor`) so the button appears fast and taps reliably (`420ms` long-press threshold, generous tap slop); added active Google overlay presence monitoring so the button auto-dismisses within ~0.25s whenever you exit Circle to Search without tapping it.

- **`v3.4.8`**: **Fixed Fast Circle to Search forcing a drop back to the Home screen right after taking the screenshot**: Removed `singleInstance`, empty `taskAffinity`, and the 220ms post-trigger `finish()` delay in `FastCircleSearchActivity` & `circlestub` (aligning with MiCTS's immediate `finish()` in `onCreate()`), introduced headless `FastCircleTriggerProvider` so the standalone "Fast Circle" stub triggers Circle to Search with zero second-Activity/Task hop, and added automatic Shizuku upgrade for existing `circlestub` v1 installs.

- **`v3.4.7`**: **Long-Press Draggable Fast-Circle Handoff Button, Google Circle Bar Vertical Tracking & Foldable Inner/Outer Position Memory**: Long-press (~0.3s) the circular Pass-Through Translate handoff button over Fast Circle to Search to drag and fine-tune its position; automatically glides vertically in lockstep when Google Circle to Search's interface bar moves up or down; remembers independent saved positions for foldable inner vs. outer screens (and portrait/landscape) for both the handoff button and Scroll Translate bar.

- **`v3.4.6`**: **Direct Local / Google Drive Backup with Remembered Paths**: Export dialog now lets you pick **Local Backup** or **Google Drive Backup** directly with inline **Change Path** buttons. Local backup remembers a persisted folder (`ACTION_OPEN_DOCUMENT_TREE`) for instant 1-tap exports next time; Google Drive backup remembers the chosen Drive SAF location (`EXTRA_INITIAL_URI`) for subsequent exports & restores (with background stream writes and Drive App share fallback).

- **`v3.4.5`**: **Auto-cancel Fast Circle to Search on Screen Off**: Automatically dismisses both the bottom-right handoff button and any active Google Circle to Search overlay when the screen turns off (`ACTION_SCREEN_OFF`).

- **`v3.4.4`**: **2.5-second idle final check & sleep until next touch/scroll**: After 2.5 seconds without touch or scrolling, Pass-Through Translate performs one final check/translation and then locks idle (ignoring background mutations) until the next user touch or scroll.

- **`v3.4.3`**: **Never auto-pause Pass-Through Translate (stops only on explicit close or screen-off)**: Removed all automatic standby/pause triggers (including inside the host app and across orientation/foldable configuration changes), ensuring continuous active translation in both portrait and landscape until the user taps `✕`.

- **`v3.4.2`**: **Fixed Pass-Through Translate "flashing on then disappearing back to Standby" and missing translations after momentum scroll**: (1) Ignored self-emitted `TYPE_WINDOW_STATE_CHANGED` events from our own `TYPE_ACCESSIBILITY_OVERLAY` windows and restricted host-app checks to `TYPE_APPLICATION` windows; (2) Added a post-momentum final-settle verification pass (`finalSettleVerifyRunnable`) and micro-deceleration filter so screens always translate reliably once scrolling comes to a complete stop.

- **`v3.4.1`**: (1) **Auto-stop Pass-Through Translate on Screen Off**: Automatically stops Scroll Translate and clears overlays when the screen turns off; (2) **Pre-Circle App/Launcher State Handoff**: Captures the active App or Launcher package at the exact moment Fast Circle launches and passes it into Scroll Translate so Recents restoration reliably returns to the original App (or stays on Home if started from Home).

- **`v3.4.0`**: **Improved Recents card tap restoration for Pass-Through Translate**: Automatically opens system Recents and taps the most recently used app card if a transient Home drop occurs after launch (while skipping Recents completely when started directly on the Launcher/Home screen).

- **`v3.3.9`**: (1) **Recents-based task restoration for Pass-Through Translate**: Stays on the launcher when started from Home; when started from an app and transiently dropped to Home, restores the exact previous task via Shizuku `moveTaskToFront` (with Accessibility Recents fallback) without resetting the app screen; (2) **Full-bar dragging on the Translate bar**: Drag anywhere on the floating capsule bar to reposition and save its location.

- **`v3.3.8`**: (1) **Startup Home-screen guard for Pass-Through Translate**: Captures the active app before launch and automatically returns to that app if a transient Home drop occurs right after startup (while staying on Home if launched from Home); (2) **Horizontal swipe & touch-pause / release-to-translate**: Added non-blocking screen touch detection and `scrollX` tracking so any vertical or horizontal swipe pauses active translation on touch and immediately translates once touch stops.

- **`v3.3.7`**: (1) **Prevented accidental Home gesture triggers on bottom controls**: Added `systemGestureExclusionRects` and safe bottom gesture inset margins to both the Fast Circle handoff button and the Scroll Translate bottom bar; (2) **Immersive borderless translation overlay**: Removed the visible white box borders in `ScrollTranslateCanvasView` and improved surrounding dominant background sampling + color caching so translated text blends seamlessly into the original page.

- **`v3.3.6`**: **Added Input Method (IME) Visibility & Default Manager in Tab 6**: Lists all installed keyboards with icons and status, lets you toggle whether each IME is shown (enabled) or hidden (disabled) in the system via Shizuku, and includes a one-tap Set Default button.

- **`v3.3.5`**: **Responsive 2-column side-by-side card layout**: Automatically arranges each tab's feature cards into left/right columns on phone landscape, unfolded foldable inner screens, 8"/10" tablet landscape, and Pixelbook windows (while preserving single-column portrait on phones).

- **`v3.3.4`**: (1) **Redesigned Fast Circle handoff pill into a compact circular scroll-translate icon button pinned at the bottom-right corner** (matching Google's scroll-translate icon); (2) **Moved the default Pass-Through Scroll Translate bar position to bottom-center** (matching Google's official Circle to Search bar placement, still draggable).
- **`v3.3.3`**: **Fixed Fast Circle exiting to the Home screen upon launch**: Removed the `AssistantHandoffActivity` task-switching launch and added `singleInstance` + empty `taskAffinity` on `:circlestub`, triggering `VisTrigger.triggerCircleToSearch` directly over the current app page so both Circle to Search and Scroll Translate handoff stay on your active screen.
- **`v3.3.2`**: **Added floating "🌐 Scroll Translate" handoff pill after Fast Circle launches** (shown only when Pass-Through Scroll Translate is unlocked via paid tier): tapping it automatically dismisses Circle to Search and hands the current screen directly over to Pass-Through Scroll Translate.
- **`v3.3.1`**: (1) Removed the "Google Circle to Search / MiCTS Anti-Freeze Accelerator" card from Tab 6; (2) Fixed Option B "Fast Circle to Search" (`VisTrigger.triggerCircleToSearch`) to pass MiCTS-aligned bundle extras (`omni.entry_point = 1`, `invocation_time_ms`, `micts_trigger = true`) so it opens Circle to Search / Translate directly instead of the generic assistant sheet.
- **`v3.3.0`**: **Added "Declare Installer as Google Play Store (`-i com.android.vending`)" toggle in Tab 6 Shizuku Silent APK Installer**: Allows installing APKs (such as Android Auto companion apps like `AATube-Caster`) via Shizuku while declaring `com.android.vending` as the installer package.
- **`v3.2.9`**: (1) **Added Option B "Fast Circle to Search" Shortcut, Quick Tile & Standalone Launcher App (`Fast Circle` / `極速畫圈`) in Tab 6**: Pre-warms `AssistantHandoffActivity` (~90ms) before triggering `VisTrigger` to eliminate the ~3s Vivo OriginOS cold-handoff lag; supports generating a standalone launcher app for gesture apps ("Launch Application"), dynamically detected by the main app and auto-removed together upon uninstall (unaffected by updates); (2) **Fixed GitHub API 403 Rate-Limit Update Failures**: Added web-redirect fallback (`releases/latest`) in `UpdateChecker`; (3) **Slimmed APK ABI to `arm64-v8a`** for much faster in-app downloads.
- **`v3.2.8`**: **Added User-Selectable Preload Language Packs & Update Checker in Tab 5**: Users can select and pre-download on-device ML Kit translation packs (15 languages including ZH, EN, JA, KO, TH, VI, FR, DE, ES, RU, etc.) plus GMS OCR modules to accelerate Scroll Translate (~20ms on-device inference without network wait), and check/update all packs & OCR modules to the latest Google version.
- **`v3.2.7`**: **Auto-Report All Redeemed Codes, Google Account & Device ID on App Update**: Automatically syncs every active redeemed code (`CN2M-`/`CN3M-`/`CNPRO-`/`CNFAM-`/`CNVIP*`/Gumroad), bound Google account, and Widevine hardware ID to the cloud sheet upon app update (`MY_PACKAGE_REPLACED`) or launch.

- **`v3.2.6`**: **Auto-Sync Existing 10-Device Redemptions with Google Account**: Devices that already redeemed a 10-device code (`CN2M-` / `CN3M-` / `CNPRO-`) automatically sync their hardware ID and Google account email to the cloud license sheet on launch or when verifying via Google Account Restore.
- **`v3.2.5`**: **Added Cloud Device Counting & Deduplication for 10-Device Redemption Codes (`CN2M-` / `CN3M-` / `CNPRO-`)**: Registers Widevine hardware IDs in the cloud license sheet (`usage / 10`) while keeping `CNFAM-` / `CNVIP` codes unlimited.
- **`v3.2.4`**: **Added Target AI Selector to Tab 3 (Voice Intercept)**: Choose between 4 launch modes after intercepting CN voice assistants — (1) **Default: Gemini System Overlay**; (2) **Direct Launch: Gemini Live**; (3) **Custom AI Voice Mode** (curated popular AI list with auto-detected install status: ChatGPT Voice, Google Gemini Voice, Perplexity, Microsoft Copilot, Grok, Doubao, Claude, Kimi, DeepSeek); (4) **Launch Target App Only** (searchable picker with app icons).
- **`v3.2.3`**: (1) **Redesigned Tab 5 Floating Capsule**: Simplified the left badge to clean `Standby` / `Active` (`待命` / `啟動`) states, and replaced the right controls with symmetric **`Source` ⇄ `Target Lang` (`來源語系` ⇄ `目標語言`)** pickers and one-tap language swapping (removed the redundant in-app source language button); (2) **Added "Google Circle to Search / MiCTS Anti-Freeze Accelerator" in Tab 6 (ON by default)**: Uses Shizuku to keep `com.google.android.googlequicksearchbox` in Doze & AppOps background whitelists; (3) **Added Custom Device Name Prefix to Settings Backup**: Export dialog now includes an optional device name field prepended to exported `.json` filenames.
- **`v3.2.2`**: (1) Fixed Pass-Through Scroll Translate partial/fragmented paragraph translations and occluded ghost boxes on Chrome/WebView pages containing inline `<a href>` links or sticky headers/ads—upgraded to a **Visual Screenshot OCR-primary + 2-Stage Layout Reconstructor** (merging same-row inline link spans and clustering paragraphs by single-line height across TextBlocks, matching Google Circle to Search layout quality), plus script-aware OCR selection and contrast/micro-text filtering to eliminate diagram/dim-ad hallucinations; (2) Blocked background animated-ad `WINDOW_CONTENT_CHANGED` storms from aborting active screenshot passes or falling back to fragmented node mode, and added horizontal pill expansion so short buttons (`Like` → `喜歡`) stay single-line; (3) Excluded `MiCTS` / `VISTrigger` and Circle to Search overlays from Accessibility thumbnail screenshots and Stealth checks to eliminate trigger contention.
- **`v3.2.1`**: (1) Fixed Pass-Through Scroll Translate temporarily hiding/cancelling on screen taps due to outside-touch screenshot cooldown & same-app popup events—translation now stays continuously locked on until explicitly closed via the capsule's `✕` button or the App's Tab 5 switch; (2) Upgraded default detection to **Global Language Auto-Detect (all 130+ Google Translate languages)** and documented support for **Global/International Android phones without built-in Scroll Translate**; (3) Added **Orange on Dark Gray (`橘色灰黑底`)** theme in Settings; (4) Verified and enhanced **full 6-Tab + Theme/Language Settings Backup & Restore** with automatic state materialization and instant UI reload on restore.
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
