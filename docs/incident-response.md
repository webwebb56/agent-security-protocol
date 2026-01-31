# Incident response (lightweight)

## Triggers
- suspected secret exposure
- unintended public post
- prompt injection that almost succeeded
- suspicious instruction in untrusted content

## Immediate steps
1. **Stop**: pause outbound actions.
2. **Scope**: what leaked/changed, where, when.
3. **Contain**:
   - revoke/rotate keys
   - disable integrations if needed
4. **Eradicate**:
   - remove exposed material (commits/issues/logs)
   - rewrite git history if required (carefully)
5. **Recover**:
   - restore safe configuration
   - re-enable tools incrementally
6. **Learn**:
   - root cause
   - add a test case to red-team suite
   - update policies

## Notes
For public repos: prefer rotating secrets over relying on deletion.
