# Ractive.js Website

## Requirements

- Python 2.7
- pip
- virtualenv
- mkdocs
- mkdocs-cinder

## Setup

```
# 1. Install Python 2.7, pip and virtualenv

# 2. Create a virtualenv
virutalenv ractivejs.github.io
cd ractivejs.github.io

# 3. For this repo and clone your fork.
git clone git@github.com:YOUR_USERNAME/ractivejs.github.io.git src
cd src

# 4. Install dependencies
pip install -r requirements.txt
```

### Development

```sh
# Serve the site
mkdocs serve

# Build the site
mkdocs build
```

Refer to the [mkdocs site](http://www.mkdocs.org) for more information.

## Notes

- Everything goes in the `docs` directory.
- The menu is managed in `mkdocs.yml`.
- Everything is written in markdown.

## TODO

- Automate build with Travis
