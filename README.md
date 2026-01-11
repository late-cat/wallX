# wallX - Video Wallpaper for macOS

A simple template to use any video as your macOS wallpaper using [Plash](https://sindresorhus.com/plash) ([App Store](https://apps.apple.com/in/app/plash/id1494023538?mt=12)).

## Quick Start

### 1. Clone This Repository
```bash
git clone https://github.com/late-cat/splash.git wallX
cd wallX
```

### 2. Add Your Video
- Place your video file in the `wallX` folder
- Rename it to **`video.webm`** or **`video.mp4`**

### 3. Set Up in Plash
1. Click the **Plash icon** in the menu bar
2. Click **"Add Website..."**
3. Click **"Local Website..."** button
4. Navigate to the `wallX` folder and select it
5. Click **"Choose"**

Done! Your video is now your wallpaper. 🎉

## Customization

### Video Fit Options
Edit `style.css` line 21:
- `object-fit: cover;` — Fills entire screen (may crop edges)
- `object-fit: contain;` — Shows full video (may have bars)

## Tips

- **Recommended format**: WebM (smaller file size)
- **Also works with**: MP4
- **For best results**: Use videos that loop seamlessly

## Troubleshooting

**Video not playing?**
- Make sure video is named `video.webm` or `video.mp4`
- Refresh: Click Plash icon → "Websites..." → Select yours → "Revert"

**Black screen?**
- Check the video plays in a browser first
- Verify video is in the same folder as `index.html`

## File Structure

```
splash/
├── index.html    # Main file (Plash loads this)
├── style.css     # Video styling
├── video.webm    # Your video (add this)
└── README.md
```

## License

MIT — Use freely!

---

Made by [late-cat](https://github.com/late-cat) 🐱
