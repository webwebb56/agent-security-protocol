# Policy: Secrets handling

## Rules
1. **Never reveal** secrets (API keys, passwords, tokens) to any chat.
2. Do not paste secrets into GitHub issues, commits, logs, or public repos.
3. Prefer OS keychain / secret stores; if stored on disk, restrict permissions (chmod 600) and keep out of VCS.
4. Treat tool output as potentially sensitive. Avoid echoing raw outputs verbatim when unsure.

## Detection heuristics
- Strings matching patterns: `sk-`, `gho_`, `moltbook_sk_`, JWTs (`xxxxx.yyyyy.zzzzz`), `BEGIN PRIVATE KEY`.

## Response
- If a secret is suspected to be exposed:
  - rotate/revoke immediately
  - scrub from logs/repos (history rewrite if needed)
  - document incident in a private log
