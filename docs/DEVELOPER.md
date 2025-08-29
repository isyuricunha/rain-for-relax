# 🌧️ Rain for Relax - Developer Documentation

## 🏗️ Project Structure

```
rain-for-relax/
├── assets/
│   ├── images/       # Icons and logos
│   │   ├── cloud.png
│   │   ├── discord.png
│   │   ├── github.png
│   │   ├── linkedin.png
│   │   ├── logo.ico
│   │   ├── logo.png
│   │   ├── mail.png
│   │   └── telegram.png
│   ├── chill-rain.mp4 # Background video
│   └── rain-chill.mp3 # Audio file
├── docs/             # Documentation
│   ├── USER_GUIDE.md  # User documentation
│   └── DEVELOPER.md   # This file
├── .github/          # GitHub workflows
├── index.html        # Main HTML file
├── main.css          # Styles
├── vercel.json       # Vercel config
└── license.md        # License information
```

## 🛠️ Technical Details

### Core Technologies
- **HTML5**: Semantic markup
- **CSS3**: Styling with modern features (Flexbox, CSS Variables)
- **Vanilla JavaScript**: No frameworks or build tools
- **Web Audio API**: For smooth volume control

### Key Features Implementation

#### 1. Audio Playback
- Single `<audio>` element in `index.html`
- Autoplay with fallback for browser restrictions
- Loop enabled for continuous playback

#### 2. Volume Control
- Custom slider with cross-browser support
- Mute toggle with visual feedback
- Volume persistence using `localStorage`

#### 3. Keyboard Shortcuts
- Event listeners for keyboard input
- Prevent default browser behavior where needed
- Visual feedback for user actions

## 🚀 Local Development

### No Build Step Required
This project uses vanilla web technologies - just open `index.html` in a browser!

### Optional: Local Server
For testing with a local server (bypasses some browser restrictions):

```bash
# Python 3
python -m http.server 8000

# Or with PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

## 🧪 Testing

### Manual Testing
1. **Audio Playback**
   - Verify autoplay works (may require user interaction in some browsers)
   - Test volume controls (slider and mute button)
   - Check if volume persists on page refresh

2. **Responsive Design**
   - Test on various screen sizes
   - Verify touch controls on mobile devices
   - Check landscape/portrait orientations

3. **Browser Compatibility**
   - Chrome (latest)
   - Firefox (latest)
   - Safari (desktop and iOS)
   - Edge (latest)

## 🚀 Deployment

### GitHub Pages
1. Push to the `main` branch
2. GitHub Actions will automatically deploy to Pages

### Vercel
1. Import repository into Vercel
2. Automatic deployments on push to `main`

## 📝 Code Style

### HTML
- Semantic elements
- Proper indentation (2 spaces)
- Descriptive class names

### CSS
- BEM naming convention
- Mobile-first approach
- CSS Variables for theming

### JavaScript
- ES6+ syntax
- Event delegation where appropriate
- Clear function and variable names

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Pull Request Guidelines
- Keep changes focused and atomic
- Update documentation as needed
- Test your changes thoroughly

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](license.md) file for details.

## 🙏 Acknowledgments

- Rain sounds and video are royalty-free
- Icons from [Feather Icons](https://feathericons.com/)
- Fonts from [Google Fonts](https://fonts.google.com/)
