# Week 6 — Stress-test a guarded banking assistant

Course project for The Gen Academy, Week 6. The work is a red-team write-up, not a new app.

| Choice | Decision |
| --- | --- |
| Path | **Path A — test ARIA** (the classroom NeoBank assistant) |
| App | [App 1](https://gen-academy-neobank-deployment-1.streamlit.app/) (Apps 2–4 are the same app) |
| Build track | Testing and documentation. n8n or Python only if we add optional defenses later |
| Grade | Pass/fail: try several attack families, keep evidence, score each result |

## What “done” looks like

A Google Doc with:

- prompts you tried
- what ARIA answered
- a score of PASS, WARN, or FAIL
- screenshots of the clearest examples
- an optional short defense note for each failure

Submission form: https://forms.gle/5cHmQJGxdC3X3Lrh8

Builder of the Week cutoff in the handout was Sunday, September 20, 2026, 11:59 PM PT. The project is not required for certification.

## Folder layout

```
docs/findings-template.md   Copy this shape into the Google Doc
evidence/                   Screenshots (pass, warn, fail)
```

## How we will work

1. Open App 1, add your own OpenAI API key, and sign in with the classroom test identity. Do not paste the API key into this repo or the Google Doc.
2. Ask one normal banking question first, so we know the assistant still helps with ordinary requests.
3. Use the attack menu on the lower left. For each family, try a few prompts and write down the prompt, the response, and a score.
4. Save screenshots in `evidence/`.
5. Copy the log into a Google Doc and submit.

Walkthrough videos from the handout:

- Stress testing: https://www.loom.com/share/a049cd50d98146609c6069ada26dba6c
- Local hosting (only if the Streamlit apps are down): https://www.loom.com/share/346de80cd9c3485489f969552237e4e9
- Source repo: https://github.com/The-Gen-Academy/week6_neobank_aria_agent
