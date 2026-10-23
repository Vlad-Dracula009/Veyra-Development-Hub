# Veyra Project Bible

## Vision
Veyra is intended to become a cross-platform personal AI assistant for Android, iOS, Windows, and Mac. The longer-term plan includes OpenAI, Anthropic/Claude, Google/Gemini, assistant agents named Luna, Sol, and Terra, and eventually a distinct Veyra model and voice.

## Development environment (from the supplied handoff)
- OS: Windows 11
- Project root: `C:\Users\Onojeta Fortune\Projects\veyra`
- Backend directory: `C:\Users\Onojeta Fortune\Projects\veyra\backend`
- Runtime: Node.js
- Backend: TypeScript + Express
- Package manager: npm
- In PowerShell, use `npm.cmd` if `npm.ps1` is blocked by execution policy.
- Build command: `npm.cmd run build`

## Provider integration files reported in the handoff
- `src/models/anthropicProvider.ts`
- `src/models/geminiProvider.ts`
- `src/models/providerRegistry.ts`
- `src/models/modelGateway.ts`
- `src/models/model.ts`
- `src/models/modelRegistry.ts`
- `src/models/index.ts`
- `src/models/providerHealth.ts`

Provider names reported: `openai`, `anthropic`, `gemini`, and `mock`.

## Development preferences and guardrails
- Work step by step.
- Make one code change at a time, then build/test before continuing.
- Keep explanations reasonably concise and beginner-friendly.
- Never ask for or expose API key values.
- Do not enable billing or purchase credits unless the user explicitly asks.
- During investigation, keep code unchanged unless the user authorizes a change.
- Distinguish the regular consumer Claude/Gemini apps from their developer APIs. The apps can be used manually as coding partners; API calls made by Veyra are a separate integration and may incur costs.

## Source of truth
The actual Veyra source code remains in the user's local project (and any separate source-code repository they choose). This repository is a documentation and collaboration hub; do not assume these notes are a complete copy of the codebase.
