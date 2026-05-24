# Reverie

A browser-based ambient music workstation with three distinct sonic engines. No installs, no plugins — just open and play.

🎵 **[Try it live](https://duttatrey.github.io/reverie)**

---

## Features

- **Three sound engines** — Cinematic Space Ambient, Tape-Flutter Lo-Fi Lounge, and Minimalist Neo-Classical Ensemble
- **10 harmonic presets per engine** — curated chord progressions spanning jazz, modal, orchestral, and electronic styles
- **Real-time mixing console** — per-channel gain control for pad, sub bass, arpeggio, percussion, and noise wash layers
- **Ambient & harmony modes** — switch between deep drone washes and active melodic lines
- **Tempo control** — adjustable BPM from 40 to 180
- **Pattern variations** — randomisable rhythm patterns per channel
- **Offline WAV export** — render tracks from 30 seconds up to 30 minutes directly in the browser
- **Batch export** — generate multiple unique variations in one run
- **Zero dependencies** — pure Web Audio API, React (CDN), and Tailwind; no build step required

---

## How It Works

Reverie uses the browser's **Web Audio API** to synthesise all sound in real time — no samples or audio files are loaded. Each engine defines its own oscillator types, filter curves, and chord voicings. The scheduler runs on a lookahead clock to keep timing tight even under load.

Exports are rendered offline at 44.1kHz using `OfflineAudioContext`, then encoded as 16-bit PCM WAV files and downloaded directly.

---

## Usage

Just open `index.html` in any modern browser. No server required.

```
git clone https://github.com/duttatrey/reverie.git
cd reverie
open index.html
```

---

## Built With

- [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
- [React 18](https://react.dev/) (CDN)
- [Tailwind CSS](https://tailwindcss.com/) (CDN)

---

## License

MIT
