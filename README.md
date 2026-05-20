# 📖 AlatiphA EPUB — PWA EPUB Reader

A beautiful, offline-capable Progressive Web App for reading EPUB books — with full support for **interactive links**, **footnotes**, **table of contents**, and **reading preferences**.

## ✨ Features

- 📂 **Open any EPUB** via drag-and-drop or file picker
- 🔖 **Auto-saves reading position** per book (using IndexedDB + CFI)
- 📚 **Recent books library** — reopen books without re-uploading
- 📑 **Table of Contents** panel — tap any chapter to jump
- 💬 **Footnotes & endnotes** — tap a superscript to see the footnote in a popup
- 🔗 **Internal & external links** fully handled
- 🌙 **Dark / Sepia / Light themes**
- 🔤 **Adjustable font size, line spacing, font family**
- 📴 **Offline support** via Service Worker
- 📲 **Installable** as a PWA on mobile and desktop
- ⌨️ **Keyboard navigation** (← → arrow keys, Space)
- 👆 **Swipe navigation** on touch devices


### Install as PWA

- **Mobile (iOS)**: Open in Safari → Share → "Add to Home Screen"
- **Mobile (Android)**: Open in Chrome → browser menu → "Add to Home Screen" / "Install App"
- **Desktop**: Chrome/Edge will show an install icon in the address bar



## 📁 File Structure

```
folio-epub-reader/
├── index.html              # App shell
├── style.css               # All styles (themes, layout, components)
├── app.js                  # Main app logic
├── sw.js                   # Service Worker (offline support)
├── manifest.json           # PWA manifest
├── icon-192.png        # PWA icon
├── icon-512.png        # PWA icon
├── library/
│   ├── sample.epub      # PWA EPUB 
│   └── sample2.epub       # PWA EPUB 
└── .github/
    └── workflows/
        └── deploy.yml      # GitHub Pages auto-deploy
```

## 📝 EPUB Compatibility

Tested with:
- EPUB 2 and EPUB 3 files
- Books with footnotes (`epub:type="noteref"`, `role="doc-noteref"`, `#fragment` links)
- Books with internal chapter navigation
- Books with embedded images

---

## ⚙️ Customization

**Change default theme:** Edit `state.theme` in `app.js`  
**Change default font:** Edit `state.fontFamily` in `app.js`  
**Add more fonts:** Add to the Google Fonts link in `index.html` and the `<select>` in settings

---

## 📄 License

MIT — free to use, modify, and deploy.
