# Dataset Preparation Guides for the EDI Community

This repository contains a series of documents about preparing and publishing datasets in the environmental sciences and similar contexts. Topics include community-developed metadata standards, serialization and markup formatting guidelines, and best practices for the content of published research datasets. This documentation is maintained by the [Environmental Data Initiative](https://edirepository.org) (EDI) and all content has been developed and written in coordination with EDI's community of scientists, data managers, and repository users. There are two versions published online:

* [The current production version](https://ediorg.github.io/dataset_preparation_guides/)
* [A pre-release version](https://prerelease-edi-docs.netlify.app) (in development)

**NOTE: Content in the current production version was originally taken from EDI's [*Data Package Best Practices*](https://ediorg.github.io/data-package-best-practices/) site ([repo](https://github.com/EDIorg/data-package-best-practices))**

The guide documents are published as a collection of [Quarto books](https://quarto.org/docs/books). Revisions to these guides will occur using this repository, with periodic releases and distribution of PDF copies.

# Contributing

This repository and the included documents are currently maintained by EDI, with major updates and new content developed and approved through community working groups. If you would like to help develop these documents please contact the maintainers and working group leads listed on the "About" page, or reach out to EDI at [info@edirepository.org](mailto:info@edirepository.org>). Some details on how contribution works are below.

## Branches

* **main**: The `main` branch holds the current production version of the documents. Documents in the main branch are published in website format with GitHub Pages in the "EDIorg" organization. This constitutes the 
* **prerelease**: The `prerelease` branch contains the in-development, "next version" of the documents. Documents in the prerelease branch are published in website format on Netlify.
* **feature** or **content** branches: These may exist during the early development of new features or drafting of content. They will first be merged into the _prerelease_ branch and they are not currently published in website form.

## Drafting and proposing changes

All documents and website content are written in Quarto markdown and the resulting`.qmd` files are rendered to the websites (as HTML files, ultimately). See the [Quarto guide](https://quarto.org/docs/guide/) for information on how to author `.qmd` files. New content or edits to the documents should be submitted as a pull request to the prerelease branch. Once merged into the prerelease version, changes will be reviewed by the community and approved (or not) for inclusion in the production documents. If you would like push permission to the `prerelease` branch please contact the maintainers.

## Publishing workflow

Both `main` and `prerelease` branches have GitHub Actions workflows configured to build and deploy their associated website any time new commits are pushed to that branch. The production site, derived from `main`, is published as a GitHub pages site ([Quarto docs](https://quarto.org/docs/publishing/github-pages.html#github-action)). The prerelease site, derived from the `prerelease` branch, is published to Netlify ([Quarto docs](https://quarto.org/docs/publishing/netlify.html#github-action)). The GitHub Actions publishing workflow for both branches is specified in the [`.github/workflows/publish.yml`](.github/workflows/publish.yml) file, which was modeled in part on the [Quarto website version](https://github.com/quarto-dev/quarto-web/blob/main/.github/workflows/publish.yml).


