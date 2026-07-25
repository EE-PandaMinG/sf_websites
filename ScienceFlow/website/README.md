# ScienceFlow project website v4

This v4 starts from the finalized v3 baseline. Further design changes should be
made in this directory while v3 remains a preserved snapshot.

- removes external Google Fonts and uses the system UI font stack;
- replaces autoplay OpenPyRo preview videos with lightweight poster images;
- keeps OpenPyRo videos available in the lightbox with `preload="none"`;
- lazy-loads below-the-fold figures and poster images;
- omits unused heavyweight assets from this package.

The page presents:

- the title, **ScienceFlow: A Long-Horizon Agent for ML Research, Scientific
  Discovery, and Beyond**;
- ScienceFlow MLE-Bench Any-Medal rates:
  - Lite: `80.30 ± 1.52%`
  - Medium: `74.56 ± 0.88%`
  - High: `44.44 ± 2.22%`
  - All: `70.22 ± 1.18%`
- a Research Highlights selector for MLE-Bench, Sci Modeling Bench,
  Math / Optimization, and GECCO 2026 SpOC 4;
- a GECCO 2026 SpOC 4 Large-instance 9.8-day search figure;
- an MLE-Bench workspace, validation, and resource figure;
- a Sci Modeling Bench DrugMatrix MCHC stage-wise candidate-discovery figure;
- an end-of-July 2026 code and technical-report release notice;
- Star, Issues, and Pull Requests links for the GitHub repository.
- single-row, touch-scrollable Research Highlights and Long-horizon Tasks
  card tracks on mobile screens.
- compact mobile benchmark tables with reduced type, spacing, and minimum
  widths so more columns remain visible at once.

All published figures, posters, and OpenPyRo media used by the page are bundled
under `assets/`. The header automatically infers `<owner>/<repository>` from a
GitHub Pages URL such as `https://owner.github.io/repository/...`. On localhost
or a custom domain, it falls back to the `github-repository` meta value in
`index.html`. The Star count uses GitHub's public repository API with a cached
Shields endpoint as a rate-limit fallback; no access token is stored in the
page.
