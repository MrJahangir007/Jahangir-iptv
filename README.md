# 📡 Jahangir IPTV

> **World Best IPTV Player** — Full-featured web-based IPTV player with instant channel switching, multiple proxy fallback, and support for M3U playlists.

![Jahangir IPTV](https://img.shields.io/badge/Version-21.0-gold?style=flat-square&logo=github)
![HTML](https://img.shields.io/badge/HTML-100%25-orange?style=flat-square&logo=html5)
![HLS.js](https://img.shields.io/badge/HLS.js-Latest-blue?style=flat-square&logo=javascript)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## 🌟 Features

| Feature | Description |
|---------|-------------|
| **📺 100+ Embedded Channels** | Pre-loaded Bangladeshi, Sports, FIFA, and International channels |
| **⚡ Instant Channel Switching** | Click any channel — it plays immediately, no waiting |
| **🔄 Multi-Proxy Fallback** | 4 different proxies (corsproxy.io, allorigins.win, cors-anywhere, cors.sh) |
| **🎯 Smart Channel Grouping** | Same-name channels (like T Sports) are grouped with multi-URL fallback |
| **🔑 Xtream Login Support** | Enter Server/User/Password to load Xtream Codes playlists |
| **📂 Playlist Manager** | Tivimate-style playlist management — add/remove playlists easily |
| **🔗 M3U Support** | Load any M3U/M3U8 URL or upload local `.m3u` files |
| **🏆 FIFA World Cup 2026** | Dedicated category for all FIFA matches & channels |
| **⚽ Match Schedule** | Live match updates with scores and standings |
| **📊 Group Standings** | Group-wise points table with qualification indicators |
| **🎮 Keyboard Shortcuts** | Space (play/pause), ←/→ (seek), ↑/↓ (volume), F (fullscreen), P (PiP), M (mute) |
| **📱 Fully Responsive** | Works on mobile, tablet, desktop, and TV |
| **🖼️ PiP Support** | Picture-in-Picture mode for multitasking |

---

## 🚀 Quick Start

### Option 1: Use the Live Demo
Simply open the HTML file in any modern browser.

### Option 2: Host on GitHub Pages
1. Fork this repository
2. Go to Settings → Pages
3. Select `main` branch and `/ (root)` folder
4. Your player will be live at `https://your-username.github.io/Jahangir-iptv/`

### Option 3: Local Usage
1. Download the `index.html` file
2. Double-click to open in browser
3. No server required — works offline with embedded channels

---

## 📂 Playlist Management

The player includes a Tivimate-style playlist manager:

| Playlist | Description |
|----------|-------------|
| **Local** | Pre-embedded channels (100+ working channels) |
| **15k+ Playlists** | Load from 6+ public M3U sources |
| **M3U Import** | Upload your own `.m3u` or `.m3u8` files |
| **Xtream** | Enter Server URL, Username, Password to load Xtream Codes |

### How to Add Your Own Playlist:
1. Paste your M3U URL in the input field
2. Click **"📥 Load"**
3. Or click **"📂 File"** to upload a local `.m3u` file
4. Or click **"🔑 Xtream"** to login with Server/User/Pass

---

## 🛠️ Technical Details

### Proxy System
```javascript
const PROXIES = [
    'https://corsproxy.io/?',
    'https://api.allorigins.win/raw?url=',
    'https://cors-anywhere.herokuapp.com/',
    'https://proxy.cors.sh/'
];
Smart Channel Grouping
Channels with the same tvg-name are grouped together

Multiple URLs for the same channel are tried sequentially until one works

Perfect for services like T Sports with multiple server URLs

Xtream Codes Support
The player supports Xtream Codes format:

text
http://SERVER:PORT/get.php?username=USER&password=PASS&type=m3u_plus&output=ts
Simply use the 🔑 Xtream button in the toolbar to enter your credentials.

HLS.js Configuration
Optimized for low latency and smooth playback:

Manifest timeout: 60s

Max retries: 5

Fragments timeout: 30s

Backbuffer: 30s (smooth mode)

📋 Channel Categories
Category	Description
🏆 FIFA WC 26	All FIFA World Cup 2026 channels
📺 All Channels	Complete channel list
🇧🇩 BD Channels	Bangladeshi channels (NTV, Jamuna, Channel i, etc.)
⚽ Sports	Sports channels (T Sports, BeIN, Fox, etc.)
⚽ Matches	Live match schedule & scores
📊 Standings	Group-wise points table
🔧 How to Update Channels
Method 1: Update playlist.m3u8 (Recommended)
Edit playlist.m3u8 file in this repository

Add or remove channels in standard M3U format

Commit changes — the player will auto-load them

Method 2: Edit Embedded Channels
Open index.html

Find FULL_CHANNELS array

Add/modify channels in this format:

javascript
{ name: "Channel Name", url: "https://example.com/stream.m3u8", group: "Sports", flag: "⚽" }
Method 3: Use External URL
Paste any M3U URL in the input field

Click Load

📊 Channel Status Indicators
Color	Status
🟢 Green	Channel is working
🔴 Red	Channel failed to load
⚪ Gray	Channel not yet tested
⌨️ Keyboard Shortcuts
Key	Action
Space	Play/Pause
← →	Seek backward/forward 10 seconds
↑ ↓	Volume up/down
F	Fullscreen
P	Picture-in-Picture (PiP)
M	Mute/Unmute
📱 Mobile Support
Fully responsive design

Touch-friendly channel grid

Swipe to scroll channels

Landscape mode optimized

Mobile-optimized controls

🐛 Troubleshooting
Channels not loading?
Refresh the page (Ctrl+F5)

Check your internet connection

Try VPN (some streams are geo-blocked)

Click "▶️ Auto" button — it will skip dead channels

Enable "🐢 Smooth" mode for slow networks

"Failed to fetch" error?
The proxy server might be down

Wait a moment and try again

The player will auto-switch to the next proxy

Video lag or buffering?
Enable "🐢 Smooth" mode

Lower video quality (select 480p or 360p)

Close other bandwidth-heavy applications

Xtream not working?
Make sure Server URL includes the port (e.g., http://86.107.179.250:80)

Check Username and Password are correct

Try loading the M3U URL directly in the input field

🤝 Contributing
Fork the repository

Create your feature branch (git checkout -b feature/amazing-feature)

Commit your changes (git commit -m 'Add some amazing feature')

Push to the branch (git push origin feature/amazing-feature)

Open a Pull Request

📝 License
This project is licensed under the MIT License — see the LICENSE file for details.

🙏 Acknowledgments
HLS.js — HLS playback engine

Font Awesome — Icons

Google Fonts — Inter font

📞 Contact
Developer: Md Jahangir Alam

Facebook: MrJahangir007

Telegram: iammrjahangir

Email: mrjahangiralam007@gmail.com

⭐ Support
If you find this project useful, please give it a ⭐ on GitHub!

https://img.shields.io/github/stars/MrJahangir007/Jahangir-iptv?style=social
https://img.shields.io/github/forks/MrJahangir007/Jahangir-iptv?style=social

Made with ❤️ by Md Jahangir Alam
