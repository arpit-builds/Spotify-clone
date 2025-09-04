# Spotify Clone - Web Music Player

A Spotify-inspired web music player supporting dynamic album and playlist browsing, music playback controls, and a responsive UI. This project is a front-end clone built using HTML, CSS, and JavaScript.

---

## Project video
https://github.com/user-attachments/assets/f3ab2fb1-ecbb-48d0-946e-db196f804fcf

## Features
- **Spotify-like UI**: Mimics the modern look and feel of Spotify's web player.
- **Dynamic Song/Album Listing**: Fetches albums and songs from a specified server directory.
---
- **Full Playback Controls**: Play, pause, next, previous, seek, and volume adjustment.
- **Responsive Navigation**: Hamburger menu and sidebar expand/collapse for easy browsing.
- **Track Information**: Displays current song/info and updates playback progress in real time.
- **Volume Control & Mute**: Adjust or mute playback volume interactively.

---

## Getting Started

### Prerequisites
- Local/remote web server capable of serving song directories and JSON album info (see below).
- Modern web browser (Chrome, Firefox, Edge, etc.).

### Folder Structure
```
project-root/
├── spotify.html
├── js/
│   └── script.js
├── css/
│   ├── style.css
│   └── utility.css
├── img/
│   └── [SVG, logos, controls, thumbnails]
├── songs/
│   └── [albums]/
│       ├── cover.jpg
│       ├── info.json
│       └── [song].mp3
└── README.md
```

### Album Format
Each album is a folder under `songs/`, containing:
- `cover.jpg`: Album cover image
- `info.json`: Album metadata (`title`, `description`)
- `.mp3` files: Songs belonging to the album

Example `info.json`:
```json
{
  "title": "Album Name",
  "description": "Short description of the album."
}
```

### Setup & Usage
1. Start a local HTTP server in the root project directory. (e.g., with Python: `python -m http.server 3000`)
2. Ensure albums are placed under the `songs/` directory in the required structure (see above).
3. Open `spotify.html` in your browser, or navigate to `http://localhost:3000/spotify.html`.
4. Browse albums, click to view and play songs, use the playback controls.

**Note:** The JavaScript fetches songs using an IP and port (`http://192.168.1.9:3000/...`). For local use, update these URLs in `js/script.js` to match your server address (e.g., `http://localhost:3000/`).

---

## Customization
- Update styles in `css/style.css` and `css/utility.css`.
- Replace images in `img/` with your preferred icons and logos.
- Add new albums/songs by placing them in the appropriate directory structure.

---

## Credits
This project is for educational purposes learned form CodeWithHarry. It is not affiliated with or endorsed by Spotify.
