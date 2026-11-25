# Cell Danger Response & The Health Cycle

A curated, human-readable study wiki distilling the **public first half** of:

> A Midwestern Doctor (Jul 5, 2023). ["Systemic Treatments for the Cell Danger Response"](https://www.midwesterndoctor.com/p/systemic-treatments-of-the-cell-danger). *The Forgotten Side of Medicine* (Substack), integrating the Cell Danger Response, Healing Cycle, and Health Cycle work of Dr. Robert K. Naviaux.

*(Note: Only the free public first half of the essay is covered here; the subscriber-only second half detailing specific systemic regenerative therapies is excluded. Read the full original article on [Substack](https://www.midwesterndoctor.com/p/systemic-treatments-of-the-cell-danger).)*

**Live site:** https://iamflipse.github.io/cell-danger-response-wiki/

## Layout

- `src/` — markdown pages (`index.md`, `about.md`, `concepts/`, `reference/`)
- `book/` — generated static `mdbook` output (built locally; published via `gh-pages` branch)
- `tools/mdbook` — local `mdbook` binary (ignored in git)

## Rebuild & Republish

```sh
./tools/mdbook build -d book
git add -A && git commit -m "update" && git push origin main
```

To republish the static site to GitHub Pages, copy `book/*` plus `.nojekyll` into an orphan `gh-pages` branch commit and push to `origin gh-pages`.
