---
name: gemini-omni-flash-api
description: "Use this skill for generative video editing, text-to-video, image- and video-referenced video generation, keyframe transitions, and video extensions using gemini-omni-1.2-flash."
---
# Gemini Omni Flash Video Skill

## Summary

Workflows for generating, editing, and extending video (3s-15s across 360p, 720p, 1080p, and 4K) with `gemini-omni-1.2-flash` via the Gemini Interactions API and Files API.

## Key Rules

- Upload input images/videos via the Files API and wait until `ACTIVE` before calling `client.interactions.create`.
- Bind media using natural language by order in `input` rather than deprecated tags.
- Include `"Keep everything else the same."` when performing targeted video edits.

## Fuente Oficial y Actualizacion

- **Directorio:** https://geminiskill.org/skills
- **Repositorio Origen:** `https://github.com/google-gemini/gemini-skills.git` (`skills/gemini-omni-flash-api`)
- **Comando de actualizacion directa:** `npx skills add google-gemini/gemini-skills --skill gemini-omni-flash-api`
