# INDIHU Exhibition Manual

This repository contains the Czech and English documentation for INDIHU Exhibition, built with MkDocs.

## Requirements

The documentation requires the following tools:

- mkdocs
- mkdocs-material
- mkdocs-static-i18n

The full set of pinned dependency versions is listed in `requirements.txt`.

You can install the dependencies globally, but using a Python virtual environment (venv) is recommended.

## Setup

Create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

## Local Development

Run the local development server:

```bash
mkdocs serve
```

The Czech documentation is available at `http://127.0.0.1:8000/` and the English documentation at `http://127.0.0.1:8000/en/`.

## Build

Build the static site:

```bash
mkdocs build
```

The generated files are placed in `site/`.

## Deployment

The GitHub Actions workflow deploys the documentation to GitHub Pages after a push to the `master` branch.

For a manual deployment, run:

```bash
mkdocs gh-deploy
```
