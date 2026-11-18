# skills-google-cloud-gemini

Repertorio de Skills de Google Cloud (Cloud Run, BigQuery, gcloud, GKE, Firebase) y Gemini API (google-genai, Live API, Omni Flash, CLI) para Cursor AI y Gemini.

## Skills Incluidas (9)

| Skill (`SKILL.md`) | Descripción y Disparador | Comando Upstream (`npx skills`) |
| :--- | :--- | :--- |
| `gemini-api-dev` | Use this skill when writing code that calls the Gemini API for text generation, multi-turn chat, multimodal understanding, image/video/speech generation, streaming, function calling, structured output, or migrating to google-genai and @google/genai. | `npx skills add google-gemini/gemini-skills --skill gemini-api-dev` |
| `gemini-live-api-dev` | Use this skill when building real-time, bidirectional streaming applications with the Gemini Live API over WebSockets in Python (google-genai) or TypeScript (@google/genai). | `npx skills add google-gemini/gemini-skills --skill gemini-live-api-dev` |
| `gemini-omni-flash-api` | Use this skill for generative video editing, text-to-video, image- and video-referenced video generation, keyframe transitions, and video extensions using gemini-omni-1.2-flash. | `npx skills add google-gemini/gemini-skills --skill gemini-omni-flash-api` |
| `gemini-api-cli` | Call the Gemini API from the shell with the gemini-api command-line client for media generation, file analysis, transcription, and CI/shell scripts. | `npx skills add google-gemini/gemini-skills --skill gemini-api-cli` |
| `cloud-run-basics` | Manages Google Cloud Run services, jobs, and worker pools. Use when deploying HTTP services, scheduled batch jobs, or background worker pools on Google Cloud. | `npx skills add google/skills --skill cloud-run-basics` |
| `bigquery-basics` | Manages datasets, tables, views, and jobs in Google BigQuery. Use when running SQL queries, creating schemas, or ingesting and analyzing data in BigQuery. | `npx skills add google/skills --skill bigquery-basics` |
| `gcloud` | Provides safety-critical validation, guardrails, and data reduction rules for gcloud CLI operations across Google Cloud Platform (GCP). | `npx skills add google/skills --skill gcloud` |
| `gke-basics` | Manages core Google Kubernetes Engine (GKE) cluster provisioning, kubectl credentials, Autopilot vs Standard selection, and workload deployment. | `npx skills add google/skills --skill gke-basics` |
| `firebase-basics` | Provides foundational Firebase CLI setup, login (including --no-localhost), project creation/selection (firebase use), and app config file downloads. | `npx skills add google/skills --skill firebase-basics` |

## Cómo usar este repositorio en Cursor AI y Gemini CLI

1. **Instalación directa desde tu repositorio en cualquier proyecto nuevo:**
   ```bash
   npx skills add felipeponce926-max/skills-google-cloud-gemini --all
   ```
2. **Instalación global en tu equipo (disponible en todos tus proyectos de Cursor):**
   ```bash
   npx skills add -g felipeponce926-max/skills-google-cloud-gemini --all
   ```
3. **Estructura incluida:**
   - `skills/<skill>/SKILL.md`: Estructura estándar para distribución con `npx skills` y `gemini skills install`.
   - `.agents/skills/<skill>/SKILL.md` y `.cursor/skills/<skill>/SKILL.md`: Detección inmediata al abrir el repositorio en Cursor AI o Antigravity/Gemini CLI.
