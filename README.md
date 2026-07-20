# 隱私政策 Privacy Policy

**謎之輸入法**
最後更新日期：2026-07-20

本頁為謎之輸入法（mizu input，HarmonyOS）的公開隱私政策，供應用市場審核與使用者參閱。

> **正式頁面 Official page**：https://mshwinfo.github.io/mizu-input-privacy/
> 應用市場後台與 App 內連結請一律填寫上方 GitHub Pages 網址。

## 下載檔案 Downloads

> **下載頁 Download page**：https://mshwinfo.github.io/mizu-input-privacy/downloads/
> （建議由此頁下載——點按鈕直接下載檔案，不會在瀏覽器中開啟內容。）

- [`downloads/ja_words_full.txt`](downloads/ja_words_full.txt) — 完整版日文詞庫（16.2 萬讀音，生成自 JMdict，見主專案 `THIRD_PARTY_LICENSES.md`）。於 App 主程式「日文詞庫」下載並匯入即可使用。
- [`downloads/table_wubi86.txt`](downloads/table_wubi86.txt) — 五筆 86 碼表（轉換版，7.6 萬編碼）。轉換自 [rime/rime-wubi](https://github.com/rime/rime-wubi)，LGPL-3.0 授權（見 [`downloads/LGPL-3.0.txt`](downloads/LGPL-3.0.txt)）。於 App 主程式「匯入五筆碼表」選擇此檔即可。
- [`downloads/table_stroke.txt`](downloads/table_stroke.txt) — 筆畫碼表（轉換版，3.4 萬編碼，h/s/p/n/z 五筆畫）。轉換自 [rime/rime-stroke](https://github.com/rime/rime-stroke)，LGPL-3.0 授權。於 App 主程式「匯入筆畫碼表」選擇此檔即可。

> 轉換版碼表已過濾一般輸入用不到的罕用漢字（CJK 擴充區、相容表意文字等），並統一為 App 的 `code=候選` 內部格式，檔案更小、匯入更快。轉換不更動任何編碼規則。

---

## 繁體中文

### 總覽
謎之輸入法（以下稱「本輸入法」）尊重並保護使用者隱私。本輸入法的**打字輸入**核心功能為**完全離線**運作，**不會收集、不會上傳、不會分享**您鍵入的任何文字。本輸入法另提供**語音輸入**這項**選用**功能，僅在您主動點擊語音輸入按鍵時才會啟用，啟用時會將您的語音上傳至華為雲端進行辨識（詳見下方「關於語音輸入」）；除此之外，本輸入法不會傳送任何資料。本文件說明本輸入法如何處理資料。

### 我們不做的事
- **不收集您鍵入的文字**：您透過本輸入法鍵入的任何內容，僅用於當下的輸入轉換，不會被記錄、傳送或儲存到任何伺服器。
- **打字功能不連網、不上傳**：本輸入法的打字輸入核心功能不需要網路權限，不會將任何資料傳送到外部伺服器或雲端；僅「語音輸入」這項選用功能在您主動使用時例外（見下）。
- **無帳號、無登入**：本輸入法不要求註冊或登入，不收集任何個人身分資訊。
- **無廣告、無第三方分析 SDK**：不整合任何廣告或使用者行為追蹤工具。

### 關於語音輸入
語音輸入為**選用**功能，預設需您在鍵盤面板中主動點擊語音輸入按鍵才會啟動，不會在背景自動錄音。啟用後：
- 本輸入法會透過 HarmonyOS 系統的語音辨識服務（Core Speech Kit），將您當次的語音**即時上傳至華為雲端**進行辨識，並將辨識出的文字回傳顯示；辨識完成或您取消後即結束本次連線。
- 之所以採用雲端辨識，是因為 HarmonyOS 系統對第三方應用（非系統內建應用）的純離線語音辨識設有存取限制，僅雲端辨識路徑對第三方應用開放；語音資料的傳輸與後續處理由華為的語音辨識服務負責，其保存與使用方式請參閱華為相關服務條款。
- 使用語音輸入需要麥克風權限（僅於您點擊語音輸入按鍵時使用，不會背景擷取）與網路連線，且需要您已將本輸入法切換為系統的「完整體驗模式」。
- 若您不希望語音內容經由網路傳送，請不要使用語音輸入按鍵；不使用此功能時，本輸入法完全不會存取麥克風或網路。

### 儲存在您裝置本機的資料
以下資料僅儲存在您裝置的應用程式私有空間，不會離開您的裝置，解除安裝 App 即一併移除：
- **輸入偏好設定**：如震動／按鍵音開關、音量與強度、簡體輸出、模糊音、啟用的輸入法語言、鍵盤底圖等。
- **使用者詞庫學習**：為提升選字準確度，本輸入法會在本機記錄您選過的字詞頻率（含中文與英文）。此資料僅存於本機，不上傳。
- **剪貼簿歷史（預設關閉）**：此功能預設為關閉；僅在您於鍵盤設定中主動開啟「剪貼簿歷史」後，才會在本機記錄最近複製的文字（上限 20 筆），供您快速貼上使用，不上傳；可於面板內清除，關閉後亦會一併清除既有記錄。未開啟時，本輸入法不會在背景讀取或記錄系統剪貼簿。
- **最近使用的表情符號**：Emoji 面板會在本機記錄最近使用的表情（上限 24 筆）。
- **匯入的碼表／詞庫**：您自行匯入的形碼碼表檔、日文完整版詞庫，僅存於本機供輸入使用。
- **鍵盤底圖**：您從相簿選擇的鍵盤背景圖片，僅複製一份存於本機供顯示使用。

### 權限說明
- **震動（ohos.permission.VIBRATE）**：用於按鍵震動回饋，可於設定關閉。
- **剪貼簿存取**：複製／貼上僅於您主動操作時讀寫系統剪貼簿，內容不離開裝置。背景記錄剪貼簿歷史的功能預設關閉，僅在您主動開啟後才啟用。
- **相簿存取**：僅於您主動點擊「選擇底圖」時，透過系統相簿選擇器挑選單張圖片（可先選相簿目錄縮小範圍，方便相片多時尋找），不會批次讀取或掃描您的相片內容。
- **麥克風（ohos.permission.MICROPHONE）**：僅於您主動點擊語音輸入按鍵時使用，用於將語音上傳華為雲端辨識為文字；不使用語音輸入功能時不會擷取麥克風。

### 關於「完整體驗模式」
HarmonyOS 會對所有第三方輸入法顯示是否啟用「完整體驗模式」的系統級提示（非本輸入法特有的行為）。系統未授予此模式時，會限制部分能力（例如按鍵震動、語音輸入）；開啟後這些功能才能正常運作。該提示顯示的「可能傳輸您輸入的內容」為系統對此模式的通用制式警語（所有第三方輸入法皆顯示相同文字）——本輸入法的打字輸入完全離線、未宣告任何網路權限，技術上不可能傳送任何資料；僅語音輸入這項選用功能在您主動使用時，會依上方「關於語音輸入」所述將語音上傳雲端辨識。

### 外部連結
主程式「哪裡找碼表？」與「支持開發者」提供的連結會開啟您裝置的瀏覽器前往第三方網站（如 GitHub、Ko-fi、綠界科技），本輸入法不經手您在該網站的任何行為（包括贊助／付款流程），該網站有其自身的隱私政策。

### 兒童隱私
本輸入法不針對兒童設計，也不會刻意收集兒童的個人資訊（實際上本輸入法不收集任何人的個人資訊）。

### 政策變更
若本政策有更新，將於本頁更新「最後更新日期」。

### 聯絡方式
如對本隱私政策有任何疑問，請透過 GitHub Issues 聯絡：
https://github.com/mshwinfo/mizu-input-privacy/issues

---

## English

### Overview
mizu input ("the IME") respects and protects user privacy. The IME's core **typing** functionality operates **fully offline** and does **not collect, upload, or share** anything you type. The IME also offers an **optional Voice Input** feature that only activates when you actively tap the voice input button; when used, it uploads your speech to Huawei's cloud for recognition (see "About Voice Input" below). Outside of that, the IME never transmits any data. This document explains how the IME handles data.

### What we do NOT do
- **We do not collect what you type.** Text entered through the IME is used only for on-device input conversion and is never logged, transmitted, or stored on any server.
- **No network, no upload for typing.** Core typing functionality requires no network permission and sends no data to any external server or cloud; the only exception is the optional Voice Input feature when you actively use it (see below).
- **No account, no login.** No registration or personal identity information is collected.
- **No ads, no third-party analytics SDKs.**

### About Voice Input
Voice Input is an **optional** feature: it only starts recording when you actively tap the voice input button in the keyboard panel, never in the background. When you use it:
- The IME uses HarmonyOS's built-in speech recognition service (Core Speech Kit) to stream your speech **to Huawei's cloud** for recognition in real time, and displays the recognized text as it comes back; the connection ends when recognition completes or you cancel.
- Cloud recognition is used because HarmonyOS restricts fully on-device speech recognition for third-party (non-system) apps — only the cloud recognition path is available to apps like this one. The transmission and subsequent handling of your voice data is performed by Huawei's speech recognition service; refer to Huawei's own service terms for how it is retained and used.
- Voice Input requires microphone permission (used only while you're actively tapping the voice button, never captured in the background), a network connection, and requires the IME to be switched into HarmonyOS's "Full Experience Mode."
- If you do not want your voice sent over the network, simply don't use the voice input button — when unused, the IME never accesses the microphone or network.

### Data stored locally on your device
The following is stored only in the app's private storage on your device, never leaves your device, and is removed when you uninstall the app:
- **Input preferences** (haptics/sound toggles, volume/intensity, Simplified output, fuzzy phonetics, enabled input languages, keyboard background image, etc.).
- **User dictionary learning**: selection frequencies (Chinese and English) recorded locally to improve candidate ordering. Local only; never uploaded.
- **Clipboard history (off by default)**: disabled unless you turn on "Clipboard history" in the keyboard settings. Only then does it keep up to 20 recently copied items locally for quick paste; never uploaded; can be cleared in the panel and is cleared when you turn the feature off. While disabled, the IME does not read or record the system clipboard in the background.
- **Recently used emoji** (up to 24, local).
- **Imported code tables / dictionaries**: shape-based code tables and the full Japanese dictionary you import yourself, stored locally for input only.
- **Keyboard background image**: a photo you pick is copied locally for display only.

### Permissions
- **Vibration (ohos.permission.VIBRATE)**: for key haptic feedback; can be turned off in settings.
- **Clipboard access**: copy/paste read and write the system clipboard only when you actively trigger them; content never leaves the device. Background clipboard-history recording is off by default and only runs after you enable it.
- **Photo access**: only triggered when you tap "Choose background" via the system photo picker (you may first pick an album/folder to narrow it down, which helps when you have many photos) for a single image; no bulk access or scanning of your photo content.
- **Microphone (ohos.permission.MICROPHONE)**: used only while you're actively tapping the voice input button, to upload speech to Huawei's cloud for recognition (see "About Voice Input" above); the microphone is never accessed when Voice Input is not in use.

### About "Full Experience Mode"
HarmonyOS shows a system-level prompt asking whether to enable "Full Experience Mode" for all third-party input methods (not specific to this IME). When not granted, some capabilities (e.g. key vibration, Voice Input) are restricted; enabling it allows them to work normally. The prompt's warning that the app "may transmit anything you type" is HarmonyOS's standard boilerplate for this mode (shown identically for every third-party keyboard) — the IME's typing functionality is fully offline and declares no network permission, so it is technically incapable of transmitting any data; only the optional Voice Input feature, when you actively use it, uploads speech to the cloud as described above.

### External links
Links under "Where to find code tables" and "Support the developer" open your device browser to third-party sites (e.g. GitHub, Ko-fi, ECPay); the IME is not involved in anything you do there (including donation/payment flows), and those sites have their own privacy policies.

### Children's privacy
The IME is not directed at children and does not knowingly collect children's personal information (in fact it collects no one's personal information).

### Changes
Updates will be reflected on this page via the "Last updated" date.

### Contact
For questions about this policy, please open a GitHub Issue:
https://github.com/mshwinfo/mizu-input-privacy/issues
