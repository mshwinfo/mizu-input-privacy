# 隱私政策 Privacy Policy

**謎之輸入法 mizu input**
最後更新日期：2026-07-12

本頁為謎之輸入法（mizu input，HarmonyOS）的公開隱私政策，供應用市場審核與使用者參閱。

> **正式頁面 Official page**：https://mshwinfo.github.io/mizu-input-privacy/
> 應用市場後台與 App 內連結請一律填寫上方 GitHub Pages 網址。

## 下載檔案 Downloads
- [`downloads/ja_words_full.txt`](downloads/ja_words_full.txt) — 完整版日文詞庫（16.2 萬讀音，生成自 JMdict，見主專案 `THIRD_PARTY_LICENSES.md`）。於 App 主程式「日文詞庫」下載並匯入即可使用。
- [`downloads/table_wubi86.txt`](downloads/table_wubi86.txt) — 五筆 86 碼表（轉換版，7.6 萬編碼）。轉換自 [rime/rime-wubi](https://github.com/rime/rime-wubi)，LGPL-3.0 授權（見 [`downloads/LGPL-3.0.txt`](downloads/LGPL-3.0.txt)）。於 App 主程式「匯入五筆碼表」選擇此檔即可。
- [`downloads/table_stroke.txt`](downloads/table_stroke.txt) — 筆畫碼表（轉換版，3.4 萬編碼，h/s/p/n/z 五筆畫）。轉換自 [rime/rime-stroke](https://github.com/rime/rime-stroke)，LGPL-3.0 授權。於 App 主程式「匯入筆畫碼表」選擇此檔即可。

> 轉換版碼表已過濾一般輸入用不到的罕用漢字（CJK 擴充區、相容表意文字等），並統一為 App 的 `code=候選` 內部格式，檔案更小、匯入更快。轉換不更動任何編碼規則。

---

## 繁體中文

### 總覽
謎之輸入法（以下稱「本輸入法」）尊重並保護使用者隱私。本輸入法為**完全離線**運作的輸入法，**不會收集、不會上傳、不會分享**您輸入的任何內容。本文件說明本輸入法如何處理資料。

### 我們不做的事
- **不收集您輸入的文字**：您透過本輸入法鍵入的任何內容，僅用於當下的輸入轉換，不會被記錄、傳送或儲存到任何伺服器。
- **不連網、不上傳**：本輸入法核心功能不需要網路權限，不會將任何資料傳送到外部伺服器或雲端。
- **無帳號、無登入**：本輸入法不要求註冊或登入，不收集任何個人身分資訊。
- **無廣告、無第三方分析 SDK**：不整合任何廣告或使用者行為追蹤工具。

### 儲存在您裝置本機的資料
以下資料僅儲存在您裝置的應用程式私有空間，不會離開您的裝置，解除安裝 App 即一併移除：
- **輸入偏好設定**：如震動／按鍵音開關、音量與強度、簡體輸出、模糊音、啟用的輸入法語言、鍵盤底圖等。
- **使用者詞庫學習**：為提升選字準確度，本輸入法會在本機記錄您選過的字詞頻率（含中文與英文）。此資料僅存於本機，不上傳。
- **剪貼簿歷史（預設關閉）**：此功能預設為關閉；僅在您於鍵盤設定中主動開啟「剪貼簿歷史」後，才會在本機記錄最近複製的文字（上限 20 筆），供您快速貼上使用，不上傳；可於面板內清除，關閉後亦會一併清除既有記錄。未開啟時，本輸入法不會在背景讀取或記錄系統剪貼簿。
- **最近使用的表情符號**：Emoji 面板會在本機記錄最近使用的表情（上限 24 筆）。
- **匯入的碼表／詞庫**：您自行匯入的形碼碼表檔、日文完整版詞庫，僅存於本機供輸入使用。
- **鍵盤底圖**：您從相簿選擇的鍵盤背景圖片，僅複製一份存於本機供顯示使用。
- **備份檔案**：您於「備份與還原」主動匯出的設定與學習資料備份檔（JSON），內容與上述本機資料相同，儲存於您指定的裝置位置；本輸入法不會自動上傳或分享此檔案，匯入時也僅在您主動選擇檔案後才讀取。

### 權限說明
- **震動（ohos.permission.VIBRATE）**：用於按鍵震動回饋，可於設定關閉。
- **剪貼簿存取**：複製／貼上僅於您主動操作時讀寫系統剪貼簿，內容不離開裝置。背景記錄剪貼簿歷史的功能預設關閉，僅在您主動開啟後才啟用。
- **相簿存取**：僅於您主動點擊「選擇底圖」時，透過系統相簿選擇器挑選單張圖片，不會批次存取或掃描您的相簿。

### 關於「完整體驗模式」
HarmonyOS 會對所有第三方輸入法顯示是否啟用「完整體驗模式」的系統級提示（非本輸入法特有的行為）。系統未授予此模式時，會限制部分能力（例如按鍵震動）；開啟後這些功能才能正常運作。該提示顯示的「可能傳輸您輸入的內容」為系統對此模式的通用制式警語（所有第三方輸入法皆顯示相同文字），並非本輸入法會如此運作——本輸入法完全離線、未宣告任何網路權限，技術上不可能傳送任何資料。

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
mizu input ("the IME") respects and protects user privacy. The IME operates **fully offline** and does **not collect, upload, or share** anything you type. This document explains how the IME handles data.

### What we do NOT do
- **We do not collect what you type.** Text entered through the IME is used only for on-device input conversion and is never logged, transmitted, or stored on any server.
- **No network, no upload.** Core functionality requires no network permission; no data is sent to any external server or cloud.
- **No account, no login.** No registration or personal identity information is collected.
- **No ads, no third-party analytics SDKs.**

### Data stored locally on your device
The following is stored only in the app's private storage on your device, never leaves your device, and is removed when you uninstall the app:
- **Input preferences** (haptics/sound toggles, volume/intensity, Simplified output, fuzzy phonetics, enabled input languages, keyboard background image, etc.).
- **User dictionary learning**: selection frequencies (Chinese and English) recorded locally to improve candidate ordering. Local only; never uploaded.
- **Clipboard history (off by default)**: disabled unless you turn on "Clipboard history" in the keyboard settings. Only then does it keep up to 20 recently copied items locally for quick paste; never uploaded; can be cleared in the panel and is cleared when you turn the feature off. While disabled, the IME does not read or record the system clipboard in the background.
- **Recently used emoji** (up to 24, local).
- **Imported code tables / dictionaries**: shape-based code tables and the full Japanese dictionary you import yourself, stored locally for input only.
- **Keyboard background image**: a photo you pick is copied locally for display only.
- **Backup file**: a JSON file you export from "Backup & Restore" containing the same local data above, saved to a location you choose; the IME never uploads or shares it automatically, and only reads a file you actively pick when importing.

### Permissions
- **Vibration (ohos.permission.VIBRATE)**: for key haptic feedback; can be turned off in settings.
- **Clipboard access**: copy/paste read and write the system clipboard only when you actively trigger them; content never leaves the device. Background clipboard-history recording is off by default and only runs after you enable it.
- **Photo access**: only triggered when you tap "Choose background" via the system photo picker for a single image; no bulk access or scanning of your photo library.

### About "Full Experience Mode"
HarmonyOS shows a system-level prompt asking whether to enable "Full Experience Mode" for all third-party input methods (not specific to this IME). When not granted, some capabilities (e.g. key vibration) are restricted; enabling it allows them to work normally. The prompt's warning that the app "may transmit anything you type" is HarmonyOS's standard boilerplate for this mode (shown identically for every third-party keyboard) — it does not describe what this IME actually does. As stated above, this IME is fully offline and declares no network permission, so it is technically incapable of transmitting any data.

### External links
Links under "Where to find code tables" and "Support the developer" open your device browser to third-party sites (e.g. GitHub, Ko-fi, ECPay); the IME is not involved in anything you do there (including donation/payment flows), and those sites have their own privacy policies.

### Children's privacy
The IME is not directed at children and does not knowingly collect children's personal information (in fact it collects no one's personal information).

### Changes
Updates will be reflected on this page via the "Last updated" date.

### Contact
For questions about this policy, please open a GitHub Issue:
https://github.com/mshwinfo/mizu-input-privacy/issues
