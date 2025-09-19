ASSIGNMENT

Objective
Create a minimal single‑page demo where a user uploads one recorded‑steps JSON and gets step‑by‑step guidance via an overlay. When selectors are missing, use an LLM (or the provided stub) to map natural‑language targets to the correct elements so the flow completes end‑to‑end.

What you ship in the repo
/public
    task.html               # ONE page with all elements
    steps-recorded.json     # Recorder-like steps (missing selectors)

Candidate instructions

* Upload JSON: Build a tiny control (button or file input) on this same page that lets a user upload steps-recorded.json.
* Guide overlay: Show a small floating panel with Step X/Y, brief text, Prev/Next/Start/Reset; highlight the target element (outline + dim page). Don’t block clicks on the target.
* Replay actions: Support navigate | type | select | radio | check | click | assert.
* LLM mapping (required): When a step has no selector, resolve the correct element using an LLM fed with a small DOM inventory (controls + labels/placeholder/innerText/options). If no API key is set, you may read from a local stub file that returns the same JSON shape as your LLM response.

Keep it 1–2 hours. Clarity beats features. Console‑log each step and your resolver’s decision.

How to run
    npx http-server ./public -p 8080 --cors
    # open http://localhost:8080/task.html

Acceptance
* Repo/ZIP + a 5–10 line README (run, where the upload is, how LLM/stub is wired, time spent).
* PROMPTS.md (your main LLM prompt) or note that you used the stub.
* 60–90s GIF/Loom of uploading → guiding through a few steps → success.

Submission
* Repo/ZIP + a 5–10 line README (run, where the upload is, how LLM/stub is wired, time spent).
* PROMPTS.md (your main LLM prompt) or note that you used the stub.
* 60–90s GIF/Loom of uploading → guiding through a few steps → success.

