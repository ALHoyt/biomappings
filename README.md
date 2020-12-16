<p align="center">
  <img src="docs/source/logo.png" height="150">
</p>

<h1 align="center">
  Biomappings
</h1>

<p align="center">
    <a href="https://github.com/biomappings/biomappings/actions?query=workflow%3A%22Check+mappings%22">
        <img alt="Check mappings" src="https://github.com/biomappings/biomappings/workflows/Check%20mappings/badge.svg" />
    </a>
    <a href="https://pypi.org/project/biomappings">
        <img alt="PyPI" src="https://img.shields.io/pypi/v/biomappings" />
    </a>
    <a href="https://pypi.org/project/biomappings">
        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/biomappings" />
    </a>
    <a href="https://github.com/biomappings/biomappings/blob/main/LICENSE">
        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/biomappings" />
    </a>
    <a href="https://zenodo.org/badge/latestdoi/285352907">
        <img src="https://zenodo.org/badge/285352907.svg" alt="DOI">
    </a>
</p>

Community curated and predicted equivalences and related mappings between named biological entities that are not
available from primary sources.

Human-curated true mappings are
in [`src/biomappings/resources/mappings.tsv`](https://github.com/biomappings/biomappings/raw/master/src/biomappings/resources/mappings.tsv)
, and automatically predicted mappings are
in [`src/biomappings/resources/predictions.tsv`](https://github.com/biomappings/biomappings/raw/master/src/biomappings/resources/predictions.tsv)
Human-curated *false* (i.e., incorrect) mappings that are non-trivial are
in [`src/biomappings/resources/incorrect.tsv`](https://github.com/biomappings/biomappings/raw/master/src/biomappings/resources/incorrect.tsv)
.

Equivalences and related mappings that are available from the OBO Foundry and other primary sources can be accessed
through [Inspector Javert's Xref Database](https://zenodo.org/record/3757266)
on Zenodo which was described in [this blog post](https://cthoyt.com/2020/04/19/inspector-javerts-xref-database.html).

## ⬇️ Installation

The most recent release can be installed from
[PyPI](https://pypi.org/project/biomappings/) with:

```bash
$ pip install biomappings
```

The most recent code and data can be installed directly from GitHub with:

```bash
$ pip install git+https://github.com/biomappings/biomappings.git
```

To install in development mode, use the following:

```bash
$ git clone git+https://github.com/biomappings/biomappings.git
$ cd biomappings
$ pip install -e .
```

## 🌐 Web Curation Interface

Install with the `web` option as in `pip install biomappings[web]` or just install
`flask` and `flask-bootstrap` then run the following:

```bash
$ biomappings web
```

## 🙏 Contributing Curations

### GitHub Web Interface

GitHub has an interface for editing files directly in the browser. It will take care of creating a branch for you and
creating a pull request. After logging into GitHub, click one of the following links to be brought to the editing
interface:

- [True Mappings](https://github.com/biomappings/biomappings/edit/master/src/biomappings/resources/mappings.tsv)
- [False Mappings](https://github.com/biomappings/biomappings/edit/master/src/biomappings/resources/mappings.tsv)
- [Predictions](https://github.com/biomappings/biomappings/edit/master/src/biomappings/resources/mappings.tsv)

This has the caveat that you can only edit one file at a time. It's possible to navigate to your own forked version of
the repository after, to the correct branch (will not be the default one), then edit other files in the web interface as
well. However, if you would like to do this, then it's probably better to see the following instructions on contributing
locally.

### Locally

1. Fork the repository at https://github.com/biomappings/biomappings, clone locally, and make a new branch
2. Edit one or more of the resource files (mappings.tsv, incorrect.tsv, predictions.tsv)
3. Commit to your branch, push, and create a pull request back to the upstream repository.

## ⚖️ License

Code is licensed under the MIT License. Data is licensed under the CC0 1.0 Universal License.
