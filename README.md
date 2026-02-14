# Heart-Beats-Counter

A real-time heart rate monitoring simulation built with vanilla HTML, CSS, and JavaScript. Watch your heart beat in style with a beautiful glass-morphism interface.

![Screenshot_14-2-2026_232023_127 0 0 1](https://github.com/user-attachments/assets/c7511e12-c9e1-4c19-bbf1-d056fc55c3e4)


## ✨ Features

- **Real-time BPM display** – Simulated heart rate that you can control
- **Animated heart** – Pulsates with every beat for visual feedback
- **Total beats counter** – Accumulates every heartbeat (automatic + manual)
- **Interactive controls** – Add beats manually, increase BPM, reset everything
- **Visual progress bar** – Shows intensity relative to BPM range (30–180)
- **Responsive design** – Works beautifully on all screen sizes
- **Glass-morphism UI** – Modern, sleek, with subtle glow effects

## 🎮 How It Works

The heart beats automatically based on the current BPM (beats per minute):
- **72 BPM** – Default resting rate
- **+5 button** – Increases heart rate by 5 BPM (capped at 180)
- **BEAT button** – Manually trigger a heartbeat (adds to total count)
- **Reset button** – Resets total beats to 0 and BPM to 72

The heart icon pulses with each beat, and the progress bar reflects the current BPM intensity.

## 🚀 Quick Start

1. Clone this repository:
```bash
git clone https://github.com/yourusername/heart-beats-counter.git
```

2. Open `index.html` in your browser

That's it! No dependencies, no build steps – just pure HTML, CSS, and JavaScript.

## 🎨 Customization

You can easily customize the simulation:

### Adjust BPM Range
In the JavaScript section, modify these constants:
```javascript
const minBpm = 30;   // Minimum BPM
const maxBpm = 180;  // Maximum BPM
```

### Change Visual Theme
The color scheme uses CSS variables in the `.card` and gradient classes. Main accent colors:
- Primary pink: `#ff3b5c`
- Background dark: `#1a1e2f`
- Glass effect: `rgba(18, 22, 40, 0.75)`

### Modify Animation Speed
The heart beat interval automatically syncs with BPM, but you can adjust the animation duration in the `.heart-shape.beat` class:
```css
.heart-shape.beat {
    transform: scale(1.2);
    transition: transform 0.15s cubic-bezier(...);
}
```

## 📱 Responsive Behavior

The card layout adapts to different screen sizes:
- **Desktop**: 420px fixed width with comfortable spacing
- **Mobile**: Full-width with reduced padding (max-width: 100%)
- All fonts and controls scale appropriately

## 🧠 Technical Implementation

- **Pure vanilla JavaScript** – No frameworks, lightweight (~150 lines)
- **CSS Glass-morphism** – Backdrop filters, subtle borders, and glow effects
- **Real-time updates** – Automatic interval scheduling based on BPM
- **Smooth animations** – CSS transitions for heart pulses and progress bar
- **Accessible** – Semantic HTML, proper button labels, and ARIA-friendly structure

## 🎯 Use Cases

- **Fitness demos** – Visualize heart rate concepts
- **UI inspiration** – Glass-morphism design patterns
- **Learning tool** – Understand setInterval, CSS animations, and reactive UI
- **Relaxation** – Watch the heart pulse at different rhythms

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features (like sound effects, historical graphs, or different heart styles)
- Submit pull requests for improvements

## 📄 License

MIT License – feel free to use this in your own projects!

## 🙏 Acknowledgments

- Inspired by medical monitors and fitness trackers
- Heart icon and animations created with pure CSS/HTML
- Special thanks to the open-source community for design inspiration

---

**Made with ❤️ and lots of heartbeats**
