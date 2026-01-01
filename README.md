# 🎨 Prism.Tools

**Developer Utilities, Refined**

A collection of privacy-focused, client-side developer tools. No tracking, no ads, no server-side processing. Everything runs in your browser.

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://blgardner.github.io/prism.tools/)
[![License](https://img.shields.io/badge/License-Custom-blue.svg)](LICENSE)
[![Donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](https://www.paypal.com/paypalme/BLGApps)

## ✨ Features

- **Client-Side** - All processing happens in your browser
- **Privacy First** - No data collection, no tracking, no analytics
- **Always Free** - Free to use, online and local
- **38 Tools** - Constantly growing collection
- **Modern UI** - Clean, dark-themed interface
- **Keyboard Shortcuts** - Press `/` to search tools
- **Recent Tools** - Quick access to your last used tools
- **Mobile Friendly** - Responsive design for all devices

## 🛠️ Tool Categories

### 📋 Formatters & Parsers
- Code Formatter - Format & beautify code
- JSON Formatter - Format & validate JSON
- SQL Formatter - Format SQL queries
- YAML ↔ JSON Converter - Convert between YAML and JSON
- CURL to Fetch - Convert CURL commands to JavaScript

### 🔒 Security & Dev
- JWT Decoder - Decode JWT tokens
- Password Generator - Generate secure passwords
- Hash Generator - MD5, SHA-256, SHA-512
- UUID Generator - Generate UUIDs v1/v4
- Subnet Calculator - IP & network calculations

### 🎨 Visual & CSS
- SVG Editor - Create & edit SVG graphics
- CSS Gradient Generator - Create CSS gradients
- CSS Shadow Generator - Create box shadows
- Clip-path Maker - Create polygon clip-paths
- Glassmorphism Generator - Frosted glass effects
- Favicon Generator - Create favicons from text/images/emoji
- Color Converter - HEX, RGB, HSL converter
- Image Tools - Resize, convert images

### ✨ Generators & Content
- Lorem Ipsum - Generate placeholder text
- Random Data - Generate test data
- QR Code Generator - Generate QR codes
- ASCII Art Generator - Convert images/text to ASCII
- Slug Generator - Generate URL-safe slugs
- Meta Tag Generator - Generate SEO & Open Graph tags
- Robots.txt Generator - Generate robots.txt files

### 🔄 Encoders & Transformers
- Base64 - Encode/decode Base64
- URL Encoder - Encode/decode URLs
- HTML Encoder - Encode/decode HTML entities
- Case Converter - Convert text case
- String Escaper - Escape strings for multiple languages
- Minifier - Minify CSS/JS/HTML
- Timestamp Converter - Unix timestamp converter
- List Sorter - Sort & filter lists
- Unit Converter - Convert between units
- Regex Tester - Test regex patterns
- Diff Checker - Compare text differences
- Markdown Preview - Live markdown preview
- Cron Builder - Build cron expressions

## 🚀 Quick Start

### Option 1: Use Online
Visit [https://blgardner.github.io/prism.tools/](https://blgardner.github.io/prism.tools/)

### Option 2: Run Locally
```bash
# Clone the repository
git clone https://github.com/blgardner/prism.tools.git

# Navigate to directory
cd prism.tools

# Open in browser (no build step required!)
open index.html
# or
python -m http.server 8000
```

### Option 3: Deploy Your Own
Deploy to any static hosting provider:
- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages
- AWS S3 + CloudFront

Simply upload the files - no build process needed!

## 📁 Project Structure
```
prism.tools/
├── index.html              # Main landing page
├── tools/                  # Individual tool pages
│   ├── json-formatter.html
│   ├── base64.html
│   ├── jwt-decoder.html
│   └── ... (+35 more)
└── README.md
```

## 🎨 Adding a New Tool

Each tool is a standalone HTML file with embedded CSS and JavaScript:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Tool Name - Prism.Tools</title>
  <style>
    /* Tool-specific styles */
  </style>
</head>
<body>
  <nav class="navbar">
    <a href="../index.html" class="logo">PRISM</a>
    <a href="../index.html" class="back-link">← All Tools</a>
  </nav>
  
  <div class="container">
    <!-- Tool content -->
  </div>
  
  <script>
    // Tool logic
    function trackUsage() {
      let count = parseInt(localStorage.getItem('prism-usage-count') || '0');
      count++;
      localStorage.setItem('prism-usage-count', count);
    }
  </script>
</body>
</html>
```

Then add it to `index.html` in the `tools` array:
```javascript
{
  id: 'your-tool',
  name: 'Your Tool Name',
  icon: '🎯',
  description: 'Tool description',
  color: '#A78BFA',
  file: 'tools/your-tool.html',
  category: 'formatters' // or security, visual, generators, encoders
}
```

## 🎯 Design Principles

1. **Privacy First** - No external dependencies that track users
2. **Fast & Lightweight** - No frameworks, minimal JavaScript
3. **Accessible** - Works without JavaScript where possible
4. **Self-Contained** - Each tool is a single HTML file
5. **No Build Step** - Pure HTML/CSS/JS, deploy anywhere
6. **Consistent UX** - Unified dark theme across all tools

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Add New Tools** - See "Adding a New Tool" above
2. **Improve Existing Tools** - Bug fixes, feature additions
3. **Report Issues** - Found a bug? Open an issue
4. **Suggest Features** - Ideas for new tools or improvements
5. **Documentation** - Help improve the README

### Contribution Guidelines
- Keep tools self-contained (single HTML file)
- Follow the existing design patterns
- Test on multiple browsers
- No external dependencies that track users
- Use only free CDN resources (cdnjs.cloudflare.com)

## 💖 Support

If you find Prism.Tools useful, consider supporting development:

- ☕ [Donate via PayPal](https://www.paypal.com/paypalme/BLGApps)
- ⭐ Star this repository
- 🐦 Share on social media
- 🐛 Report bugs and suggest features

**Running costs:** $0/month (static hosting)  
**Your donations fund:** Development time and new features

## 📜 License

MIT License - see [LICENSE](LICENSE) file for details

## 🔗 Links

- **Live Demo:** [https://blgardner.github.io/prism.tools/](https://blgardner.github.io/prism.tools/)
- **GitHub:** [https://github.com/blgardner/prism.tools](https://github.com/blgardner/prism.tools)
- **Donate:** [https://www.paypal.com/paypalme/BLGApps](https://www.paypal.com/paypalme/BLGApps)

## 🙏 Acknowledgments

Built with:
- Pure HTML, CSS, and JavaScript
- No frameworks or build tools
- CDN resources from [cdnjs.cloudflare.com](https://cdnjs.cloudflare.com)
- Icons from Unicode emoji

Special thanks to all contributors and supporters! 💜

---

Made with 💜 by developers, for developers

*Privacy-focused • Ad-free • Open source*
