# Brief for agents editing docs.madeformeai.com

1. Audience: a small-business owner or their staff whom Quick IT Projects has already set up. They arrived from a direct link in an email. They are not shopping.
2. The rules in STYLE-CONTRACT.md apply to every page. Read it before writing.
3. Pages are guides, not marketing. One task per page, numbered steps, an "If this fails" section at the end.
4. No infrastructure: no internal hostnames, IPs, topology, env vars, API routes, or the names of internal services.
5. No customer names, tenant names, or any other customer's details.
6. No sales language, no pricing, no "coming soon", no comparisons to other products.
7. No em dashes. Use a comma or a period.
8. Facts come only from the source files named in the task. If a source does not say it, do not write it.
9. Never guess a menu label. Describe the location if the label is unknown.
10. Keep existing screenshots, video embeds, and mermaid blocks in place. Never invent an image path.
11. Links between pages are root-relative Mintlify links.
12. Valid YAML frontmatter on every page: a short title and a one-sentence description.
13. Run `bash scripts/docs-leak-scan.sh` before every push. It must print CLEAN.
14. Pushing `main` deploys the live site, so preview with `mint dev` when in doubt.
15. Support contact on every page that needs one is support@madeformeai.com. No chat or community invite links.
