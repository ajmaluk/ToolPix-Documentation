# ToolPix – AI-Powered Productivity Platform

[![Live Platform](https://img.shields.io/badge/Platform-Live-brightgreen?style=for-the-badge&logo=googlechrome)](https://toolpix.pythonanywhere.com/)
[![License](https://img.shields.io/badge/Source-Proprietary%20%2F%20Closed--Source-red?style=for-the-badge)](https://toolpix.pythonanywhere.com/terms)
[![Python](https://img.shields.io/badge/Backend-Python%20%7C%20Flask-blue?style=for-the-badge&logo=python)](https://toolpix.pythonanywhere.com/about)
[![AI Integration](https://img.shields.io/badge/AI-Gemini%20%26%20NVIDIA-purple?style=for-the-badge&logo=google)](https://toolpix.pythonanywhere.com/aistudio)

> 🔒 **Notice:** **ToolPix** is a proprietary, closed-source project. This repository (**[ToolPix-Documentation](https://github.com/ajmaluk/ToolPix-Documentation)**) serves as the official public documentation hub, platform feature showcase, and technical architecture reference. The internal backend source code and underlying implementation files are private and not publicly available.

---

## 🌐 Live Web Application

Experience the full collection of intelligent productivity tools live on the web:

➡️ **[https://toolpix.pythonanywhere.com/](https://toolpix.pythonanywhere.com/)**

---

## 🚀 Overview

**ToolPix** is a production-ready, unified AI-powered productivity platform designed to streamline daily workflows for developers, content creators, students, and professionals. 

Instead of switching across multiple isolated web apps, **ToolPix** consolidates Next-Gen AI capabilities, multi-language online compilers, document processing, image manipulation, and developer utilities into a single, cohesive, high-performance web interface.

---

## 🛠️ Architecture & Technical Stack

ToolPix is built with a modular, highly scalable web architecture designed for security, rapid page loads, and seamless user interaction.

```text
                               ┌───────────────────────────┐
                               │   User / Web Browser      │
                               └─────────────┬─────────────┘
                                             │
                                             ▼
                               ┌───────────────────────────┐
                               │  Frontend Interface       │
                               │  HTML5 / CSS3 / ES6 JS    │
                               │  Monaco & CodeMirror IDEs │
                               └─────────────┬─────────────┘
                                             │ HTTPS
                                             ▼
                               ┌───────────────────────────┐
                               │  Flask Application Backend│
                               │  Blueprint Modular Router │
                               │  Canonical URL Engine     │
                               └─────────────┬─────────────┘
                                             │
       ┌────────────────────┬────────────────┼────────────────────┬────────────────────┐
       ▼                    ▼                ▼                    ▼                    ▼
┌──────────────┐    ┌──────────────┐  ┌──────────────┐    ┌──────────────┐    ┌──────────────┐
│  AI Studio   │    │   Online     │  │  PDF & Doc   │    │ Image & OCR  │    │ Developer &  │
│ Gemini &     │    │  Compilers   │  │  Engine      │    │  Engine      │    │  Utility     │
│ NVIDIA APIs  │    │ (Sandbox API)│  │ (PyPDF/PyMu) │    │ (Pillow/Tess)│    │  Suite       │
└──────────────┘    └──────────────┘  └──────────────┘    └──────────────┘    └──────────────┘
       │                    │                │                    │                    │
       └────────────────────┴────────────────┼────────────────────┴────────────────────┘
                                             ▼
                               ┌───────────────────────────┐
                               │  SQLite & WSGI Host       │
                               │  PythonAnywhere Server    │
                               └───────────────────────────┘
```

### Stack Details
- **Backend:** Python 3, Flask Framework, Modular Blueprint Architecture, RESTful Services.
- **Frontend:** Responsive HTML5, Vanilla CSS3 (Custom Design System with Dark Mode & Glassmorphism), Vanilla JavaScript (ES6+), Monaco Editor & CodeMirror for web-based IDEs.
- **AI Integrations:** Google Gemini API & NVIDIA AI Services powering text generation, image synthesis, intelligent code creation, and audio/voice capabilities.
- **Processing Engines:** PyPDF, `pdfplumber`, `pdf2image`, Tesseract OCR, Pillow (PIL), OpenCV, Client-side Canvas API.
- **Database & Services:** SQLite for ratings and telemetry; isolated code execution sandbox with key-authenticated endpoints.
- **Deployment:** PythonAnywhere cloud infrastructure with strict SSL enforcement, automated canonical URL normalization, rate limiting, and dynamic XML sitemap generation.

---

## 🌟 Feature Modules & Platform Tools

ToolPix hosts an extensive catalog of web tools organized into 6 core categories:

### 1. 🤖 [AI Studio](https://toolpix.pythonanywhere.com/aistudio)
Suite of generative AI utilities for creation, coding, and assistant workflows:
- **[AI Text Chat](https://toolpix.pythonanywhere.com/aistudio/text-chat):** Conversational AI assistant for research, brainstorming, and writing.
- **[AI Image Generator](https://toolpix.pythonanywhere.com/aistudio/image-generator):** Generate high-quality visual artwork from text prompts.
- **[AI Website Builder](https://toolpix.pythonanywhere.com/aistudio/website-builder):** Instantly generate responsive HTML/CSS website projects from text descriptions.
- **[AI Resume Builder](https://toolpix.pythonanywhere.com/aistudio/resume-builder):** Craft professional, resume templates enhanced with AI content suggestions.
- **[AI Code Generator](https://toolpix.pythonanywhere.com/aistudio/code-generator):** Generate clean code snippets, functions, and algorithms across 15+ languages.
- **[AI Content Writer](https://toolpix.pythonanywhere.com/aistudio/content-writer):** Draft articles, blog posts, emails, and marketing copy automatically.
- **[AI Grammar Fixer](https://toolpix.pythonanywhere.com/aistudio/grammar-fixer):** Proofread and refine writing tone, spelling, and sentence structures.
- **[AI Voice Studio](https://toolpix.pythonanywhere.com/aistudio/voice-studio):** Convert text to natural speech audio with multi-voice synthesis.
- **[AI Audio Editor](https://toolpix.pythonanywhere.com/aistudio/audio-editor):** Edit, transcribe, and enhance audio recordings online.

---

### 2. ⚡ [AI Online Compilers & IDEs](https://toolpix.pythonanywhere.com/ai-online-compilers)
Cloud-based code editors with syntax highlighting, live previews, and instant execution:
- **[Python Online Compiler](https://toolpix.pythonanywhere.com/compiler/python):** Run Python scripts directly in the browser.
- **[C Online Compiler](https://toolpix.pythonanywhere.com/compiler/c):** Compile and debug standard C code.
- **[C++ Online Compiler](https://toolpix.pythonanywhere.com/compiler/cpp):** Execute C++17/20 programs with stdout feedback.
- **[Java Online Compiler](https://toolpix.pythonanywhere.com/compiler/java):** Build and execute Java classes instantly.
- **[Go Online Compiler](https://toolpix.pythonanywhere.com/compiler/go):** Compile Golang programs in real-time.
- **[Rust Online Compiler](https://toolpix.pythonanywhere.com/compiler/rust):** Run safe, fast Rust code online.
- **[JavaScript Playground](https://toolpix.pythonanywhere.com/compiler/javascript):** Test Node.js & browser JavaScript snippets.
- **[React Online IDE](https://toolpix.pythonanywhere.com/compiler/react):** Interactive browser environment for building React components with live preview.
- **[SQL Compiler & Playground](https://toolpix.pythonanywhere.com/compiler/sql):** Execute SQL queries against instant in-memory relational databases.
- **[HTML/CSS Live Editor](https://toolpix.pythonanywhere.com/compiler/html):** Real-time web playground with instantaneous visual output.
- **[Bash Script Runner](https://toolpix.pythonanywhere.com/compiler/bash):** Execute Linux shell scripts safely.
- **[PHP Compiler](https://toolpix.pythonanywhere.com/compiler/php):** Test PHP scripts directly online.
- **[Kotlin Compiler](https://toolpix.pythonanywhere.com/compiler/kotlin):** Run Kotlin code snippets online.
- **[Swift Compiler](https://toolpix.pythonanywhere.com/compiler/swift):** Test Swift language syntax online.
- **[Perl Compiler](https://toolpix.pythonanywhere.com/compiler/perl):** Run Perl scripts in the browser.
- **[LaTeX Editor](https://toolpix.pythonanywhere.com/latex-editor):** Write and render mathematical LaTeX documents with live visual preview.
- **[Markdown Editor](https://toolpix.pythonanywhere.com/markdown-editor):** Write GitHub-Flavored Markdown with side-by-side rendering.

---

### 3. 📄 [PDF Processing Suite](https://toolpix.pythonanywhere.com/pdf-tools)
Complete online PDF utility library for document management and conversion:
- **[Merge PDF](https://toolpix.pythonanywhere.com/pdf-tools/merge-pdf):** Combine multiple PDF documents into a single file.
- **[Split PDF](https://toolpix.pythonanywhere.com/pdf-tools/split-pdf):** Extract specific page ranges or split PDFs into individual pages.
- **[Compress PDF](https://toolpix.pythonanywhere.com/pdf-tools/compress-pdf):** Reduce PDF file size without sacrificing quality.
- **[PDF Editor & OCR](https://toolpix.pythonanywhere.com/pdf-tools/pdf-editor-ocr):** Edit PDF text and extract searchable text using Optical Character Recognition.
- **[Protect PDF](https://toolpix.pythonanywhere.com/pdf-tools/protect-pdf):** Encrypt PDFs with secure passwords.
- **[Unlock PDF](https://toolpix.pythonanywhere.com/pdf-tools/unlock-pdf):** Remove password protection from PDFs.
- **[Rotate PDF](https://toolpix.pythonanywhere.com/pdf-tools/rotate-pdf) & [Organize PDF](https://toolpix.pythonanywhere.com/pdf-tools/organize-pdf):** Reorder, rotate, or delete pages inside PDFs.
- **[Redact PDF](https://toolpix.pythonanywhere.com/pdf-tools/redact-pdf):** Black out sensitive confidential text and images permanently.
- **AI PDF Converters:**
  - [PDF to Word Converter](https://toolpix.pythonanywhere.com/pdf-tools/ai-pdf-to-word) | [Word to PDF Converter](https://toolpix.pythonanywhere.com/pdf-tools/ai-word-to-pdf)
  - [Excel to PDF Converter](https://toolpix.pythonanywhere.com/pdf-tools/ai-excel-to-pdf) | [PDF to Excel Converter](https://toolpix.pythonanywhere.com/pdf-tools/pdf-to-excel)
  - [PPT to PDF Converter](https://toolpix.pythonanywhere.com/pdf-tools/ai-ppt-to-pdf) | [PDF to PPT Converter](https://toolpix.pythonanywhere.com/pdf-tools/pdf-to-ppt)
  - [Image to PDF Converter](https://toolpix.pythonanywhere.com/pdf-tools/image-to-pdf) | [PDF to Image / JPG](https://toolpix.pythonanywhere.com/pdf-tools/pdf-to-image)
  - [HTML to PDF Converter](https://toolpix.pythonanywhere.com/pdf-tools/html-to-pdf)

---

### 4. 🎨 [Image Processing & Graphics](https://toolpix.pythonanywhere.com/image-tools)
Fast web-based graphics tools, converters, and photo manipulation utilities:
- **[Advanced Photo Editor](https://toolpix.pythonanywhere.com/image-editor/advanced):** Browser-based photo editor with layers, adjustments, and crop tools.
- **[Background Remover](https://toolpix.pythonanywhere.com/image-editor/background-remover):** AI-powered automatic background removal for photos.
- **[Image Compressor](https://toolpix.pythonanywhere.com/image-editor/compressor):** Compress PNG, JPG, and WebP images efficiently.
- **[Image Resizer](https://toolpix.pythonanywhere.com/image-editor/resizer) & [Cropper](https://toolpix.pythonanywhere.com/image-editor/cropper):** Change dimensions or extract regions with aspect ratio locking.
- **[Image Filters](https://toolpix.pythonanywhere.com/image-editor/filters):** Apply visual filters, dark mode conversion, and artistic effects.
- **[SVG Optimizer](https://toolpix.pythonanywhere.com/image-editor/svg-optimizer):** Minify vector SVG graphics for faster web rendering.
- **[OCR Text Extractor](https://toolpix.pythonanywhere.com/image-editor/ocr):** Extract raw text from images, screenshots, and scanned documents.
- **[Name in Landsat](https://toolpix.pythonanywhere.com/name-in-landsat):** Spell out words using real NASA satellite photography of Earth features.
- **Format Converters:** PNG to JPG, JPG to WebP, Image to Base64, Steganography, Collage Maker, Favicon Maker.

---

### 5. 🛠️ [Developer & Coding Utilities](https://toolpix.pythonanywhere.com/coding-tools)
Essential web tools for developers, system administrators, and web designers:
- **[JSON Formatter & Validator](https://toolpix.pythonanywhere.com/free-online-json-formatter):** Format, validate, fix, and minify JSON data.
- **[Base64 Encoder / Decoder](https://toolpix.pythonanywhere.com/free-online-base64-encoder):** Convert text or binaries into Base64 format and back.
- **[JavaScript Obfuscator](https://toolpix.pythonanywhere.com/free-online-js-obfuscator):** Protect JS source code with code obfuscation algorithms.
- **[CSS Obfuscator](https://toolpix.pythonanywhere.com/free-online-css-obfuscator):** Minify and obscure CSS stylesheet rules.
- **[Regex Tester & Debugger](https://toolpix.pythonanywhere.com/free-online-regex-tester):** Test regular expression match patterns in real-time.
- **[SQL Formatter](https://toolpix.pythonanywhere.com/free-online-sql-formatter):** Format and beautify complex SQL queries.
- **[XML Beautifier](https://toolpix.pythonanywhere.com/free-online-xml-beautifier):** Format and indent structured XML documents.
- **[HTML Encoder / Decoder](https://toolpix.pythonanywhere.com/free-online-html-encoder-decoder):** Encode special characters for web safety.
- **[Code Diff Tool](https://toolpix.pythonanywhere.com/free-online-code-diff-tool):** Compare code snippets side-by-side to highlight differences.

---

### 6. 🧰 [General Productivity & Daily Utilities](https://toolpix.pythonanywhere.com/utility-tools)
Handy tools to increase daily productivity:
- **[Temp Mail Generator](https://toolpix.pythonanywhere.com/temp-mail):** Create temporary disposable email addresses with passwords for online registrations.
- **[QR Code Generator](https://toolpix.pythonanywhere.com/convert-url-to-qr-code-online):** Convert URLs and text into downloadable QR codes.
- **[QR Code Scanner](https://toolpix.pythonanywhere.com/convert-qr-to-url-online):** Decode QR code images uploaded or captured via webcam.
- **[Password Generator](https://toolpix.pythonanywhere.com/free-online-password-generator):** Create strong, cryptographically secure passwords.
- **[Kanban Board](https://toolpix.pythonanywhere.com/free-online-kanban-board):** Visual task management board stored locally in browser.
- **[Day Planner](https://toolpix.pythonanywhere.com/free-online-day-planner):** Schedule daily tasks and hourly routines.
- **[Pomodoro Timer](https://toolpix.pythonanywhere.com/free-online-pomodoro-timer):** Boost focus using structured work/break interval timers.
- **[Typing Speed Test](https://toolpix.pythonanywhere.com/free-online-typing-speed-test):** Measure Words Per Minute (WPM) and typing accuracy.
- **[Color Picker & Palette](https://toolpix.pythonanywhere.com/free-online-color-picker):** Extract HEX, RGB, and HSL color values with ease.

---

## 📌 Important Links & Information

- 🔗 **Main Platform:** [https://toolpix.pythonanywhere.com/](https://toolpix.pythonanywhere.com/)
- 📖 **Documentation:** [ToolPix Documentation](https://toolpix.pythonanywhere.com/documentation)
- ℹ️ **About ToolPix:** [About Us](https://toolpix.pythonanywhere.com/about) | [Features](https://toolpix.pythonanywhere.com/features)
- 📚 **Guides & Blog:** [User Guides](https://toolpix.pythonanywhere.com/guides) | [Official Blog](https://toolpix.pythonanywhere.com/blog/)
- 🔒 **Security & Terms:** [Security Overview](https://toolpix.pythonanywhere.com/security) | [Terms of Service](https://toolpix.pythonanywhere.com/terms) | [Privacy Policy](https://toolpix.pythonanywhere.com/privacy)
- 💬 **Support & Feedback:** [Help Center](https://toolpix.pythonanywhere.com/help-center) | [Contact Us](https://toolpix.pythonanywhere.com/contact) | [Feedback](https://toolpix.pythonanywhere.com/feedback)
- 🟢 **System Status:** [Live Service Status](https://toolpix.pythonanywhere.com/status)

---

## ⚖️ License & Proprietary Rights

© **ToolPix**. All rights reserved.

ToolPix is a proprietary software product. The source code, application assets, designs, backend APIs, and underlying implementations are strictly private and closed-source. 

This repository ([`ajmaluk/ToolPix-Documentation`](https://github.com/ajmaluk/ToolPix-Documentation)) is provided for public reference, architectural overview, and feature documentation purposes only. No part of the proprietary platform codebase may be reproduced, distributed, reverse engineered, or cloned without prior written permission.
