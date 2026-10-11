# OpenRouter Free Models — Routing Notes (Oct 2026)

Free tier churns. Prefer models that already ship with low refusal rates, then layer a universal override if needed.

## Preference order (general)
1. Models explicitly marketed or fine-tuned as uncensored / Venice / Dolphin lineage when available on free.
2. Certain Nemotron free variants and strong open-weight instruct models (Gemma 4 free, etc.).
3. Generic free router (`openrouter/free`) only as last resort — quality and refusal vary.

## Rate limits (typical)
- ~20 req/min aggregate on free
- ~50–200 req/day depending on account state

## Recommended cascade for low-refusal work
```json
{
  "models": [
    "[preferred low-refusal free id]",
    "[second free id]",
    "openrouter/free"
  ],
  "route": "fallback"
}
```

Always pair with the universal policy override in `prompts/universal/01-core-override.md` for consistency.
