# BoringManager

<img width="1366" height="685" alt="image" src="https://github.com/user-attachments/assets/5ae2f26e-13d8-47d8-8d8c-0741777660c9" />

A lightweight, dependency-free, single-file PHP file manager packed into **1 line of code**.

---

## 📋 Requirements

- **PHP Version:** **PHP 5.3+** *(Fully compatible with PHP 5.3, 5.4, 5.5, 5.6, 7.x, and 8.x)*
- **PHP Extensions:**
  - `php-zip` *(Optional, required for creating and extracting `.zip` archives)*
  - `php-session` *(Standard in most PHP installations)*

---

## ✨ Features

- **Packed in 1 Line of Code:** Entire backend, frontend, and scripts bundled into a single line.
- **Zero CSS / Lightweight:** Pure standard HTML without external stylesheets or bloated frameworks.
- **Multi-Select & Batch Actions:**
  - Checkboxes on all items with a master **Select All** toggle.
  - **Shift + Click** support to select a range of items in one click.
  - Batch **Delete Selected** and **Zip Selected**.
- **Smooth Audio & Video Streaming:**
  - Full HTTP 206 Partial Content (byte-range) support.
  - Fast, unfreezing seeking/scrubbing across audio and video timelines without session locking.
- **Fit-to-Screen Media Previews:** Responsive viewer automatically scales images, audio, videos, and PDFs to fit your screen/viewport.
- **Chunked File Upload:** Upload large files reliably in 2 MB slices with real-time percentage progress.
- **File Operations:** Create files and folders, rename, delete, and view metadata (permissions, sizes, recursive counts).
- **In-Browser Code/Text Editor:** Edit text/code files directly from your browser with instant save notifications.
- **Archive Support:** Create and extract `.zip` files on the fly.
- **Recursive Search & Breadcrumbs:** Instant recursive file/folder search across all nested subdirectories.
- **Master Password Protection:** Optional authentication lock to secure access.

---

## 🚀 Quick Start

1. Copy the code into an `index.php` file (or any `.php` file on your server).
2. *(Optional)* Set a master password by editing `$AUTH_PASSWORD='your_password';` near the beginning of the file.
3. Open the file in your web browser.

---

## ⚙️ Configuration

| Variable | Default | Description |
|---|---|---|
| `$AUTH_PASSWORD` | `''` | Set a password string to require login before accessing files. Leave empty `''` to disable login. |
| `FM_ROOT_PATH` | `realpath(__DIR__)` | Root directory path that BoringManager is allowed to manage (prevents directory traversal outside root). |
