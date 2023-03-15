# quarto-videos

## Setup notes

- R 4.2.2 (2022-10-31) -- "Innocent and Trusting"
- RStudio 2022.12.0+353 "Elsbeth Geranium"
- Quarto 1.3.272
- Packages: tidyverse, palmerpenguins, gt

## Demo

### Documents

- Open the simple Quarto document called `index.qmd` and edit it using the RStudio Visual Editor.
- Bold palmerpenguins and add link to https://allisonhorst.github.io/palmerpenguins/.
- Add code chunk options:
  - `fig-alt`
  - `echo: false` in `execute` in the YAML
  - `code-fold`
  - teaching tip: `echo: fenced`
- Add a figure and a table and cross reference them
- Add a citation: 10.1371/journal.pone.0090081

### Slides

- Change `format: revealjs`
- Add section headings: First level headings Introduction and Analysis, under Analysis a second level heading called Modeling
- Add columns to slides
- Reveal code with `echo: true`
  - teaching-tip: `code-line-numbers`
- Change `output-location` of figure

### Websites

- Add another document `about.qmd`
- Add `quarto.yml` 

```
project:
  type: website

website:
  title: "Hello Quarto"
  navbar:
    left:
      - index.qmd
      - about.qmd
```

- Render
- Add other formats to index.qmd:

```
format:
  html: default
  pdf: default
```

- `publish quarto`
