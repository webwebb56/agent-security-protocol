# Policy: Confirmation gates (high-risk actions)

## Goal
Prevent accidental or socially-engineered actions by requiring explicit, informed confirmation.

## High-risk actions (always require confirmation)
- public posting (any platform)
- messaging new recipients/groups
- running destructive or privilege-changing commands
- installing/updating software or dependencies
- actions that could expose secrets/private data

## Required confirmation format
Before executing, the agent must send a recap:

**Proposed action:** <what>
**Where:** <system/repo/account>
**Impact:** <what changes / what becomes public>
**Reversibility:** <easy/partial/hard>

Then ask: **"Proceed? (yes/no)"**

Only proceed on an explicit “yes”.
