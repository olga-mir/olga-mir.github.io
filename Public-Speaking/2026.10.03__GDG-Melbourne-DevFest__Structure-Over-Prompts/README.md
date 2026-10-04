# Structure Over Prompts: Building an SRE Agent on Gemini Enterprise Agent Platform

We built an automated SRE agent on the Agent Development Kit (ADK) and Gemini Enterprise Agent Platform to investigate end-to-end test failures — parsing logs, diffing source code, and classifying each failure as a genuine bug, a PR regression, or a flake. The first iteration produced answers, but suffered from classic agentic fragility: unbounded execution loops despite token guards, non-deterministic routing through identical errors, and confident hallucinations drawn from a single line of log output.

The fix wasn't a better prompt — it was treating the agent as a software program rather than a series of LLM calls. We encoded the investigation process into the agent's structure: explicit states, typed transitions, and guardrails defined in ADK, bringing determinism to a highly indeterministic system while cutting prompt volume. This talk walks through the production graph topology, the custom tool boundaries, context engineering under tight platform constraints (no persistent volumes — all source access via GitHub APIs), and the inline verifier that forces the agent to be uncertain and honest rather than confident and wrong.

**Event:** [GDG Melbourne DevFest 2026](https://gdgmelbourne.com/devfest/)

**Date:** 3 October 2026

**Location:** William Angliss Institute, 555 La Trobe Street, Melbourne, VIC 3000

**Session:** [Sessionize page](https://gdg-melbourne-devfest-2026.sessionize.com/session/1321201)

## Slides

- [Download PDF (Melbourne, 3 Oct 2026)](./Structure-Over-Prompts-Melbourne-DevFest-2026.pdf)

## Related

This talk was also presented, with significantly updated slides, at [DevFest Sydney 2026](../2026.10.10__GDG-DevFest-Sydney__Structure-Over-Prompts/) (10 Oct 2026).
