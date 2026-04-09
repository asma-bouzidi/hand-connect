# Hand Connect - Neon Aura AR

[![Hand Tracking Demo](screenshots/demo.gif)](https://github.com/yourusername/hand-connect)

## 🌟 Overview

**Hand Connect** is an immersive Augmented Reality (AR) experience that transforms your webcam feed into a mesmerizing neon light show controlled by your hands. Built with [MediaPipe Hands](https://mediapipe.dev/) for real-time hand tracking, it features:

- **Dual-hand tracking** with glowing neon skeletons
- **5 dynamic themes**: Rainbow, Cyberpunk, Lava, Ocean, Galaxy
- **Interactive gestures**: Pinch to create shockwaves ⚡
- **Procedural audio synthesis** responding to hand proximity
- **Matrix rain background** that accelerates with hand movement
- **Particle systems & physics** at fingertips
- **Mandala formations** connecting both hands
- **Glassmorphism UI** with live stats (FPS, gesture detection)

Perfect demo of computer vision + WebGL effects in a single HTML file.

## 🎮 Live Demo

Simply open `index.html` in any modern browser and grant camera permissions!

**Pro Tip**: Try bringing two hands close together for electric arcs and binaural humming!

## 🚀 Quick Start

```bash
# Clone/Download the repo
git clone https://github.com/yourusername/hand-connect.git
cd hand-connect

# Open in browser
open index.html  # macOS
xdg-open index.html  # Linux
start index.html  # Windows
```

**No build step required** - pure vanilla HTML/CSS/JS!

## ✨ Features

| Feature | Description |
|---------|-------------|
| **Real-time Tracking** | MediaPipe Hands (2 hands max, high accuracy) |
| **Visual Effects** | Neon glows, particles, shockwaves, lightning arcs |
| **Audio Reactivity** | Procedural synth (pitch/volume follows hand distance) |
| **Gestures** | Pinch detection, spread percentage, hand velocity |
| **Themes** | 5 switchable color palettes with live preview |
| **Performance** | 60FPS target, WebGL-accelerated canvas rendering |

## 🎨 Themes

- **🌈 Rainbow**: Classic HSV rainbow cycling
- **💿 Cyberpunk**: Pink/cyan electric palette
- **🔥 Lava**: Flowing orange-red gradients  
- **🌊 Ocean**: Cool blue/teal waves
- **🌌 Galaxy**: Purple/magenta cosmic hues

## 🛠 Tech Stack

```
Core: Vanilla HTML/CSS/JS
Vision: MediaPipe Hands v0.4+
Graphics: HTML5 Canvas + Screen Blend Mode
Audio: Web Audio API (Oscillators + Gain)
Physics: Custom particle/ripple systems
CDN: Unpkg (zero setup)
```

## 🎯 Gestures & Interactions

1. **Single Hand**: Neon fingertip trails + matrix acceleration
2. **Two Hands**: Cross-hand lightning + mandala patterns
3. **Pinch (Thumb+Index)**: Shockwave explosion + zap SFX
4. **Hand Spread**: Live % indicator (fist → open hand)
5. **Proximity**: Binaural hum pitch/volume modulation

## 📱 Browser Support

✅ Chrome/Edge/Firefox/Safari (desktop/mobile)  
✅ Webcam + microphone permissions required  
✅ Works on most devices with front-facing camera  

## 🔮 Customization

The code is highly modular:

```js
// Add new theme
themes['MyTheme'] = (t, index, total) => `hsl(${t*50 + index*60}, 100%, 70%)`;

// New gesture
if (isHeartGesture()) createHeartParticles();

// Custom audio
const myOsc = audioCtx.createOscillator();
```

## 📈 Performance Tips

- Use hardware-accelerated browsers (Chrome/Edge recommended)
- Close other tabs for best FPS
- Enable GPU acceleration in browser settings
- Lower `modelComplexity` in MediaPipe config for mobile

## 🎨 Screenshots

Add your screenshots here:
- ![Start Screen](screenshots/start.png)
- ![Tracking](screenshots/tracking.png)
- ![Pinch Effect](screenshots/pinch.png)

## 🤝 Contributing

1. Fork the repo
2. Create feature branch (`git checkout -b feature/amazing-effect`)
3. Commit changes (`git commit -m 'Add amazing effect'`)
4. Push (`git push origin feature/amazing-effect`)
5. Open Pull Request

## 📄 License

MIT License - feel free to use in commercial projects, modify, redistribute.

```
Copyright (c) 2024 Hand Connect

Permission is hereby granted, free of charge, to any person obtaining a copy...
```

## 🙌 Acknowledgments

- [MediaPipe Team](https://mediapipe.dev/) - Amazing hand tracking ML
- [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API) - Procedural sound
- Countless shader artists for WebGL inspiration

---

⭐ **Star this repo if you found it mesmerizing!**  
🚀 **Made with ❤️ using pure web technologies**

