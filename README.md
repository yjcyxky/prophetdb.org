<h2 align="center">A website for Ran Lab</h2>
<p align="center">
Ran Lab is a research group in the Department of Molecular and Human Genetics at Shanghai Institute of Health Sciences. We are interested in understanding the molecular mechanisms of human diseases and toxicants, and developing novel therapeutic strategies.
</p>

<p align="center">
<img src="https://img.shields.io/github/license/prophetdb-openlab/prophetdb.org.svg?label=License" alt="License"> 
<a href="https://github.com/prophetdb-openlab/prophetdb.org/releases"><img alt="Latest Release" src="https://img.shields.io/github/release/prophetdb-openlab/prophetdb.org.svg?label=Latest%20Release"/></a>
<a href="https://github.com/prophetdb-openlab/prophetdb.org/actions/workflows/publish-docs.yml"><img alt="Quality Control" src="https://github.com/prophetdb-openlab/prophetdb.org/actions/workflows/publish-docs.yml/badge.svg"/></a>
</p>

## For Developers

### Install Dependencies

```
# Clone the repository
git clone https://github.com/prophetdb-openlab/prophetdb.org.git

cd prophetdb.org

# Create virtual environment
virtualenv .env

# Activate virtual environment
source .env/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### Launch Docs Website

If you want to launch the docs website locally, you can use the following command:

```
mkdocs serve
```

The output should be like this:

```
(quartet-docs) ➜ /quartet-docs git:(master) ✗ > mkdocs serve
INFO     -  Building documentation...
WARNING  -  Config value: 'announce'. Warning: Unrecognised configuration name: announce
WARNING  -  Config value: 'announce_text'. Warning: Unrecognised configuration name: announce_text
INFO     -  Cleaning site directory
INFO     -  The following pages exist in the docs directory, but are not included in the "nav" configuration:
              - about/collaborators.md
              - about/members.md
              - data_dictionary/about.md
              - data_dictionary/metadata.md
              - ...
INFO     -  Documentation built in 3.18 seconds
INFO     -  [09:30:55] Watching paths for changes: 'docs', 'mkdocs.yml'
INFO     -  [09:30:55] Serving on http://127.0.0.1:8000/
```

After that, you can visit the website at `http://127.0.0.1:8000/`. Then you can edit the markdown files and see the changes in real time.

### Modify Docs

Modify the markdown files in the `docs` folder. If you want to modify the table of contents, please modify the `mkdocs.yml` file.

You can follow the [MkDocs](https://squidfunk.github.io/mkdocs-material/) documentation to learn more.

### Publish Docs Website

If you want to submit your changes, please push your changes to your own branch and create a pull request.

```
git checkout -b <Your Branch Name>
git add -u
git commit -m "<Your Message>"
git push origin <Your Branch Name>
```

After merging the pull request, the docs website will be automatically published to [https://prophetdb.org](https://prophetdb.org).
