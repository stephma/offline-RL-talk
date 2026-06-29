# Offline RL Talk

LaTeX Beamer deck for a 60-minute internal technical talk:

**From Control to Offline Reinforcement Learning: Learning Better Decisions from Logged Data**

## Build

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Or use:

```bash
latexmk -pdf main.tex
```

## Structure

- `main.tex`
- `sections/00_title.tex`
- `sections/01_motivation.tex`
- `sections/02_control_to_rl.tex`
- `sections/03_mdp_value_functions.tex`
- `sections/04_online_and_model_based_rl.tex`
- `sections/05_offline_rl.tex`
- `sections/06_bc_awr.tex`
- `sections/07_iql_idql.tex`
- `sections/08_product_checklist.tex`
- `refs.bib`

## Grain terminal example

The introduction uses a running grain-terminal example:

- decisions over truck selection, unloading pits, conveyor routes, silos, blending, and train loading
- logged terminal operator decisions as the offline data source
- delayed operational outcomes such as congestion, rehandling, train delay, and loading penalties
