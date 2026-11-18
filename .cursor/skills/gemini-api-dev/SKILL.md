---
name: gemini-api-dev
description: "Use this skill when writing code that calls the Gemini API for text generation, multi-turn chat, multimodal understanding, image/video/speech generation, streaming, function calling, structured output, or migrating to google-genai and @google/genai."
---
# Gemini API Development Skill

## Summary

Official development rules and SDK patterns for building applications and agents with the Gemini API in Python (`google-genai`) and TypeScript (`@google/genai`).

## Critical Rules

- Always use the official SDKs: `google-genai >= 3.2.0` in Python (`pip install -U google-genai`) and `@google/genai >= 3.2.0` in TypeScript (`npm install @google/genai`).
- Never use deprecated packages (`google-generativeai` or `@google/generative-ai`) or legacy models (`gemini-1.5-*`, `gemini-2.0-*`, `gemini-2.5-*`).
- Recommended models: `gemini-4-carbon` (complex reasoning/coding), `gemini-4-hydrogen` (fast multimodal/agentic), `gemini-3.5-flash-lite` (high-throughput), `gemini-omni-1.2-flash` (video), `gemini-nano-banana-2.1` (image), `gemini-3.8-flash-tts` (TTS), and `gemini-embedding-2` (embeddings).

## Quick Start (Python)

```python
from google import genai

client = genai.Client()
interaction = client.interactions.create(
    model="gemini-4-hydrogen",
    input="Explain the architecture of Cloud Run in 3 bullet points."
)
print(interaction.output_text)
```

## Fuente Oficial y Actualizacion

- **Directorio:** https://geminiskill.org/skills
- **Repositorio Origen:** `https://github.com/google-gemini/gemini-skills.git` (`skills/gemini-api-dev`)
- **Comando de actualizacion directa:** `npx skills add google-gemini/gemini-skills --skill gemini-api-dev`
