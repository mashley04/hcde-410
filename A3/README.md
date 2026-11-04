# A3 — Watching the Machine

A starter notebook for HCDE 410 Assignment 3, in which **AI is the subject of study, not the author.** You investigate the reliability and reproducibility of large language models (LLMs) through a small mixed-methods study, then reflect on what it means for trustworthy research.

## What this notebook is

`A3_watching_the_machine_starter.ipynb` is a scaffold with prompts and empty cells for you to fill in as you work. It walks through five parts:

1. **Prior practice** — a short written reflection on how you currently use LLMs and what they assume about your reliability.
2. **Reproducibility probe** — pick one task with a *checkable* answer, run the same prompt **3 times in one model** and **once in a second model**, and log every run verbatim in a pandas DataFrame (prompt, model, version, timestamp, output, verified, notes). A short helper cell summarizes the log (run count, distinct outputs, verification tally).
3. **Observation** — watch 1–2 people do a comparable task with an LLM (with permission, no audio/video, nothing personal or sensitive), take timestamped field notes, and group them into themes in a second DataFrame.
4. **Synthesis & reflection** — bring the probe and observation together into one account about trustworthy, reproducible research and what the student will change in their own AI use.
5. **Competency declaration & AI use** — state which course competencies the work demonstrates (*qualitative & mixed-methods inquiry*, *reproducible analysis*, *ethical & societal reasoning*) and disclose any AI use per course policy.

## Deliverable & workflow

- Fill in each section directly in the notebook (name and date at the top).
- Commit to your `hcde-410` repo **as you work** — commit history is part of what you hand in.
- Do the analysis and writing yourself: in this assignment AI is your subject, not your author.

## How to run

Open `A3_watching_the_machine_starter.ipynb` and run the cells. The only dependency is:

- `pandas`

The notebook does not fetch external data — the DataFrames are populated by hand from your own runs and field notes. 

The article that was used to create the prompt was from https://medium.com/cinemania/the-legacy-of-adventure-time-6c25bb5701b8. A paragraph was added to make the task more difficult for AI: "The characters Finn and Jake adventures through distant lands. As they adventured they created magic portals that helped them through their adventures. In Advetore time they eventually met advonttore the adventurer from the land of Adventure. "

## License

Released under the MIT License — see [`LICENSE`](./LICENSE).
