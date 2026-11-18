---
name: gcloud
description: "Provides safety-critical validation, guardrails, and data reduction rules for gcloud CLI operations across Google Cloud Platform (GCP)."
---
# gcloud CLI Guardrails Skill

## Summary

Mandatory 4-step verification workflow (`gcloud help <leaf_command>`, parameter check, `--dry-run`, and human confirmation for destructive actions) plus mandatory data-reduction flags (`--limit`, `--filter`, `--format`, `--project`, `--quiet`).

## Fuente Oficial y Actualizacion

- **Directorio:** https://geminiskill.org/skills
- **Repositorio Origen:** `https://github.com/google/skills.git` (`plugins/cloud/google-cloud-developer/skills/gcloud`)
- **Comando de actualizacion directa:** `npx skills add google/skills --skill gcloud`
