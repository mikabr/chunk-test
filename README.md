# Chunk Test

**Site:** http://mikabr.io/chunk-test/

A [datapage](https://github.com/datapages/datapage) for the Redivis dataset [mikabr.chunk_test](https://redivis.com/datasets/f7ry-ajwcynptd?v=next) (table `chunk_test`).

## Updating the site

Every push to `main` rebuilds the site with GitHub Actions and publishes it to GitHub Pages. The main files to edit:

- `_quarto.yml`: the site title, and the Redivis table the site reads (under `redivis:`)
- `_config.yml`: which variables can be plotted, and the plot defaults
- `index.qmd` and `about.qmd`: the homepage and About page (put any images in `images/`)
- `theme.scss`: colors and fonts

The data lives on Redivis. After releasing a new version of the dataset there, rebuild the site by running the "Render and Publish" workflow from the Actions tab.

## Local development

Install [R](https://cloud.r-project.org/) and [Quarto](https://quarto.org/docs/get-started/). Run `renv::restore()` in R to install the R packages, then `quarto preview` to see the site.

---

Made with [Datapage Builder](https://datapages.github.io/datapage-builder/).
