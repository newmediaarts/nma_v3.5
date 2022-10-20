# NMA v3.5 - A Simplified Eleventy Static Site
Another static version of the NMA site, built/staticly generated using [11ty](https://www.11ty.dev/), but this one is designed to be bare bones simple and 100% pre-rendered (e.g. no native web components).

[View Demo on Github Pages](https://newmediaarts.github.io/nma_v3-5/dist/) - (not working)

## Goals/Constraints:
* minimal config (easy to understand and get up and running right out of the box)
* support for relative paths via a found "Relbase" liquid hack/work-around (e.g. enabling the site to be staticly hosted in any sub-directory)
* Other key features:
    * html includes (via [nunjucks](https://mozilla.github.io/nunjucks/)/liquid)
    * html files with mixed front matter + markup (thank you eleventy)

##  Local pre-requisites:
Make sure you have node and npm installed. See installation docs: (https://nodejs.org/en/). To confirm node and npm are installed:
```
    node -v
    npm -v
```

## To install, setup, & serve locally

``` npm run dev ```

or:

``` npx @11ty/eleventy --serve ```

## To-do Wish List
* need to fix github pages (not working)
* figure out a system for docs (improve the readme for now)
* establish a baseline multi-page site with content from [existing nma website](https://kccnma.site/)
* migrate/copy over content from [latest nma wordpress site](https://kccnma.site/home)
* create reusable components/partials (need to establish how to best to do, e.g. nunjucks blocks or macros etc.)
* add support for sass
* add prettier and vs code workspace settings to ensure consistent formatting (temp fix = disable auto-format-on-save via VS Code manually, for now)
* add a contributing.md file and github workflow (e.g. branching > pr)
* add support for taxonomy collections (e.g. categories + tags ) if we add any of the following sections/features:
    * nma news (blog)
    * nma gallery (of student projects)