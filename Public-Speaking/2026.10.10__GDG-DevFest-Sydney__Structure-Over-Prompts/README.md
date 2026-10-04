# Structure Over Prompts: Building an SRE Agent on Gemini Enterprise Agent Platform

We built an automated SRE agent on the Agent Development Kit (ADK) and Gemini Enterprise Agent Platform to investigate end-to-end test failures — parsing logs, diffing source code, and classifying each failure as a genuine bug, a PR regression, or a flake. The first iteration produced answers, but suffered from classic agentic fragility: unbounded execution loops despite token guards, non-deterministic routing through identical errors, and confident hallucinations drawn from a single line of log output.

The fix wasn't a better prompt — it was treating the agent as a software program rather than a series of LLM calls. We encoded the investigation process into the agent's structure: explicit states, typed transitions, and guardrails defined in ADK, bringing determinism to a highly indeterministic system while cutting prompt volume. This talk walks through the production graph topology, the custom tool boundaries, context engineering under tight platform constraints (no persistent volumes — all source access via GitHub APIs), and the inline verifier that forces the agent to be uncertain and honest rather than confident and wrong.

**Event:** [DevFest Sydney 2026](https://devfest.gdgsydney.com/)

**Date:** 10 October 2026

**Location:** Torrens University, Shop 1/37 Foveaux St, Surry Hills, NSW 2010

## Slides

_Coming soon — the Sydney deck is a significant revision of the talk, not a repeat of the Melbourne version. Will be published after the session (10 Oct 2026)._

## Related

This talk was first presented at [GDG Melbourne DevFest 2026](../2026.10.03__GDG-Melbourne-DevFest__Structure-Over-Prompts/) (3 Oct 2026).
