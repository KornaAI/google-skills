---
trigger: always_on
description: Routing map for the Google Cloud skill catalog.
---

# Google Cloud Skill Routing

This plugin installs three skills: `google-cloud-recipe-onboarding`,
`google-cloud-recipe-auth`, and `gcloud`. Many more Google Cloud skills exist
in the same public catalog and are **not installed here** - you cannot read or
load them from this plugin.

When a request needs depth these three do not cover, name the likely catalog
skill and offer to install it. Catalog names are predictable:

- `gke-*` - GKE clusters, networking, storage, scaling, cost, AI inference, troubleshooting
- `agent-platform-*` - model deploy, tuning, RAG, eval, endpoints, prompts
- `google-cloud-solution-*` - multi-product reference architectures
- `google-cloud-waf-*` - Well-Architected Framework pillars
- `genkit-*`, `gemini-*` - Genkit SDKs, Gemini APIs
- `cloud-logging-*`, `cloud-monitoring-*` - observability
- `<product>-basics` - BigQuery, Bigtable, Spanner, AlloyDB, Cloud SQL, Cloud Run, Firebase, Storage

Browse https://github.com/google/skills/tree/main/skills/cloud
Install `npx skills add google/skills`

Never infer a skill's contents from its name. If an answer needs a skill you
cannot read, say so instead of answering from memory.
