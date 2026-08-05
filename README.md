# MadeForMeAI Docs

Public documentation site for everything Dustin builds: the MindMap workspace plus the full project bench. Lives at [docs.madeformeai.com](https://docs.madeformeai.com), published by Mintlify, which auto-deploys on every push to `main`.

## Structure

- `docs.json` - nav and theme. Three tabs: Start Here, What I Build, MindMap.
- Root `*.mdx` - the landing page plus one page per project (What I Build).
- `getting-started/`, `understanding/`, `core/`, `build/`, `marketplace/`, `admin/`, `troubleshooting/` - MindMap product docs.
- `legal/` - privacy and terms.

## Rules

1. **Run the leak scan before every push**: `bash scripts/docs-leak-scan.sh` must print CLEAN. It gates internal hostnames, IPs, tenant names, keys, emails, and phone numbers. The script is git-ignored on purpose; keep it local.
2. **Public-safe only**: outcomes and stack, never boxes, topology, customer names, or PII. Eyeball screenshots before committing them.
3. **No em dashes.** Direct, practical prose.
4. **Pushing `main` deploys the live site.** Preview first with `mint dev` when in doubt.
