# Pip

Pip is Hassen's voice-only AI companion. It appears as a glowing brain of light on a black screen, wired into a neon network. Talk to it out loud and it answers in a natural human voice. There's no chat box.

## What it does

- **Always listening.** Allow the mic once and Pip keeps the conversation going on its own.
- **A brain with four memory lobes.** *Hassen* holds facts about you, *Topics* holds what you've talked about, *Seen* holds what Pip noticed on your screen, and *Plans* holds goals and reminders. A bright core in the middle is Pip's voice. Each lobe grows new dots as it learns. When Pip remembers something, signals race down the synapses to that lobe and a note pops up, then dissolves.
- **Captions that come and go.** Pip's words appear as it speaks, then scatter into dust. What you said floats up into the brain.
- **Thousands of connected dots.** Every lobe is a web of linked nodes filled with glowing dust, and a neural field of drifting dots links the whole brain together.
- **Zoom and turn.** Scroll or pinch to zoom in and out, drag to spin the brain, and double-tap (or press 0) to reset. The + and - keys zoom too.
- **Neon background.** Glowing wires carry LED pulses that flicker with Pip's voice.
- **Human British voice.** With an ElevenLabs key, Pip speaks as George, a warm, calm British man (say "use Daniel" for a deeper one). Without one, Pip downloads a free British voice (Kokoro, about 90 MB, once) that runs on your device. Groq's Orpheus voice covers the gap while it loads. Say "change your voice" to switch, or "use your American voice".
- **Sees your screen.** Tap the eye, pick a screen or tab, then ask "what do you see?"
- **Memory on every device.** Your memory is end-to-end encrypted with your passphrase and stored in Supabase. Open the site on any computer or phone, type the same passphrase once, and Pip remembers you, and your Groq key comes with it.

## Setup

1. Open https://drexskills.github.io/pip-voice/
2. First time: choose a memory passphrase (8+ characters) and paste your Groq API key.
3. On any other device, type the same passphrase. That's all.
4. Optional: for the most human voice, add an ElevenLabs API key on the start screen ("Add an ElevenLabs key"). It syncs, encrypted, with your memory.

Chrome or Edge works best. Safari can talk and listen. Firefox can't do speech recognition.

## Privacy

- Memory and your Groq key are encrypted in the browser (AES-GCM, key derived from your passphrase) before upload. The database only ever sees ciphertext, stored under a hash of your passphrase.
- Nobody can read your memory without the passphrase, and nobody can recover it if you forget it.
- Use a passphrase you don't use anywhere else.

## Models

`qwen/qwen3.8-27b` for talking and seeing, and `canopylabs/orpheus-v1-english` for the voice. Change them at the top of the script in `index.html`.
