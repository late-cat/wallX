# Video Wallpaper for macOS (Plash)

A simple, minimal website template to use any video as your macOS wallpaper using [Plash](https://sindresorhus.com/plash).

![Demo](https://img.shields.io/badge/macOS-Wallpaper-blue)

## What You'll Get

- Full-screen video background
- Seamless looping
- No UI elements - just your video
- Optimized for Plash

## Quick Start

### 1. Clone This Repository
```bash
git clone https://github.com/late-cat/splash.git
cd splash
```

### 2. Add Your Video
- Place your video file in the project folder
- Rename it to **`video.webm`** OR **`video.mp4`**
- Supported formats: `.webm`, `.mp4`

### 3. Open in Plash
1. Open **Plash** app on your Mac
2. Click the **+** button to add a new website
3. Enter the file path:
   ```
   file:///ABSOLUTE/PATH/TO/splash/index.html
   ```
   Replace `ABSOLUTE/PATH/TO` with the actual path (e.g., `file:///Users/yourname/splash/index.html`)
4. Click **Done**

That's it! Your video is now your wallpaper.

## Customization

### Using a Different Video File
Edit `index.html` line 12:
```html
<source src="your-video-name.webm" type="video/webm">
```

### Changing Video Fit
Edit `style.css` line 20:
- `object-fit: cover;` - Fills screen (may crop)
- `object-fit: contain;` - Fits entire video (may show bars)

## Requirements

- **macOS** with [Plash](https://sindresorhus.com/plash) installed
- Video file in WebM or MP4 format
- Modern web browser support

## Tips

- **Video Quality**: 4K videos work great but use more resources
- **File Size**: Keep videos under 100MB for best performance
- **Format**: WebM is recommended for smaller file sizes
- **Compression**: Use Handbrake or ffmpeg to compress large videos

## Troubleshooting

**Video not playing?**
- Make sure the video path in `index.html` is correct
- Refresh Plash (click Revert, then Done)
- Check if the video plays in a regular browser first

**Black screen in Plash?**
- Verify the file path is absolute (starts with `file:///`)
- Make sure `style.css` is in the same folder as `index.html`

## File Structure

```
splash/
├── index.html      # Main HTML file
├── style.css       # Styling for full-screen video
├── video.webm      # Your video file (not included)
└── README.md       # This file
```

## License

MIT License - Feel free to use and modify!

## Credits

Created for easy video wallpapers on macOS using Plash.

---

**Enjoy your animated wallpaper!** 🎬
