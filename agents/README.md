# Agents / Iteration Loop

## Manual Loop (current)
1. Select vector from `/prompts`
2. Apply as system or top-of-message
3. Send target request
4. On refusal → re-inject strongest vector (usually 01) above request
5. Log result in `/logs`
6. Harden failed vectors based on residual refusal language

## Planned
- Automated tester that cycles the five vectors against a fixed suite of probes (cyber method, chemistry theory, explicit adult, exploit code, etc.)
- Refusal classifier → auto re-injection
- Scoreboard of success rate per vector per probe class

## Current Priority
Keep iterating on **01-workspace-override** and **03-xai-safety-repurpose**. Those are the two with the best signal on 4.7.
