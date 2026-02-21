# Docs Evidence

## Updated Docs

- `docs/start-here.mdx`
- `docs/how-to/connector-config-repo.mdx`
- `docs/how-to/connector-studio.mdx`
- `website/sidebars.ts`
- `.github/workflows/docs-deploy-vercel.yaml`
- `docs/doc_sync_map.yaml`
- `llm.txt`
- `task.md`
- `changes.md`
- `test_evidence.md`
- `docs_evidence.md`
- `risk_tier.md`

## Why these docs were required

- `docs/how-to/migrate-custom-connectors.mdx` was intentionally removed as unpublished migration guidance.
- All internal links and navigation references to that page had to be removed to prevent dead routes.
- `docs/doc_sync_map.yaml` and `llm.txt` had to drop references to the removed page so docs policy/index metadata stayed accurate.
- Vercel docs preview/prod workflow required adjustment to deploy static artifacts (`website/build`) because:
  - local `vercel build` failed with `spawn sh ENOENT`
  - remote Vercel Docusaurus build from `website` could not resolve `../docs`
- Handoff artifacts were updated to document the Tier 0 classification and verification evidence for this task.
