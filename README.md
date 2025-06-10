# 🚀 Node.js Static File Server

A blazing-fast, minimal, and pure Node.js static file server.  
Serve your HTML, CSS, JS, and images with zero dependencies and full control over your server logic.

---

## ✨ Features

- **No Frameworks:** Built using only Node.js core modules (`http`, `fs`, `path`).
- **Smart Routing:** Serves `index.html` at root and any file in your project directory.
- **MIME Type Detection:** Handles `.html`, `.css`, `.js`, `.png` out of the box.
- **Custom Error Handling:** Clean 404 responses for missing files.
- **Ultra Lightweight:** Perfect for learning, prototyping, or as a foundation for bigger projects.

---

## 🛠️ How It Works

1. **Request Handling:**  
   The server listens on port `3000` and parses incoming requests to serve the correct file.

2. **Dynamic File Path Resolution:**  
   Uses `path.join` and `__dirname` to safely resolve file paths, preventing directory traversal attacks.

3. **MIME Type Mapping:**  
   Automatically sets the correct `Content-Type` header based on file extension.

4. **Error Handling:**  
   Responds with a custom 404 page if the file is not found.

---

## 🚦 Quick Start

```bash
git clone https://github.com/yourusername/node-static-server.git
cd node-static-server/Server
node server.js
```

- Place your static files (e.g., `index.html`, `style.css`, `script.js`, images) in the same directory as `server.js`.
- Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📁 Project Structure

```
Server/
  /public
  ├── script.js
  ├── index.html
  ├── style.css
  └── ... (other static files)
├── server.js

```

---

## 🧠 Code Highlights

- **Zero Dependencies:** No `npm install` required.
- **Easily Extendable:** Add more MIME types or custom routes as needed.
- **Console Logging:** See every file request in your terminal for easy debugging.

---

## 🚀 Future Enhancements

- [ ] Directory listing
- [ ] Gzip compression
- [ ] HTTPS support
- [ ] Caching headers
- [ ] Logging middleware

---

## 🤝 Contributing

Pull requests and suggestions are welcome!  
Feel free to fork this repo and make it your own.

---

## 📜 License

MIT License

---

> **Built with Node.js, curiosity, and a passion for clean code.**
