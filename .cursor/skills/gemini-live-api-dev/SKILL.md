---
name: gemini-live-api-dev
description: "Use this skill when building real-time, bidirectional streaming applications with the Gemini Live API over WebSockets in Python (google-genai) or TypeScript (@google/genai)."
---
# Gemini Live API Development Skill

## Summary

Guide for building low-latency, real-time bidirectional voice, video, and text applications over WebSockets using `gemini-3.8-live`, `gemini-3.8-live-extended-thinking`, and `gemini-3.5-transcribe-live`.

## Key Rules

- Input audio: 16-bit PCM mono at 16kHz (`audio/pcm;rate=16000`). Output audio: 24kHz PCM.
- Use `session.send_realtime_input(audio=..., video=..., text=...)` for real-time streaming input.
- Set `behavior="NON_BLOCKING"` on tool declarations when using extended thinking and monitor `interaction_status` (`IN_PROGRESS` vs `IDLE`).

## Fuente Oficial y Actualizacion

- **Directorio:** https://geminiskill.org/skills
- **Repositorio Origen:** `https://github.com/google-gemini/gemini-skills.git` (`skills/gemini-live-api-dev`)
- **Comando de actualizacion directa:** `npx skills add google-gemini/gemini-skills --skill gemini-live-api-dev`
