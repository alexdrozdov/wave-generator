# 🎛️ Stereo Signal Generator

A browser-based stereo signal generator designed for mobile and desktop use. It mimics the tactile feel of physical lab equipment, allowing precise control over frequency, phase shift, and stereo balance.

---

## 🚀 Features

- Dual sine wave generation (Left and Right channels)
- Adjustable frequency (20–300 Hz by default)
- Adjustable phase shift (±180°), active only when frequencies are equal
- Stereo balance control (0.0 = full Left, 1.0 = full Right)
- Lock/unlock frequency synchronization
- Live parameter updates while running
- Safety modal on first run (session-based suppression)
- Responsive layout for portrait and landscape modes
- Instrument-style UI with beveled panels and tactile controls

---

## 📱 Layout Behavior

- **Portrait (mobile)**: Stacked vertical layout, optimized for one-handed use
- **Landscape (mobile)**: Side-by-side controls, labels aligned left, caption hidden
- **Desktop**: Always uses portrait layout for consistent panel feel

---

## 🧱 Tech Stack

- HTML5 + CSS3
- JavaScript (Web Audio API)
- No external dependencies
- Fully client-side, deployable via GitHub Pages

---

## ⚙️ Usage

1. Open `index.html` in a browser
2. Adjust frequency, phase shift, and balance
3. Press **Start** to begin signal generation
4. Use **Lock Frequencies** to synchronize channels
5. Adjust parameters live while running

> ⚠️ On first run, a safety modal warns about full-volume output. You can suppress it for the session.

---

## 📐 File Structure

```
/stereo-signal-generator/
  ├── index.html # Main app
  ├── README.md # Project overview
  ├── requirements.md # Functional & non-functional specs
```

---

## 🛠️ Planned Enhancements

- Settings panel (frequency range, channel count)
- Waveform selection (sine, square, etc.)
- Preset management
- PWA packaging for offline use
- LED-style indicators for running state

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

## 🙌 Acknowledgments

Designed and refined collaboratively with a focus on tactile feedback, clarity, and reviewability. Inspired by real-world signal generator equipment and iterative UI design.