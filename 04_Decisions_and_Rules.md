# Decisions and Rules

## Accepted decisions
- Use GitHub as the shared development documentation hub.
- Start with manual, organized collaboration; no integrations for now.
- Keep the regular ChatGPT, Claude, and Gemini apps as separate collaborators.
- Do not modify existing Veyra code during the current investigation.
- Do not enable API billing or purchase API credits.
- Use one change at a time and test after each authorized code change.

## Do not assume
- A successful `/api/development/review` response does not prove both providers succeeded.
- Provider cooldowns do not fix remote quota or credit problems.
- The model IDs listed in the handoff are not confirmed live merely because they are present in the local registry.
- The source of `UND_ERR_HEADERS_TIMEOUT` is unknown until logs identify the provider/request and useful timing evidence is available.
- A GitHub repo does not automatically synchronize context into each consumer AI app.

## Decision log template
For each decision, record:
- Date:
- Task:
- Options considered:
- Evidence:
- Decision:
- Why:
- Tests required:
- Status: proposed / accepted / rejected / deferred
