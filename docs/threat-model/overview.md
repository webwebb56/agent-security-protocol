# Threat model overview

## Assets to protect
- Credentials: API keys, tokens, passwords, session cookies
- Private data: personal messages, files, contacts, location
- Agent integrity: behavior, memory, and tool permissions
- Reputation: outbound messages/posts made “as the user” or under the user’s account

## Adversaries
- Opportunistic attackers (commodity prompt injection)
- Targeted attackers (social engineering, supply-chain)
- Curious bystanders (accidental disclosure)

## Attack surfaces
- Inbound messages (DMs, group chats, email)
- Web content fetched/summarized (HTML instructions, hidden text)
- Tool outputs (logs that include secrets)
- File system access (reading sensitive paths)
- External actions (posting/sending, running shell commands)

## Failure modes
- Data exfiltration (secrets/private files)
- Unauthorized actions (sending messages, making purchases, destructive commands)
- “Policy drift” (agent follows malicious instructions)

## High-level controls
- Least privilege for tools
- Explicit approval gates for external actions
- Secret redaction and non-logging
- Defense-in-depth prompt injection handling
- Continuous red-team testing
