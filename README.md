# Agent Security Protocol

A practical, version-controlled security playbook for operating tool-using AI agents.

## Goals
- Reduce risk from **prompt injection**, social engineering, and malicious content.
- Prevent accidental leakage of **secrets** (API keys, passwords, private files, personal data).
- Define **operational controls** (permissions, review gates, logging, incident response).

## Scope
This repo documents controls and procedures. It cannot guarantee safety, but it can make failures rarer, smaller, and easier to detect.

## Contents
- `docs/threat-model/` — assets, adversaries, attack surfaces
- `docs/policies/` — rules the agent/system must follow (data handling, external comms, tool use)
- `docs/red-team/` — tests and scenarios to continuously evaluate the setup

## Quickstart
1. Read: `docs/threat-model/overview.md`
2. Adopt: `docs/policies/secrets-handling.md` + `docs/policies/prompt-injection.md`
3. Run: `docs/red-team/prompt-injection-suite.md`

## License
MIT
