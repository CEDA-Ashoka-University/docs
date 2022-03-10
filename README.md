# Documentation for CEDA Software & Systems
## Introduction
This is a site built on [Mkdocs](https://www.mkdocs.org/) and hosted on GitHub Pages to document code as well as processes for CEDA's tools and systems, and to serve as a learning point for those trying to build similar systems.

The site is hosted at [docs.ceda.ashoka.edu.in](https://docs.ceda.ashoka.edu.in).

Please document all software tools and their processes here for efficient knowledge transfer.

## Contributing to these docs
Mkdocs parses Markdown files using python-markdown to generate pages - you'll write your pages as .md files and save it in the `docs` folder. Any commit to the `main` branch will trigger a rebuiid of the website using GitHub Actions (see `.github/workflows/deploy.yml`).

Checkout the `main branch`, commit your .md files to the `docs` folder, and submit a Pull Request to merge into `main`.

Please refer to [this cheatsheet](https://www.markdownguide.org/cheat-sheet/) for a quick overview of Markdown syntax.

Please refer to [this guide](https://www.mkdocs.org/user-guide/writing-your-docs/) on structuring your pages in Mkdocs.

## Setting up this site
### Local
Clone the repository contents, ensure Python 3.8+ is installed on your system, and run `pip install -r requirements.txt`. You can test the site using `mkdocs serve`, and generate pages through `mkdocs build`.

### On GitHub Pages
Before you add files to your GitHub repo, ensure that you have created a branch called `gh-pages`. **Keep this branch empty**.

Upload this repository's contents on another branch. GitHub will recognise the `deploy.yml` Actions Workflow within and build the site. The built site will be hosted off the gh-pages branch.

Go to your repository's settings and enable Pages, with gh-pages being the root branch.

## Extending the site's functionalities
You can install extensions for both Mkdocs and python-markdown to extend the site's functionalities, which are in the form of Python PIP packages. 

Add the package name and version to `requirements.txt`, and then run `pip install -r requirements.txt` (for local development) or push it to the repo (for deployment on-site).
