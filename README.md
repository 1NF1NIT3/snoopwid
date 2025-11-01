# Music Widget 🎵

A beautiful, minimal music widget with vinyl visualization that works on desktop (Electron) and mobile (PWA + Native Widgets).

## Features

- 🎨 **Themed UI** - Multiple beautiful themes (GLUE Song, Anything)
- 🎵 **Music Playback** - Play/pause controls with offline support
- 💿 **Vinyl Animation** - Realistic spinning vinyl disc visualization
- 📱 **Mobile Support** - Works on iOS and Android as PWA or native widgets
- 🌙 **Offline Mode** - All assets cached, works without internet
- 🎭 **Lock Screen Widgets** - Native widgets for iOS 16+ and Android 12+

## Quick Start (Desktop)

```bash
npm install
npm start
```

## Mobile Installation

### Option 1: PWA (Easiest - Recommended)

1. **Host the files** on any web server (GitHub Pages, Netlify, Vercel)
2. **Share the URL** with your friend
3. **On iOS**: Safari → Share → Add to Home Screen
4. **On Android**: Chrome → Menu → Install App

The PWA works offline and can be added to home screen!

### Option 2: Native Apps (For Lock Screen Widgets)

See `DEPLOYMENT.md` for detailed instructions on building native iOS and Android apps with lock screen widget support.

## Project Structure

```
music-widget/
├── index.html              # Main HTML (works as PWA)
├── style.css              # Styling with mobile responsiveness
├── renderer_clean.js      # App logic and theme system
├── service-worker.js      # Offline caching (PWA)
├── manifest.json          # PWA manifest
├── main_fix.js            # Electron main process (desktop)
├── assets/                # Music files, images, GIFs
├── mobile-widgets/        # Native widget implementations
│   ├── ios/              # iOS Widget Extension (Swift)
│   ├── android/          # Android App Widget (Kotlin)
│   └── react-native/     # Cross-platform wrapper
└── DEPLOYMENT.md         # Detailed deployment guide
```

## Themes

1. **GLUE (Snoopy x Glue Night)**
   - Song: GLUE SONG by Clairo
   - Background: Starlight with moon animation
   - Colors: Dark blue with gold accents

2. **Anything**
   - Song: Anything by Adrianne Lenker
   - Background: Pink polka dots
   - Colors: Light with red accents

## Deployment

### For PWA:
1. Host files on web server (requires HTTPS)
2. Share URL - users can install via browser
3. Works offline automatically

### For Native Apps:
See `mobile-widgets/README.md` and `DEPLOYMENT.md` for:
- React Native setup
- iOS App Store submission
- Android Google Play submission
- TestFlight/Google Play Beta testing

## Development

### Desktop (Electron)
```bash
npm install
npm start
```

### Mobile (PWA)
Just open `index.html` in a browser or host it on a server.

### Native Widgets
See `mobile-widgets/` folder for platform-specific setup.

## Requirements

- **Desktop**: Node.js, Electron
- **PWA**: Modern browser with service worker support
- **iOS Widgets**: Xcode 14+, iOS 16+, Apple Developer Account
- **Android Widgets**: Android Studio, Android 12+, Google Play Developer Account (optional)

## Browser Support

- ✅ Chrome/Edge (Android)
- ✅ Safari (iOS)
- ✅ Firefox
- ❌ Internet Explorer (not supported)

## Notes

- Audio requires user interaction before playing (browser security)
- Service worker caches all assets for offline use
- Widget updates may be delayed (platform limitations)
- Lock screen widgets require native apps (iOS 16+, Android 12+)

## License

MIT

---

**Made with ❤️ for music lovers**
