# 圖片全載Next Pro / Full Picture Load Next Pro v2026.4.0

> Modern image batch downloader supporting 1000+ sites, infinite scroll, ZIP packaging

## 📦 Installation

1. Install a userscript manager:
   - [Tampermonkey](https://www.tampermonkey.net/) (Chrome/Firefox/Edge)
   - [Violentmonkey](https://violentmonkey.github.io/) (Open source alternative)

2. Install the script:
   - Open `FullPictureLoad_Next_Pro_v2026.4.0.user.js` in this workspace
   - Copy the entire contents
   - Create new script in your userscript manager
   - Paste and save

## 🎯 Supported Sites (685+)

### Photo/Portfolio
- Pexels, Unsplash, Behance, ArtStation, DeviantArt, Pixiv, Wallhaven, AlphaCoders

### Manga/Comic
- MangaDex, MangaNato, MangaKakalot, Dynasty Reader, ManyToon, Toonily, Webtoon
- BiliBili Manga, 拷贝漫画, 漫画柜, 咚漫, LINE Webtoon

### NSFW (Adult)
- Cosplay sites (24cos, etc.)
- H-Comic platforms (18comic, Nhentai alternatives, etc.)

### Image Hosts
- Imgur, ImageBam, PostImg, ImageTwist, etc.

## 🚀 Features

| Feature | Description |
|---------|-------------|
| **Batch Download** | Download all images on a page as ZIP |
| **Infinite Scroll** | Auto-load next chapters/pages |
| **Gallery View** | Fancybox/ViewerJS integration |
| **Image Stitching** | Combine long images (manga mode) |
| **Queue Management** | PQueue-based download management |
| **Cross-site** | Universal pattern matching |

## ⚙️ Configuration

Click the userscript icon in your browser toolbar to access settings:

- **Threading**: Parallel download threads (default: 8)
- **ZIP Packaging**: Enable/disable ZIP compression
- **Auto-download**: Start downloads automatically
- **Comic Mode**: Optimized for manga reading
- **Gallery**: Enable Fancybox image viewer

## 🏗️ Architecture

```javascript
// Site registration format
this.register("site_id", 
  { 
    h: ["host.com"],           // Host patterns
    p: /^\/path\/\d+/,         // URL path regex
    e: "#element",             // Required element
    d: "pc|m"                  // Device type
  }, 
  async () => {
    // Extraction function
    return [
      { url: "...", filename: "...", thumb: "..." }
    ];
  }
);
```

## 🔄 Migration from Original FullPictureLoad

| Old | New |
|-----|-----|
| `customData` array | `SiteRouter.register()` calls |
| Mixed formats | Standardized extraction functions |
| Sync selectors | Async extraction support |
| Inline logic | Modular architecture |

## 🐛 Troubleshooting

**Script not running?**
- Check `@match` patterns in userscript settings
- Verify site URL matches registered patterns

**Images not loading?**
- Site may have updated their structure
- Check browser console for errors
- Report with site URL and expected behavior

**Download failures?**
- Increase retry count in settings
- Check if site requires authentication
- Some sites block cross-origin requests

## 📁 Build Information

- **Version**: 2026.4.0
- **Sites**: 685 unique registrations
- **Size**: ~302KB
- **Build Date**: 2026-04-12
- **Author**: Aura (based on 德克斯DEX)

## 📜 License

Original work by 德克斯DEX. This Pro version is a community modernization effort.

## 🙏 Credits

- Original FullPictureLoad by 德克斯DEX
- Fancybox v6 by FancyApps
- PQueue by Sindre Sorhus
- JSZip by Stuart Knightley
- Axios by Matt Zabriskie
