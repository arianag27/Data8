# CSCI 9 — JupyterLite 

[![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://jupyterlite.rtfd.io/en/latest/)

Run **CSCI 9** lecture and lab notebooks in the browser—no local install required. All materials live under **`csci9-sp26-student/`** in the file browser.

## Materials layout

| Area | Path |
| --- | --- |
| Lectures | `csci9-sp26-student/lecture/` |
| Labs | `csci9-sp26-student/lab/` |
| Course index | `csci9-sp26-student/README.md` |

## Home page

The deployed site uses a **weekly schedule** on the home page with links into each notebook (`./lab/index.html?path=csci9-sp26-student/...`). Adjust dates and ordering in `landing/index.html` to match your syllabus.

## Local build (optional)

```bash
micromamba create -f .github/build-environment.yml
jupyter lite build --contents content --output-dir dist
cp landing/index.html dist/index.html
```
