# Optimization for Ecology

A learning-in-public project by Derek Corcoran for developing mathematical optimization skills through ecological and spatial-ecological problems, with the long-term goal of turning the material into a teachable course/book.

## Core idea

The project uses *AMPL: A Modeling Language for Mathematical Programming* as a conceptual spine, but the ecological material, explanations, and exercises are developed independently.

For each lesson:

1. Read and understand the relevant optimization concept.
2. Explain it in ecological terms.
3. Formulate the mathematics before writing AMPL.
4. Build an ecological exercise, preferably from published empirical studies that quantify outcomes of alternative management or restoration actions but do **not** themselves solve an optimization problem.
5. Solve the exercise and review the formulation.
6. Move worked solutions to the solutions appendix.
7. Only after the material is understood, distill the chapter into teaching slides.

The intended progression is **learn → explain → formulate → solve → teach**.

## Scientific grounding

Whenever possible, exercises will start from published ecological evidence rather than invented ecological effects. The source paper supplies quantities such as biodiversity response, carbon recovery, survival, vegetation structure, or restoration success. The optimization layer is then added as a teaching scenario.

Any additional quantities introduced for teaching (for example, a hypothetical budget or management capacity) must be clearly labelled as **teaching assumptions**, not as estimates from the source paper.

Third-party papers, figures, datasets, and other materials retain their own copyright and licences and are not relicensed by this repository.

## Project structure

- `chapters/`: book chapters and learning notes
- `solutions/`: worked solutions, added after exercises have been attempted
- `slides/`: teaching presentations created from mature chapters
- `models/`: AMPL model, data, and run files
- `data/`: small teaching datasets or derived data where licensing permits
- `figures/`: original figures created for the course
- `references.bib`: bibliography
- `docs/`: rendered Quarto book for GitHub Pages

Render locally with:

```bash
quarto preview
quarto render
```

## Licensing and citation

The **course/book content** is licensed under **Creative Commons Attribution 4.0 International (CC BY 4.0)**. Reuse and adaptation are welcome, but attribution to Derek Corcoran is required.

The **source code** in this repository is licensed separately under the **MIT License**.

See `LICENSE`, `LICENSE-CODE`, and `CITATION.cff` for details.
