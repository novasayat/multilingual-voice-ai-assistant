# Multilingual Voice AI Assistant (Notebook)

This project is a simple notebook assistant:
1. Take voice input (or typed input fallback)
2. Detect language
3. Translate to English
4. Ask GPT
5. Translate answer back and optionally speak it

## Files
- `multilingual_voice_ai_assistant.ipynb.ipynb` → main notebook
- `RAGDataset.txt` → optional context text (used if present)

## Safe API key setup (important)
Never commit your real API key to GitHub.

### Recommended (local env variable)
On your PC terminal:

```bash
export OPENAI_API_KEY="your_real_key_here"
```

Then start Jupyter from the same terminal.

### Temporary inside notebook (safer than plain text)
Use `getpass()` in the key setup cell (already included as commented lines).
This keeps key input hidden and only for current session.

## Run on your PC
1. Clone repo
2. Open notebook
3. Run cells top to bottom
4. In first cell, install dependencies
5. Set `OPENAI_API_KEY` (env or getpass)
6. Run final cell and test by speaking or typing

## Notes
- If microphone fails, notebook falls back to typed input.
- If audio output is unavailable, response still prints.
- `RAGDataset.txt` is optional. You can replace its content with your own domain notes.
