# 圖片全載Next Pro / Full Picture Load Next Pro

> Modern image batch downloader supporting 1000+ sites, infinite scroll, ZIP packaging

## 📦 Available Versions

| Version | File | Best For |
|---------|------|----------|
| **Universal** | `FullPictureLoad_Next_Pro_v2026.4.0.user.js` | Works on both TM and VM |
| **Tampermonkey** | `FullPictureLoad_Next_Pro_Tampermonkey.user.js` | **Recommended for TM users** |
| **Violentmonkey** | `FullPictureLoad_Next_Pro_Violentmonkey.user.js` | **Recommended for VM users** |

---

## 🚀 Quick Install

### For Tampermonkey Users

1. Install [Tampermonkey](https://www.tampermonkey.net/) extension
2. Click this link to install:
   ```
   https://github.com/HeartlessVeteran2/FullPictureLoad-Pro/raw/main/FullPictureLoad_Next_Pro_Tampermonkey.user.js
   ```
3. Or manually copy from:
   ```
   https://github.com/HeartlessVeteran2/FullPictureLoad-Pro/blob/main/FullPictureLoad_Next_Pro_Tampermonkey.user.js
   ```

**Tampermonkey Features:**
- ✅ Native download via `GM_download`
- ✅ Desktop notifications via `GM_notification`
- ✅ Enhanced menu commands
- ✅ Better error handling

---

### For Violentmonkey Users

1. Install [Violentmonkey](https://violentmonkey.github.io/) extension
2. Click this link to install:
   ```
   https://github.com/HeartlessVeteran2/FullPictureLoad-Pro/raw/main/FullPictureLoad_Next_Pro_Violentmonkey.user.js
   ```
3. Or manually copy from:
   ```
   https://github.com/HeartlessVeteran2/FullPictureLoad-Pro/blob/main/FullPictureLoad_Next_Pro_Violentmonkey.user.js
   ```

**Violentmonkey Features:**
- ✅ Cross-browser compatibility
- ✅ Modern `GM.*` API
- ✅ Lightweight approach
- ✅ Open source friendly

---

### For Other Managers (Greasemonkey, etc.)

Use the **Universal** version:
```
https://github.com/HeartlessVeteran2/FullPictureLoad-Pro/raw/main/FullPictureLoad_Next_Pro_v2026.4.0.user.js
```

---

## 🎯 Supported Sites (685+)

### Photo/Portfolio
- Pexels, Unsplash, Behance, ArtStation, DeviantArt, Pixiv, Wallhaven, AlphaCoders

### Manga/Comic
- MangaDex, MangaNato, Dynasty Reader, ManyToon, Toonily
- 拷贝漫画, 漫画柜, 咚漫, LINE Webtoon, Piccoma
- Comici, Ganma, Gangan Online, Comic Days family

### NSFW/Adult
- 300+ cosplay/H-comic sites

### International
- Russian, Indonesian, Vietnamese, Turkish, Thai, Korean, Japanese

---

## 🛠️ Usage

1. **Browse** to any supported site
2. **Click** the floating "📥 FPL" button (top-right corner)
3. **Wait** for scan to complete
4. **Click Download** to save as ZIP

### Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Ctrl + D` | Start download |
| `Escape` | Cancel download |

### Menu Commands (Tampermonkey)

Right-click the userscript icon for:
- 📥 Download Images
- 🔍 Rescan Page
- ⚙️ Settings
- 📊 Stats

---

## ⚙️ Configuration

Click the floating button → Settings to configure:

| Option | Description | Default |
|--------|-------------|---------|
| Threading | Parallel downloads | 8 |
| Retry | Failed retry attempts | 3 |
| ZIP | Enable ZIP packaging | ✅ |
| Auto-insert | Auto-scan pages | ✅ |
| Comic Mode | Mobile UA for manga | ❌ |
| Fancybox | Gallery viewer | ✅ |

---

## 🔄 Version History

### v2026.4.0-TM / v2026.4.0-VM
- 685 sites converted from original FullPictureLoad
- New SiteRouter architecture
- Separate optimized versions for TM/VM
- Improved download manager with PQueue

---

## 🐛 Troubleshooting

### Script not running?
- Check if site URL matches `@match` patterns
- Verify userscript manager is enabled
- Try refreshing the page

### Images not loading?
- Site may have updated structure
- Check browser console for errors
- Try rescanning (Ctrl+Click the button)

### Download failures?
- Increase retry count in settings
- Check if site requires login
- Try lowering thread count

---

## 📁 File Structure

```
FullPictureLoad-Pro/
├── FullPictureLoad_Next_Pro_v2026.4.0.user.js    # Universal version
├── FullPictureLoad_Next_Pro_Tampermonkey.user.js # TM optimized
├── FullPictureLoad_Next_Pro_Violentmonkey.user.js # VM optimized
├── README.md                                      # This file
└── COMPLETION_REPORT.md                           # Build details
```

---

## 🙏 Credits

- Original FullPictureLoad by 德克斯DEX
- Converted and modernized by Aura
- 685 sites across 13 batches

---

## 📜 License

Original work by 德克斯DEX. This Pro version is a community modernization effort.

---

**⭐ Star this repo if you find it useful!**
