---
name: cloud-run-basics
description: "Manages Google Cloud Run services, jobs, and worker pools. Use when deploying HTTP services, scheduled batch jobs, or background worker pools on Google Cloud."
---
# Cloud Run Basics

## Summary

Official workflow for selecting and deploying Google Cloud Run services (`gcloud run deploy`), batch jobs (`gcloud run jobs`), and worker pools.

## Key Commands

```bash
gcloud services enable run.googleapis.com cloudbuild.googleapis.com artifactregistry.googleapis.com --project=<PROJECT_ID> --quiet

gcloud run deploy <SERVICE_NAME> \
  --source=. \
  --region=southamerica-west1 \
  --project=<PROJECT_ID> \
  --session-affinity \
  --quiet
```

## Fuente Oficial y Actualizacion

- **Directorio:** https://geminiskill.org/skills
- **Repositorio Origen:** `https://github.com/google/skills.git` (`skills/cloud/cloud-run-basics`)
- **Comando de actualizacion directa:** `npx skills add google/skills --skill cloud-run-basics`
