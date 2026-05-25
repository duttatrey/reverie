# Reverie
A browser-based ambient music workstation with five distinct sonic engines. No installs, no plugins — just open and play.

🎵 Try it live

## Features
- **Five sound engines** — Cinematic Space Ambient, Tape-Flutter Lo-Fi Lounge, Minimalist Neo-Classical Ensemble, Deep Focus Essay Bed, and Future Garage Short Bed
- **10 harmonic presets per engine** — curated chord progressions spanning jazz, modal, orchestral, electronic, and psychoacoustic styles
- **Real-time mixing console** — per-channel gain control for pad, sub bass, arpeggio, melodic lines, and noise wash layers
- **Ambient & harmony modes** — switch between deep drone washes and active melodic lines
- **Tempo control** — adjustable BPM from 40 to 180
- **Pattern variations** — randomisable rhythm patterns per channel
- **Single mix export** — bake the current session to a WAV at your chosen length
- **Batch export** — generate multiple unique variations in one run, each with randomised presets and patterns
- **Offline WAV export** — render tracks from 30 seconds up to 10 minutes directly in the browser, encoded at 44.1kHz 16-bit PCM
- **Zero dependencies** — pure Web Audio API, React (CDN), and Tailwind; no build step required

## Sound Engines
| Engine | Character | Default BPM |
|---|---|---|
| 🚀 Space | Cinematic sawtooth pads, deep sub drones, Lydian/Phrygian voicings | 60 |
| ☕ Lo-Fi | Tape-warm triangle pads, vinyl noise, jazz extended chords | 74 |
| 🎻 Classical | Felt strings, pizzicato plucks, neo-classical harmonic clusters | 52 |
| 🎓 Essay Bed | Notched sine pads, 50Hz sub anchor, psychoacoustic focus tuning | 50 |
| 🎬 Reels Bed | Muted organ suspensions, ghost noise shuffles, future garage patterns | 132 |

## How It Works
Reverie uses the browser's Web Audio API to synthesise all sound in real time — no samples or audio files are loaded. Each engine defines its own oscillator types, filter curves, envelope shapes, and chord voicings. A lookahead clock scheduler keeps timing tight even under load.

Exports are rendered offline using `OfflineAudioContext`, passed through a master limiter, then encoded as 16-bit PCM WAV files and downloaded directly to your device.

## Usage
Just open `index.html` in any modern browser. No server required.

```bash
git clone https://github.com/duttatrey/reverie.git
cd reverie
open index.html
```

## Built With
- Web Audio API
- React 18 (CDN)
- Tailwind CSS v4 (CDN)

## License
MIT
