# 2-assembyai

App de transcription audio + résumé IA, en anglais, arabe standard et darija marocaine. L'utilisateur upload un fichier audio (.mp3/.wav), transcrit via l'API Whisper de Groq ; la transcription (et un résumé ou une explication détaillée générés par le LLM de Groq) peuvent être exportés en PDF avec mise en forme arabe RTL.

> Note : malgré le nom du dossier, l'app utilise l'API Whisper de Groq, pas AssemblyAI.

## Tech stack

streamlit, groq (Whisper + LLaMA/gpt-oss), fpdf2, arabic-reshaper, python-bidi, python-dotenv

## Lancer le projet

```bash
pip install -r requirements.txt
```

Créer un `.env` avec `GROQ_API_KEY=...`

```bash
streamlit run app.py
```
