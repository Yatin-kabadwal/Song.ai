<div align="center">

# 🎵 SoundWave AI

### Free Music & Voice Generator — No API. No Sign-up. No Cost. Forever.

<br/>

![SoundWave AI Banner](https://via.placeholder.com/900x300/080a12/00e5a0?text=SoundWave+AI+%E2%80%94+Free+Forever)

**SoundWave AI** is a fully browser-based music and voice generation platform inspired by Suno AI — built entirely in a single HTML file with zero backend, zero API keys, and zero ongoing costs. Your users get a professional audio experience for free, forever.

[🚀 Deploy Now](#-deploy-in-2-minutes) · [✨ Features](#-features) · [🎯 How It Works](#-how-it-works) · [📱 Screenshots](#-screenshots) · [🤝 Contributing](#-contributing)

</div>

---

## ✨ Features

### 🎵 AI Music Generator
- **One-click music creation** — pick mood, genre, energy → hit Generate
- **8 Moods** — Happy, Sad, Epic, Chill, Romance, Dark, Uplift, Mystic
- **10 Genres** — Lo-Fi, Pop, Hip-Hop, Cinematic, Jazz, EDM, Ambient, Rock, R&B, Classical
- **Energy slider** — from super chill to high intensity
- **Duration control** — 15s, 30s, 45s, 1 minute
- **Multi-layer composition** — drums + bass + melody + chords + arpeggio, all generated live
- **Reverb & Delay FX** applied automatically per genre
- **Song history** — replay, manage, and delete generated tracks
- **Fixed player bar** — controls always visible while browsing

### 🎙 Voice Generator
- **4 voice characters** — Alex (male), Aria (female), Marcus (male), Sofia (female)
- **10 languages** — English (US/UK), Hindi, Spanish, French, German, Japanese, Arabic, Portuguese, Chinese
- **Speed, Pitch & Volume** controls
- **Quick example prompts** — welcome, news, story, assistant, Hindi, Spanish
- **Live waveform** animation during playback
- **Powered by Web Speech API** — zero cost, works in any modern browser

### 🛠 Technical
- ✅ **Single HTML file** — no build step, no dependencies to install
- ✅ **Zero backend** — everything runs in the browser
- ✅ **Zero API keys** — no Hugging Face, no OpenAI, nothing
- ✅ **Zero ongoing cost** — host for free forever
- ✅ **Fully mobile responsive** — works on all screen sizes
- ✅ **Keyboard shortcuts** — Space, Esc, Ctrl+Enter
- ✅ **Share button** — native share on mobile, clipboard copy on desktop

---

## 🎯 How It Works

### Music Generation
SoundWave AI uses **[Tone.js](https://tonejs.github.io/)** — a Web Audio API framework — to synthesize multi-layered music entirely in the browser:

```
User picks Mood + Genre + Energy
        ↓
Mood → sets BPM, musical key, scale (major/minor/dorian)
Genre → shapes beat pattern, instrument choices, FX
Energy → adjusts tempo, volume levels, intensity
        ↓
Engine builds layers simultaneously:
  🥁 Drum layer  (Kick, Snare, Hi-Hat sequences)
  🎸 Bass line   (genre-specific pattern + notes)
  🎹 Melody      (randomized scale-aware phrases)
  🎵 Chord pad   (diatonic chord progression)
  ✨ Arpeggio    (for Pop, EDM, Cinematic, Hip-Hop)
        ↓
Reverb + Delay FX → Master Gain → Your speakers
```

**No audio files are downloaded.** Everything is synthesized in real time using Web Audio oscillators and synthesizers.

### Voice Generation
Uses the browser's built-in **Web Speech API** (`SpeechSynthesis`):

```
User types text + selects voice character + language
        ↓
Browser's native TTS engine speaks the text
Voice character maps to male/female voice selection
Language routes to correct locale voices
        ↓
Live waveform animates during playback
```

No server, no API, no audio files — just the browser.

---

## 🚀 Deploy in 2 Minutes

### Option 1 — Netlify (Recommended, Easiest)
1. Download `soundwave-ai.html`
2. Go to [netlify.com](https://netlify.com) → Sign up free
3. Drag and drop the file onto the Netlify dashboard
4. Done — you get a live URL like `yoursite.netlify.app`

### Option 2 — GitHub Pages
```bash
# 1. Fork or clone this repo
git clone https://github.com/yourusername/soundwave-ai.git
cd soundwave-ai

# 2. Rename the file to index.html
mv soundwave-ai.html index.html

# 3. Push to GitHub
git add .
git commit -m "deploy"
git push

# 4. Go to repo Settings → Pages → Deploy from branch (main)
# Your site will be live at: yourusername.github.io/soundwave-ai
```

### Option 3 — Vercel
```bash
npm install -g vercel
vercel --prod
```

### Option 4 — Any Static Host
Just upload `soundwave-ai.html` (rename to `index.html`) to:
- **Cloudflare Pages** — free, global CDN
- **Firebase Hosting** — free tier, fast
- **Surge.sh** — `npx surge soundwave-ai.html`
- **Any web server** — Apache, Nginx, even a USB drive

> **No server config needed.** It's just one HTML file.

---

## 📁 File Structure

```
soundwave-ai/
│
├── soundwave-ai.html      ← The entire app (single file)
├── README.md              ← You are here
└── LICENSE                ← MIT License
```

That's it. One file. The entire platform.

---

## 🌐 Browser Compatibility

| Browser | Music | Voice (TTS) | Notes |
|---------|-------|-------------|-------|
| ✅ Chrome 80+ | Full | Full | **Recommended** |
| ✅ Edge 80+ | Full | Full | Fully supported |
| ✅ Safari 14+ (iOS/Mac) | Full | Partial | Tap screen first to unlock audio |
| ⚠️ Firefox | Full | Limited | Fewer TTS voice options |
| ❌ IE / Old browsers | No | No | Web Audio API not supported |

> **Best experience:** Chrome or Edge on desktop/Android. Safari on iPhone/iPad.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Space` | Play / Pause current track |
| `Escape` | Stop all audio |
| `Ctrl + Enter` | Generate music (on Music tab) / Speak (on Voice tab) |

---

## 🎛 Music Engine Details

### Supported Moods & Their Properties

| Mood | BPM | Key | Scale |
|------|-----|-----|-------|
| 😊 Happy | 125 | C | Major |
| 😢 Sad | 70 | A | Natural Minor |
| ⚡ Epic | 145 | D | Dorian |
| 🌊 Chill | 85 | G | Major |
| 💖 Romance | 90 | F | Major |
| 🌑 Dark | 110 | E | Natural Minor |
| 🚀 Uplift | 130 | D | Major |
| 🌌 Mystic | 95 | B | Dorian |

### Beat Patterns by Genre

- **Lo-Fi** — Swung kick, sparse snare, gentle hi-hats, bass groove
- **Hip-Hop** — Boom-bap kick, syncopated snare, rolling hi-hats
- **EDM** — Four-on-the-floor kick, eighth-note hi-hats, heavy bass
- **Cinematic** — Minimal drums, lush pads, melody-forward, arpeggios
- **Jazz** — Triangle bass, poly synth chords, no kick
- **Ambient** — No drums, long attack pads, slow chord changes
- **Rock** — Driving kick-snare, eighth hi-hats, sawtooth bass
- **Classical** — No drums, triangle oscillators, slow compositions

---

## 🔧 Customization

Since it's a single HTML file, customization is straightforward. Open the file in any text editor.

### Change the app name / branding
```html
<!-- Find this line and change it -->
<div class="logo">SoundWave AI</div>
```

### Add a new mood
```javascript
// In the MOODS array, add:
{id:'energetic', icon:'🔥', name:'Energetic', color:'#ff6b35', bpm:155, scale:'major', root:'A'},
```

### Add a new genre
```javascript
// In the GENRES array, add:
{id:'reggae', name:'Reggae', icon:'🌴'},
```

### Change default colors
```css
/* In :root, edit the CSS variables */
:root {
  --green: #00e5a0;    /* Primary accent */
  --purple: #8b5cf6;   /* Secondary accent */
  --pink: #f472b6;     /* Voice tab accent */
}
```

### Add a new language for TTS
```html
<!-- In the <select id="v-lang"> element, add: -->
<option value="ko-KR">🇰🇷 Korean</option>
```

---

## 📦 Dependencies

SoundWave AI uses **one external dependency**, loaded via CDN:

| Library | Version | Purpose | License |
|---------|---------|---------|---------|
| [Tone.js](https://tonejs.github.io/) | 14.8.49 | Browser audio synthesis engine | MIT |

Everything else uses:
- **Web Speech API** — built into Chrome, Edge, Safari (for TTS)
- **Web Audio API** — built into all modern browsers (used by Tone.js)
- **No npm, no node, no build tools**

---

## ❓ FAQ

**Q: Is it really free forever?**
Yes. There are no servers, no APIs, and no usage counters. Your hosting costs nothing on Netlify/GitHub Pages free tiers. The only cost would be if you choose a paid hosting plan.

**Q: Does it work offline?**
Music generation works offline once the page is loaded (Tone.js is cached). Voice/TTS requires the browser's built-in engine (works offline on most devices). The Google Fonts may not load offline (only affects typography, not functionality).

**Q: Why doesn't it sound exactly like Suno?**
Suno uses large AI neural networks running on GPU servers to generate music. That requires significant compute resources and is not possible in a browser for free. SoundWave AI uses algorithmic synthesis — it creates real music with real instruments, but through code rather than AI models.

**Q: Can I use the generated music commercially?**
The music is generated by your browser using open-source synthesis code. There are no copyrighted samples. However, please verify current laws in your jurisdiction regarding algorithmically generated music before commercial use.

**Q: The voice sounds robotic — how do I improve it?**
Voice quality depends entirely on the voices installed in the user's operating system. Chrome on Windows uses Microsoft voices, Chrome on Mac uses Apple voices, and iOS Safari uses Siri voices. Recommend Chrome on desktop for the best experience.

**Q: Can I add real AI music generation?**
Yes! You can integrate the [Hugging Face Inference API](https://huggingface.co/facebook/musicgen-small) (free tier) for real AI-generated music. Users would need a free HuggingFace token. See the previous version of the app for an implementation example.

**Q: How do I report a bug?**
Open an issue on GitHub with your browser, OS, and a description of the problem.

---

## 🤝 Contributing

Contributions are welcome! Here's how:

```bash
# 1. Fork the repository
# 2. Make your changes to soundwave-ai.html
# 3. Test in Chrome and Firefox
# 4. Submit a pull request
```

### Ideas for contributions
- [ ] Add more genres (K-Pop, Bollywood, Afrobeats, Country)
- [ ] Add more moods (Angry, Peaceful, Nostalgic)
- [ ] Implement a download/export feature for generated audio
- [ ] Add a BPM tap tempo button
- [ ] Improve mobile keyboard for synth
- [ ] Add more TTS language examples
- [ ] Dark/light theme toggle
- [ ] Add visualizer canvas during music playback

---

## 📄 License

```
MIT License

Copyright (c) 2025 SoundWave AI

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.
```

---

## 🙏 Credits & Acknowledgements

- **[Tone.js](https://tonejs.github.io/)** by Yotam Mann — the incredible Web Audio framework that powers the music engine
- **[Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)** — browser-native TTS used for voice generation
- **[Suno AI](https://suno.ai)** — inspiration for the UX and workflow
- **[Google Fonts](https://fonts.google.com/)** — Bricolage Grotesque & Instrument Sans typography

---

<div align="center">

**Built with ❤️ — Free forever for everyone**

⭐ Star this repo if you find it useful!

</div>
