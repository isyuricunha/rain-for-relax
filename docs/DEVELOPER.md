# 🌧️ Rain for Relax - Developer Documentation

## Project Structure

```
rain-for-relax/
├── assets/
│   ├── images/       # Image assets (icons, logos)
│   ├── chill-rain.mp4 # Background video
│   └── rain-chill.mp3 # Audio file
├── docs/             # Documentation
│   ├── USER_GUIDE.md  # End-user documentation
│   └── DEVELOPER.md   # This file
├── .github/          # GitHub Actions workflows
├── index.html        # Main HTML file
├── main.css          # Styles
├── vercel.json       # Vercel deployment config
└── README.md         # Project overview
```

## Local Development

### Prerequisites
- Modern web browser
- (Optional) Local web server

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/isyuricunha/rain-for-relax.git
   cd rain-for-relax
   ```

2. Start a local server:
   ```bash
   # Python 3
   python -m http.server 8000
   # or Node.js
   npx serve .
   ```
3. Open `http://localhost:8000` in your browser

## Audio Implementation

### Audio Element
- Located in `index.html` with ID `rain-audio`
- Autoplays on page load (subject to browser autoplay policies)
- Loops continuously
- Volume controlled via JavaScript

### Volume Control
- Uses the Web Audio API for smooth volume changes
- Volume range: 0 (mute) to 1 (max)
- Current volume is saved to `localStorage`

## Styling

### Color Scheme
- Background: Dark gradient with video overlay
- Text: White with subtle shadows for readability
- Controls: Semi-transparent white with hover effects

### Responsive Design
- Adapts to different screen sizes
- Touch-friendly controls for mobile devices
- Maintains aspect ratio of video background

## Deployment

### GitHub Pages
1. Push to `main` branch
2. GitHub Actions will automatically deploy to Pages

### Vercel
1. Import the repository into Vercel
2. Automatic deployments on push to `main`

## Testing

### Manual Testing
- Test on different browsers (Chrome, Firefox, Safari, Edge)
- Test on mobile devices
- Verify volume persistence
- Test keyboard shortcuts

### Browser Support
- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile Safari (iOS 10+)
- Chrome for Android

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

### Code Style
- Use semantic HTML5
- Follow BEM naming convention for CSS
- Use ES6+ JavaScript
- Keep code comments clear and concise

## License
MIT - See [LICENSE](LICENSE) for details.
