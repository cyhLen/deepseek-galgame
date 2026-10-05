# 🎮 DeepSeek Gal View

> A userscript (Tampermonkey) that turns the DeepSeek web chat interface into a **Galgame / visual-novel style** experience.
> Late-night bedroom vibes, whale girl, gorgeous dialog box, typewriter effect — every conversation feels like playing a game.

---

## 🖼️ Preview

### Chat Interface

<img src="屏幕截图_3-10-2026_165938_chat.deepseek.com.jpeg" alt="Chat Interface" width="720" />

### Config Panel

<img src="屏幕截图_3-10-2026_1710_chat.deepseek.com.jpeg" alt="Config Panel" width="720" />

---

## ✨ Features

- **Visual-novel style UI**: bedroom background, blue-haired whale girl, gradient dialog box, star sparkles, watermark
- **Typewriter effect**: adjustable speed / can be disabled
- **Enhanced Markdown rendering**: white text, compact line height, bold white table borders, polished code blocks
- **Code-block actions**: one-click copy (with ✓ feedback), download by language
- **File attachment**: three-color detail (name / type / size), left-aligned, deletable
- **Deep Think / Web Search toggles**: aligned with attachments, native-style icons, toggles the native mode in real time
- **Background system**: built-in default + local image import + URL import (save to browser / URL-only), multi-background selection with thumbnails, persisted in IndexedDB
- **Full menu**: AUTO / SKIP / LOG / SAVE / LOAD / CONFIG / Exit
- **Native DeepSeek logo badge**: the whale icon identical to the official page

## 🔧 Config Options

| Option | Description |
|---|---|
| AUTO mode | Disable typewriter, show full text directly |
| Sound effects | On / off |
| Background dim | 0–70% |
| Dialog box opacity | 60–100% |
| Font size | 15–25px |
| Typewriter speed | 0–60ms (lower = faster) |
| Background | Default / import / URL, switchable |

## 📦 Install

1. Install the [Tampermonkey](https://www.tampermonkey.net/) extension
2. Import the script file `deepseek-gal-view-1.1.user.js`
3. Open `https://chat.deepseek.com`

## 🎯 Usage

- Click **✦ Gal View** (top-right) to enter the Gal interface
- Click **CONFIG** to open the settings panel (background options are here)
- All settings are auto-saved to the local browser

## 🛠️ Tech Notes

- Backgrounds are stored in **IndexedDB**, the selection in **localStorage** — both survive refresh / restart
- Body Markdown reuses the native `.ds-markdown` renderer for parity with the original page
- Attachment upload / toggles are triggered by programmatically clicking the native controls

## 📄 License

For personal learning and entertainment only.

---

*Version 1.1.0*
