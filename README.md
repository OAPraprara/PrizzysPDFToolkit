# PDF Toolkit

A lightweight, browser-based PDF editor that works entirely client-side. No uploads, no servers - your files never leave your computer.

![PDF Toolkit](https://img.shields.io/badge/PDF-Toolkit-red?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

## ✨ Features

### 📝 Edit PDF - Remove Pages
- Upload any PDF and visually select pages to remove
- Click thumbnails to mark pages for deletion
- Download the edited PDF instantly

### ✂️ Extract Pages
- Select specific pages to keep from a PDF
- Use page range input (e.g., `1-10, 15, 20-25`) for precise selection
- Preview extracted result before downloading
- **Handles large PDFs** (800+ pages) with multiple fallback methods

### 🔗 Merge PDFs
- Combine multiple PDF files into one
- Drag and drop to reorder files
- Works with any number of files

## 🚀 Live Demo

Simply open `pdfToolv1.html` in any modern browser - no installation required!

Or deploy to GitHub Pages for online access.

## 💻 Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/OAPraprara/pdf-toolkit.git
   ```

2. Open `pdfToolv1.html` in your browser

3. That's it! No build steps, no dependencies to install.

## 🔧 Technical Details

### Libraries Used
- **[PDF-lib](https://pdf-lib.js.org/)** - PDF creation and modification
- **[PDF.js](https://mozilla.github.io/pdf.js/)** - PDF rendering for thumbnails
- **[Tailwind CSS](https://tailwindcss.com/)** - Styling
- **[Download.js](https://github.com/rndme/download)** - File downloads

### Large PDF Handling

The toolkit uses a robust 4-level fallback system for extracting pages from problematic PDFs:

1. **Chunked Copy** - Fast batch copying (works for most PDFs)
2. **Single-page Copy** - One page at a time with error recovery
3. **Page Embedding** - Embeds pages as XObjects
4. **Canvas Rasterization** - Renders pages as images (handles severely corrupted PDFs)

## 📋 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Edge
- ✅ Safari

## 🔒 Privacy

**100% Client-Side** - All processing happens in your browser. Your PDFs are never uploaded to any server.

## 📄 License

MIT License - feel free to use, modify, and distribute.

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests

---

Made with ❤️ for the PDF editing community

