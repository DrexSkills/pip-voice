# Pip

A voice-only AI companion that lives as a constellation of light on a black screen.
Talk to it out loud and it talks back. There's no chat box.

- **Always listening.** Allow the mic once and Pip keeps the conversation going on its own.
- **Heartbeat visuals.** Hundreds of drifting dots link up into a living sphere. When Pip speaks it pulses like a heartbeat and lines stretch out from its surface.
- **Sees your screen.** Tap the eye button, choose a screen or tab, then ask *"what do you see?"* A card pops up with the screenshot and the things Pip noticed, while it describes them out loud.
- **Powered by Groq** for fast replies (`qwen/qwen3.8-27b`, which handles both talking and seeing).

## Run it

Open the GitHub Pages link for this repo, or serve `index.html` from any HTTPS host or `localhost`.
Microphone and screen sharing only work on HTTPS or localhost.

1. Paste your Groq API key the first time. It's saved in your browser's local storage only, never in this repo.
2. Tap **Allow microphone and voice**.
3. Talk.

Works best in Chrome or Edge. Safari can talk and listen. Firefox can't do speech recognition.

## Notes

- Browsers require one tap per page load before a site can play sound, so on return visits you tap **Wake Pip** once.
- Your Groq key is used directly from the browser. Anyone who uses this page on your computer could read it from local storage, so set a spend limit in the Groq console.
- To change models, edit `GROQ_MODEL` near the top of the script in `index.html`.
