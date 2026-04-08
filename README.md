# VoiceIt 🔊
### Text-to-Speech Meeting Overlay — TSA Software Development

A floating overlay that lets deaf users **type and be heard** in any meeting. Type a message or tap a quick phrase — it speaks out loud through your speakers so everyone on the call hears a voice.

---

## Setup & Run

### Prerequisites
- [Node.js](https://nodejs.org/) (v18 or higher)

### Install & Launch

```bash
npm install
npm start
```

Two windows appear:
- **Floating overlay** — sits above Zoom/Meet with a text input and quick phrase buttons
- **Control panel** — voice picker, speed/pitch/volume sliders, custom phrases, spoken history

---

## How to Use

1. Join your Zoom/Teams/Meet call as normal
2. Launch VoiceIt — the overlay floats above your meeting window
3. **Type** what you want to say and press Enter (or click the speaker button)
4. **Or tap** a quick phrase button for instant responses
5. Your speakers play the voice — everyone on the call hears it

---

## Features

| Feature | Details |
|---|---|
| ⌨️ Type-to-speak | Type anything, press Enter to speak instantly |
| ⚡ Quick phrases | 12 built-in one-tap responses |
| 🎙️ Voice picker | Choose from all system voices |
| 🎛️ Voice tuning | Adjust speed, pitch, and volume |
| 📝 Custom phrases | Save your own frequently used phrases |
| 📋 Spoken history | Log of everything spoken, copyable |
| 🪟 Always on top | Floats over Zoom, Teams, Meet, any app |

---

## Tech Stack

- **Electron** — cross-platform desktop app
- **Web Speech Synthesis API** — built-in browser TTS, no API key needed
- **HTML/CSS/JS** — no frameworks

---

## TSA Documentation Notes

**Problem Solved:** Deaf and hard-of-hearing users can follow meetings using captions, but have no good way to speak back. Typing in a chat box is slow and breaks conversation flow. VoiceIt gives deaf users a voice in real-time conversations.

**Who it helps:** ~15% of adults have some degree of hearing loss. In professional settings, this creates a significant communication barrier that no major meeting platform has solved from the deaf user's perspective.

**Design choices:**
- Quick phrase buttons reduce response time to under 1 second
- Outfit font chosen for readability and modern feel
- Minimal, non-intrusive overlay so it doesn't block the meeting UI
- All processing is local — no data leaves the device
