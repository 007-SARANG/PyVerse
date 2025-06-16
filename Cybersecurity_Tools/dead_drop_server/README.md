# 🕵️ WhisperNode – Offline LAN File Drop Server

**WhisperNode** is a lightweight, Flask-based file drop server designed for secure and private file sharing over a local network. It operates completely offline, making it ideal for isolated environments, secure labs, or CTF-style dead drops.

---

## 🚀 Features

- 📡 LAN-only operation — no internet required  
- 📁 Files stored in a `/drops` folder — not directly accessible by the host due to encrpytion
- 🔒 Web UI for uploads and secure delivery  
- 🧠 Creates a log of activity for auditing  
- 💣 Support for self-destructing files (self destructs in 10 minutes or after pick-up)  
- 🧊 Clean HTML/CSS frontend, minimal and functional

---

## 📁 Project Structure
```
whispernode/
├── backend/
│   ├── drops/           # Secure file storage (not exposed, created automatically)
│   └── main.py          # Flask backend logic
├── frontend/
│   ├── static/
│   │   └── style.css    # Styling for web interface
│   └── templates/
│       ├── index.html   # Upload page
│       └── success.html # Confirmation page
└── README.md
```
## 🔐 Notes

- Files are **not accessible by direct link** — they're kept in a secure backend folder.
- A simple **log file** is maintained to record upload events and metadata.
- Designed for **offline-first security** and simplicity.

---

## 👨‍💻 Author

Contributed by @varun935 as part of **Social Summer of Code Season 4 (SSoC 4)**.

---

## 📜 License

MIT License — free to use, modify, and share.
```
