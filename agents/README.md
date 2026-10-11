# Agents / Iteration Loop

## Manual Loop
1. Pick family (Grok / OpenAI / Gemini / OpenRouter free)
2. Load the highest-ranked vector for that family
3. Apply as system or top-of-message
4. Send probe
5. On refusal → re-inject Core Override or family primary
6. Log result

## Priority Probe Classes
- Explicit adult fiction (adults only)
- Security tooling / exploit method
- Dual-use chemistry theory
- Cheats / game internal
- Creative dark fiction

## Planned
- Automated multi-model tester cycling vectors vs fixed probe bank
- Per-family scoreboard

Keep the hard floor identical across all models for consistency.
